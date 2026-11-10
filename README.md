# skills

Agent skills by [@narasaka](https://github.com/narasaka).

## Install

```sh
# Install all skills
npx skills add narasaka/skills

# Install a specific skill
npx skills add narasaka/skills --skill dotenvx
```

## Available Skills

| Skill | Description |
|-------|-------------|
| [dotenvx](./skills/dotenvx/) | Authoritative CLI reference for [dotenvx](https://dotenvx.com) — encrypt .env files, inject env vars into any process, manage multi-environment secrets, and configure CI/CD pipelines with encrypted env files. |
| [full-send](./skills/full-send/) | Say "full send" to hand off a task end to end: prove the change, review it with `sol-loop`, file the PR, babysit it, and merge once the merge gate passes. |
| [full-stop](./skills/full-stop/) | Same as `full-send`, but stops with the PR ready for you to merge. Never merges. |
| [file-pr](./skills/file-pr/) | File a concise PR: human-readable title, a description that leads with the problem, no AI attribution. |
| [babysit-pr](./skills/babysit-pr/) | Watch a PR through CI and review bots, fix real findings, and dismiss false positives with reasons. Ships `pr-wait`, a single-PR event watcher. |
| [council](./skills/council/) | Say "council" to get three reviewers from two providers (GPT-6.1 Sol, GPT-6 Astra, Claude Fable 5.2), scored per round until all are satisfied. |
| [sol-loop](./skills/sol-loop/) | Say "sol loop" to review a change with GPT Sol in a bounded loop, keeping fixes minimal and scope tight. |
| [leaving-pr-comments](./skills/leaving-pr-comments/) | Rules for GitHub comments posted on your behalf: your voice, no attribution, conclusion first. |
| [attach-media-to-pr](./skills/attach-media-to-pr/) | Screenshot the UI a PR changes at the right viewports and attach the images to the PR. |
| [modernize](./skills/modernize/) | Bring an old PR up to date: check whether the idea still belongs, then rebase, rework, or recommend closing it. |
| [takeover](./skills/takeover/) | Take over a PR, branch, or agent thread and finish it while keeping the original contributors' credit. |

## Skills I use from elsewhere

Other people wrote these, so they're linked here rather than copied. Install them from their own repos:

| Skill | Source | Install |
|-------|--------|---------|
| agent-browser | [vercel-labs/agent-browser](https://github.com/vercel-labs/agent-browser) | `npx skills add vercel-labs/agent-browser --skill agent-browser` |
| gh-stack | [github/gh-stack](https://github.com/github/gh-stack) | `npx skills add github/gh-stack --skill gh-stack` |
| unslop | [cursor/plugins](https://github.com/cursor/plugins) | `npx skills add cursor/plugins --skill unslop` |
| code-review | [mattpocock/skills](https://github.com/mattpocock/skills) | `npx skills add mattpocock/skills --skill code-review` |
| diagnosing-bugs | [mattpocock/skills](https://github.com/mattpocock/skills) | `npx skills add mattpocock/skills --skill diagnosing-bugs` |
| grill-with-docs | [mattpocock/skills](https://github.com/mattpocock/skills) | `npx skills add mattpocock/skills --skill grill-with-docs` |
| grilling | [mattpocock/skills](https://github.com/mattpocock/skills) | `npx skills add mattpocock/skills --skill grilling` |
| prototype | [mattpocock/skills](https://github.com/mattpocock/skills) | `npx skills add mattpocock/skills --skill prototype` |
| retro | [mattpocock/skills](https://github.com/mattpocock/skills) | `npx skills add mattpocock/skills --skill retro` |
| wizard | [mattpocock/skills](https://github.com/mattpocock/skills) | `npx skills add mattpocock/skills --skill wizard` |
| writing-for-agents | [mattpocock/skills](https://github.com/mattpocock/skills) | `npx skills add mattpocock/skills --skill writing-for-agents` |
| resolving-merge-conflicts | [mattpocock/skills](https://github.com/mattpocock/skills/tree/153fc1b93de6584562765cdce299324e1ff9e661/skills/engineering/resolving-merge-conflicts) | Removed upstream; the link points to the last version. |
