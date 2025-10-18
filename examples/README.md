# Examples

This directory contains multiple example projects and small demo scripts showing how to use the agents packages in different patterns and environments. Each subfolder is a self-contained example (most have their own `package.json` and a README describing usage). The top-level README below gives a short summary of what each examples subfolder demonstrates and lists the example files contained where useful. Do not rely on this file for run instructions — consult the README inside each example for the authoritative setup and run steps.

## How these examples are organized

- Each subfolder under `examples/` is an independent example app or collection of related small examples.
- Many examples are TypeScript files (.ts) meant to be run with Node (via `ts-node`, `tsx`, or after a build). Others are small projects with their own `package.json`.
- To run an example, change into the example folder and follow that folder's README. Typical steps are:

```bash
cd examples/<example-folder>
# install dependencies (pnpm is used in this repo)
pnpm install
# run the example according to the folder's README or package.json scripts
pnpm start # or pnpm dev | pnpm run <script>
```

## Example folders (high-level summaries)

- agent-patterns/
  - Purpose: A collection of small examples demonstrating agent design patterns and tool usage strategies.
  - Notable example files: `agents-as-tools.ts`, `agents-as-tools-conditional.ts`, `deterministic.ts`, `forcing-tool-use.ts`, `human-in-the-loop.ts`, `human-in-the-loop-stream.ts`, `input-guardrails.ts`, `llm-as-a-judge.ts`, `output-guardrails.ts`, `parallelization.ts`, `routing.ts`, `streamed.ts`, `streaming-guardrails.ts`.
  - See `examples/agent-patterns/README.md` for detailed run instructions and explanations.

- ai-sdk/
  - Purpose: Samples showing usage of the in-repo `ai-sdk` layer and streaming helpers.
  - Notable files: `gpt-5.ts`, `index.ts`, `stream.ts`.

- ai-sdk-v1/
  - Purpose: Legacy or v1 variant of the `ai-sdk` examples for backwards compatibility or comparison.
  - Notable files: `ai-sdk-v1.ts`, `index.ts`, `stream.ts`.

- basic/
  - Purpose: Beginner-friendly examples demonstrating core agent features and small end-to-end scripts.
  - Notable files: `hello-world.ts`, `hello-world-gpt-5.ts`, `hello-world-gpt-oss.ts`, `chat.ts`, `tools.ts`, `local-file.ts`, `local-image.ts`, `remote-image.ts`, `remote-pdf.ts`, `stream-text.ts`, `stream-items.ts`, `agent-lifecycle-example.ts`, `lifecycle-example.ts`, `previous-response-id.ts`, `dynamic-system-prompt.ts`, `prompt-id.ts`, `json-schema-output-type.ts`, `reasoning.ts`, `tool-use-behavior.ts`.
  - See `examples/basic/README.md` for per-example commands and prerequisites.

- connectors/
  - Purpose: Examples showing how to wire connectors (adapters) for third-party services or data sources.
  - Contains various connector demos and an `index.ts` entrypoint.

- customer-service/
  - Purpose: Customer service oriented agent examples (ticket-handling or support workflows).

- docs/
  - Purpose: Documentation-related examples or demos used by the docs site.

- financial-research-agent/
  - Purpose: Domain-specific example focused on financial research tasks and data extraction.

- handoffs/
  - Purpose: Examples showing handoff patterns (escalation or human handoff) between agents and humans or other systems.

- mcp/
  - Purpose: Examples related to Model Context Protocol (MCP) usage and integrations.

- model-providers/
  - Purpose: Examples demonstrating integration with different model providers and provider-specific configuration.

- nextjs/
  - Purpose: Next.js example(s) showing how to integrate agents into a Next.js app.

- realtime-demo/
  - Purpose: Small real-time demo illustrating realtime agent interactions.

- realtime-next/
  - Purpose: Next.js + realtime examples and integrations.

- realtime-twilio/
  - Purpose: Twilio-based realtime examples (telephony or SMS integration).

- research-bot/
  - Purpose: Examples building a research assistant / bot with agent patterns.

- tools/
  - Purpose: Utility tools and helper scripts used by examples or for demonstrating tool-based agent behavior.

- Any additional folders you find in `examples/` should have their own README files. This top-level README intentionally keeps summaries short — check the folder-level README for detailed instructions.

## Contributing new examples

If you add a new example folder:

- Add a short README in the new folder describing purpose and how to run it.
- Keep examples small and focused. Prefer a single-purpose example per folder.
- Update this top-level `examples/README.md` with a one-line description of the new folder and list of notable demo files.

## License and attribution

Examples inherit the repository license. See the project root `LICENSE` for details.


-----

This file is a curated index of the examples shipped with the repository. For hands-on usage and precise run steps, open the README in each example folder.