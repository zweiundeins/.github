# zwei und eins gmbh

Simpler software, ready for AI agents. We cut the cost of over-engineered web stacks and make applications usable by AI agents: one process on one server, one SQLite file, HTML over the wire, and an MCP server in front of your API.

A Swiss company in Aarberg, led by [Michael Bolli](https://github.com/mbolli), who has built and looked after web applications for over 20 years.

## What we do

- **Architecture audit**: one to two weeks of code review, a workshop and written findings on where your cost and complexity come from, and what to cut first.
- **Simplify & migrate**: off microservices, serverless or a hyperscaler, step by step, without a big-bang rewrite.
- **Make your app LLM-ready**: an MCP server, an OpenAPI spec, a typed SDK and a permission model your security team can sign off.
- **Agentic development**: we build with your team using coding agents, and show them how to keep quality under control.

Not our focus: marketing-only websites, and frontend projects without backend or architectural responsibility.

## Open source

- **[starbase](https://github.com/zweiundeins/starbase)**: gallery of Datastar web components. Go, templ, SQLite, CQRS: the stack we recommend, end to end.
- **[kanban](https://github.com/zweiundeins/kanban)**: collaborative Kanban board, one Go binary, SQLite, Datastar. Measured against PLANKA, with every script and all raw data.
- **[cashctrl-mcp](https://github.com/zweiundeins/cashctrl-mcp)**: MCP server for the Swiss accounting system CashCtrl. 376 endpoints, read-only unless write mode is on, every write previewed.
- **[cashctrl-ts-sdk](https://github.com/zweiundeins/cashctrl-ts-sdk)**: typed TypeScript client for all 376 endpoints of the CashCtrl API, with an OpenAPI 3.1 spec.
- **[payrexx-go-sdk](https://github.com/zweiundeins/payrexx-go-sdk)** and **[wallee-go-sdk](https://github.com/zweiundeins/wallee-go-sdk)**: Go SDKs for the Swiss payment providers Payrexx and Wallee.

Michael’s own projects include [php-via](https://github.com/mbolli/php-via), a real-time engine for PHP, and [nfsen-ng](https://github.com/mbolli/nfsen-ng), a NetFlow visualiser.

## How we build

- Go and PHP on the server, long-running PHP on OpenSwoole
- SQLite, or MySQL where it is already in place
- HTML over SSE with Datastar, minimal client-side state
- Every number in our [blog posts](https://zweiundeins.gmbh/en/blog) comes with the source and the raw data

## Contact

- **Website:** [zweiundeins.gmbh](https://zweiundeins.gmbh)
- **Email:** info@zweiundeins.gmbh
