# Roadmap

This roadmap covers the open source local runtime core.

## Completed

- [x] Recursive audit redaction
- [x] Fail-closed policy enforcement
- [x] Policy simulation and testing
- [x] Optional audit hash-chain integrity (tamper-evident)
- [x] Framework integration examples (LangGraph, OpenAI Agents SDK, Vercel AI SDK, MCP)
- [x] Published to npm (@enforra/sdk-node, @enforra/mcp, @enforra/cli) and PyPI (enforra)

## Near-term

- [ ] More policy condition operator
- [ ] `enforra init` CLI command to scaffold `.enforra/policies/` in any project
- [ ] `enforra report` CLI command for human-readable audit summary from local JSONL
- [ ] Expanded policy pack library: payments, database writes, filesystem, email, Slack, GitHub, package installs
- [ ] Policy packs ship with test cases so teams can run `enforra test` in CI against real scenarios
- [ ] Cross-framework demo: one policy file enforced identically across LangGraph, OpenAI Agents SDK, and Vercel AI SDK
- [ ] Larger benchmark corpus and filesystem audit measurements

## Standard layer

The goal for this OSS core is to become the default way teams define, test, reuse, and prove controls for agent tool calls across any framework or harness.

- [ ] Policy pack registry: community-contributed packs for common agent actions
- [ ] Agent and tool inventory format: structured way to declare what tools an agent can call and what policies apply
- [ ] Multi-agent traceability: chain view across agent handoffs for debugging and evidence
- [ ] MCP tool catalog: policy boundaries and decision traces per MCP tool
- [ ] Observe mode before enforce: run in log-only across a harness before switching to block

## Out of scope for this repository

Hosted API, cloud dashboard, hosted audit retention, team approvals, RBAC, SSO, Slack or email approval flows, compliance reports, and remote tool execution are not part of this OSS core.
