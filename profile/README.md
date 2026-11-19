# zwei und eins gmbh

Simpler software, better margins. For SaaS companies whose cloud bill grows with every customer and whose team spends more time on operations than on features: we make the product simpler, one server at a fixed price and code your team can change quickly again.

A Swiss company in Aarberg, led by [Michael Bolli](https://github.com/mbolli), who has built and looked after web applications for over 20 years.

## What we do

- **Find out where your margin goes**: one to two weeks of code review, a workshop and written findings on where your cost and complexity come from, and what to cut first.
- **Bring the costs down**: off microservices, serverless or a hyperscaler, to one server at a fixed price. The audit shows how gradually that can happen.
- **Ship faster again**: we build with your team and coding agents, in a codebase small enough that someone can still read every change.
- **Your product in AI agents**: an MCP server in front of your existing API, with a permission model your security team can sign off. You decide what an agent may read and write.

## Open source

The runtime and the apps that show the approach:

- **[lith](https://github.com/zweiundeins/lith)**: the Go runtime for our SQLite and Datastar apps. One writer applies every write in order, each changed view renders once per tick for everyone who has it open, and goes out compressed over SSE. [zweiundeins.gmbh](https://zweiundeins.gmbh) and our SaaS [Libretto](https://libretto.ch) run on it. [Docs](https://lith.zweiundeins.gmbh/docs).
- **[tickit](https://github.com/zweiundeins/tickit)**: an issue tracker and a wiki that several people use at once, live: the public demo of lith, with event sourcing and ProseMirror co-editing. [Try it](https://tickit.zweiundeins.gmbh).
- **[kanban](https://github.com/zweiundeins/kanban)**: a collaborative Kanban board on lith, measured against PLANKA, with every script and all raw data. [The measurements](https://zweiundeins.gmbh/en/blog/spa-vs-hypermedia-a-collaborative-kanban-board-measured-against-planka).
- **[starbase](https://github.com/zweiundeins/starbase)**: a gallery of Datastar Rocket web components. [Browse it](https://starbase.zweiundeins.gmbh).

Building blocks:

- **[lith-coedit](https://github.com/zweiundeins/lith-coedit)**: co-editing for lith apps: ProseMirror documents committed through lith's writer, with carets and comments.
- **[prosemirror-go](https://github.com/zweiundeins/prosemirror-go)**: a Go port of ProseMirror's document model and transform, standard library only, tested against upstream ProseMirror.

For Swiss services:

- **[cashctrl-mcp](https://github.com/zweiundeins/cashctrl-mcp)**: MCP server for the Swiss accounting system CashCtrl. 376 endpoints, read-only unless write mode is on, every write previewed.
- **[cashctrl-ts-sdk](https://github.com/zweiundeins/cashctrl-ts-sdk)**: typed TypeScript client for all 376 endpoints of the CashCtrl API, with an OpenAPI 3.1 spec.
- **[payrexx-go-sdk](https://github.com/zweiundeins/payrexx-go-sdk)** and **[wallee-go-sdk](https://github.com/zweiundeins/wallee-go-sdk)**: Go SDKs for the Swiss payment providers Payrexx and Wallee.

Michael's own projects include [php-via](https://github.com/mbolli/php-via), a real-time engine for PHP; [nfsen-ng](https://github.com/mbolli/nfsen-ng), a NetFlow visualiser; [php-ron](https://github.com/mbolli/php-ron), RON for PHP; and the Datastar plugins [data-on-keys](https://github.com/mbolli/datastar-attribute-on-keys) and [data-prop](https://github.com/mbolli/datastar-attribute-prop).

## How we build

- Go on the server, on lith; PHP where it is already in place, long-running on OpenSwoole with php-via
- SQLite, or MySQL where it is already in place
- HTML over SSE with Datastar, minimal client-side state
- Every number in our [blog posts](https://zweiundeins.gmbh/en/blog) comes with the source and the raw data

## Contact

- **Website:** [zweiundeins.gmbh](https://zweiundeins.gmbh)
- **Email:** info@zweiundeins.gmbh
