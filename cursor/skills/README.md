# Agent Skills

Skills seem to have to be enforced when prompting. With Opeus 4.5 in Cursor I have had the agent engage with the skills by adding `consult your skills in the vercel-react-best-practices SKILL.md` to my prompt.

## Vercel Labs

They have 2 skillsets: [react-best-practices](https://vercel.com/blog/introducing-react-best-practices) and [web-design-guidelines](https://github.com/vercel-labs/agent-skills/tree/main?tab=readme-ov-file#web-design-guidelines).

### Installation

Using npx: `npx add-skill vercel-labs/agent-skills`:

```
$ npx add-skill vercel-labs/agent-skills
Need to install the following packages:
add-skill@1.0.15
Ok to proceed? (y) y


┌   skills 
│
◇  Source: https://github.com/vercel-labs/agent-skills.git
│
◇  Repository cloned
│
◇  Found 2 skills
│
◇  Select skills to install
│  vercel-react-best-practices
│
◇  Detected 1 agent
│
●  Installing to: Cursor
│
◇  Installation scope
│  Project

│
◇  Installation Summary
│
│    vercel-react-best-practices
│
│      → Cursor: .cursor/skills/vercel-react-best-practices

│
◇  Proceed with installation?
│  Yes
│
◇  Installation complete

│
◆  Installed 1 skill to 1 agent
│
│    ✓ vercel-react-best-practices → Cursor

│
└  Done!
```