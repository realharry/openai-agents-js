# Start Here — Quick path through the examples

This file is a short, curated path for newcomers to the repo. It focuses on a small set of beginner-friendly examples you can run locally with minimal setup.

Prerequisites

- Node.js 22+ and pnpm installed.
- Copy your OpenAI API key to `OPENAI_API_KEY` (or follow the README of each example for provider-specific env vars).

Quick path (15–60 minutes)

1. Basic hello world (core concepts)

```bash
cd examples/basic
# install dependencies for this example
pnpm install
# run the hello-world example (run from repo root)
pnpm -F basic start:hello-world
```

2. Chat (multi-turn conversation)

```bash
pnpm -F basic start:chat
```

3. Stream text (how streaming differs)

```bash
pnpm -F basic start:stream-text
```

4. Tools (calling a simple tool)

```bash
pnpm -F basic start:tools
```

Next steps (after the quick path)

- Try `pnpm -F basic start:agent-lifecycle-example` to inspect lifecycle hooks.
- Explore `examples/agent-patterns/` for intermediate patterns like guardrails and agents-as-tools.
- When ready for integrations, check `examples/tools/` and `examples/mcp/` (note: many integrations require API keys or additional setup).

Troubleshooting & tips

- If you see TypeScript or missing dependency errors, run `pnpm install` at the repository root and then `pnpm -w build` to compile packages.
- Some examples require additional env vars (Twilio, custom model providers). Read the example README for required variables.

Want me to open a PR adding these files to the repository or further annotate each example README with badges? Let me know which you'd prefer.