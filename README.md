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
| [screenshots](./skills/screenshots/) | Screenshot UI work at desktop and mobile and show it in chat, or attach it to the PR as one current set. |
| [ticket](./skills/ticket/) | Start a Linear ticket on its Linear branch, solve the problem rather than the ticket's proposed fix, and ship with `full-stop`. |
| [weigh-comments](./skills/weigh-comments/) | Check a teammate's review comments against the code, give each a verdict, and draft replies for you to send. |
| [full-send](./skills/full-send/) | Say "full send" to hand off a task end to end: prove the change, review it with `sol-loop`, file the PR, babysit it, and merge once the merge gate passes. |
| [full-stop](./skills/full-stop/) | Same as `full-send`, but stops with the PR ready for you to merge. Never merges. |
| [file-pr](./skills/file-pr/) | File a concise PR: human-readable title, a description that leads with the problem, no AI attribution. |
| [babysit-pr](./skills/babysit-pr/) | Watch a PR through CI and review bots, fix real findings, and dismiss false positives with reasons. Ships `pr-wait`, a single-PR event watcher. |
| [council](./skills/council/) | Say "council" to get three reviewers from two providers (GPT-6.1 Sol, GPT-6 Astra, Claude Fable 5.2), scored per round until all are satisfied. |
| [sol-loop](./skills/sol-loop/) | Say "sol loop" to review a change with GPT Sol in a bounded loop, keeping fixes minimal and scope tight. |
| [leaving-pr-comments](./skills/leaving-pr-comments/) | Rules for GitHub comments posted on your behalf: your voice, no attribution, conclusion first. |
| [modernize](./skills/modernize/) | Bring an old PR up to date: check whether the idea still belongs, then rebase, rework, or recommend closing it. |
| [takeover](./skills/takeover/) | Take over a PR, branch, or agent thread and finish it while keeping the original contributors' credit. |

## Other skills I use

These belong to other people, so install them from their own repos:

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

## Credits

`full-send`, `full-stop`, `file-pr`, `babysit-pr`, `council`, `sol-loop`, `leaving-pr-comments`, `modernize` and `takeover` are adapted from [Theo Browne](https://github.com/t3dotgg)'s [tstack](https://github.com/t3dotgg/tstack), used under the MIT license:

<details>
<summary>tstack license</summary>

```
MIT License

Copyright (c) 2026 Theo Browne

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

</details>
