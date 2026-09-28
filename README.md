# Content Gate

[![skills.sh](https://skills.sh/b/vikingmute/content-gate)](https://skills.sh/vikingmute/content-gate)

`content-gate` is an Agent Skill for a people-first, Google Search
Central–aligned pre-publish gate on blog and guide articles. It favors
quality over page count and refuses search-engine-first shortcuts.

## What It Does

- Loads the project's own writing rules first (`CONTENT_GUIDELINES.md`,
  `guidelines.md`, or similar) and treats them as a hard gate.
- Asks **who is helped** and **what task they can finish** before keywords.
- Runs Who / How / Why, spam and scaled-content hard stops, and a
  pre-publish checklist for helpfulness, trust, craft, and localization.
- Reviews agent-written copy with the same bar as human drafts.
- Produces a pass / conditional / fail verdict with a fix plan when needed.

It is generic: use it on blogs and guides for any site. It does not assume a
product brand.

## Output

Use `assets/templates/gate_report.md` for the write-up. Record:

- `pass`, `conditional`, or `fail`
- the one-sentence Why
- Who / How / Why, hard stops, and the pre-publish checklist
- a fix plan when the verdict is conditional

Put that checklist in the PR or review notes. Titles and metadata alone do
not pass the gate.

## Installation

Install from GitHub with the Skills CLI:

```sh
npx skills add vikingmute/content-gate
```

Or use the full GitHub URL:

```sh
npx skills add https://github.com/vikingmute/content-gate
```

Install globally for a specific agent:

```sh
npx skills add vikingmute/content-gate -g -a codex
```

Install globally for multiple agents:

```sh
npx skills add vikingmute/content-gate -g -a codex -a cursor -a opencode
```

Update an installed copy:

```sh
npx skills update content-gate
```

Update only global installs:

```sh
npx skills update content-gate -g
```

For local development without publishing, clone it into the cross-client Agent
Skills directory:

```sh
git clone https://github.com/vikingmute/content-gate.git ~/.agents/skills/content-gate
```

For a project-local install, copy or clone it into the project:

```sh
mkdir -p .agents/skills
git clone https://github.com/vikingmute/content-gate.git .agents/skills/content-gate
```

Some clients also support their own native skill locations. For Codex, this is
also valid:

```sh
cp -R content-gate ~/.codex/skills/content-gate
```

Then invoke it from a compatible agent with:

```text
Use $content-gate to run the people-first publish checklist on this article.
```

If a client does not support explicit `$skill` syntax, ask it to use the
`content-gate` skill or select it from the client's skills UI.

## Example Prompts

```text
Use $content-gate to run the people-first publish checklist on this article.
```

```text
Use $content-gate before I ship this guide.
```

```text
Use $content-gate to review this draft against our CONTENT_GUIDELINES.md.
```

```text
Use $content-gate on this localization of the getting-started article.
```

```text
Use $content-gate to check this agent-written blog post before merge.
```

## Sources

Content Gate follows public Google Search Central guidance. It is not a
black-hat SEO playbook and does not cover keyword-volume or backlink tactics.

- [Creating helpful, reliable, people-first content](https://developers.google.com/search/docs/fundamentals/creating-helpful-content)
- [Guidance on generative AI content](https://developers.google.com/search/docs/fundamentals/using-gen-ai-content)
- [Spam policies for Google web search](https://developers.google.com/search/docs/essentials/spam-policies)
- [Google Search Essentials](https://developers.google.com/search/docs/essentials)
