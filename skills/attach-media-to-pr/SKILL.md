---
name: attach-media-to-pr
description: Use when the user asks you to attach media to a PR
argument-hint: "[PR numbers or URLs] [for desktop|tablet|mobile ...]"
---

Screenshot the UI each PR changes and attach the images to it. GitHub hosts every image through `gh --attach`; the repo itself stays untouched.

Arguments: `$ARGUMENTS`

## 1. Scope

Read two things from the arguments: PRs and viewports. Either (or both) may be absent, e.g. `42 43`, `for desktop and mobile`, `#42 for mobile only`.
Use the PRs named in the arguments. With none, use the thread's linked PRs (`list_thread_pull_requests`), else the PR for the current branch. For a stack, take every layer.
For each PR, read `gh pr diff <n> --name-only` and decide whether it changes what a user sees. Screenshot only those; name the skipped ones and why (e.g. "#38 is API-only") in the report.

Then pick each visual PR's viewports:

- If the arguments name viewports, use exactly those, for every visual PR.
- Otherwise decide from the diff. Default to desktop alone. Add mobile (and tablet, if the app lays out differently there) when the change alters how that size looks: media queries or responsive classes (`sm:`, `md:`, `lg:`), breakpoint hooks, a nav or sidebar that collapses, a new grid or flex layout, wide content such as tables or long strings that could overflow a narrow screen. Pure colour, copy or icon changes that reflow the same way at every size stay desktop-only.

Done when every PR is marked _visual_ or _skipped_, and each visual PR has its viewports and its list of screens: the pages, states (hover, open menus, empty and error states) and flows its diff touches.

## 2. Capture

1. Launch the app at the visual PRs' head (the `run` skill, or the repo's own launch instructions). Give pages realistic data, seeding it when they would otherwise be empty.
2. Make a fresh directory with `mktemp -d` for the images, so nothing from earlier runs gets overwritten.
3. With `agent-browser`, capture each screen at the PR's viewports, using these sizes:
   - desktop `1440 900`
   - tablet `820 1180`
   - mobile `390 844`

   Use `--full` for pages taller than the viewport. Capture interactive states (hover, open popovers) once, at the size where they read best.
4. Open every image and look at it: real content loaded, the state you meant, no error toast, nothing clipped.

Done when every screen on every visual PR's list has an image you have looked at.

## 3. Attach

The default behaviour of this is to attach the media in the PR description unless the user asks for something else.
see this docs for details about what args and flags you should be using `gh` cli with: https://docs.github.com/api/article/body?pathname=/en/github-cli/github-cli/attaching-files-with-github-cli

## 4. Report

Give each visual PR's comment link with its image count, and list the skipped PRs with their reasons. Then stop the app and anything else you started.
