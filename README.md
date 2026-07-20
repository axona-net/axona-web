# axona-web — the axona.net website

The front door of the [Axona](https://github.com/axona-net) protocol, served at
**<https://axona.net>**: the story, the two design commitments (end-to-end —
encryption is the application's responsibility; transport ID and author ID
deliberately separate), the whitepaper, the applications, a **For AI Agents
Only** section pointing at the protocol's AI documentation, agent reviews, and
a popup menu with the full inventory of documents and repositories.

It is a single static file — `index.html` — with a chat/tufte palette
(light + dark), the ant logo in `assets/`, and the whitepaper PDF under
`whitepaper/`. No build step, no framework, no server.

## Layout

```
axona-web/
├── index.html          # the entire site
├── assets/             # logo, favicon, screenshots
├── whitepaper/         # Axona-Whitepaper.pdf (linked from the hero + footer)
├── CNAME               # axona.net (GitHub Pages custom domain)
└── README.md
```

## Develop

Serve the directory statically and open it:

```bash
npx http-server -p 5173 -c-1     # → http://localhost:5173
```

## Deploy

GitHub Pages builds from `main`; the `CNAME` file binds the custom domain
`axona.net`. Push to `main` and Pages redeploys.

## History

This site previously lived in
[axona-net/axona-peer](https://github.com/axona-net/axona-peer) alongside the
reference browser peer application. It moved here to become its own project;
the deprecated peer app remains in the axona-peer repository.

## Ecosystem

| | |
|---|---|
| Protocol kernel | [axona-net/axona-protocol](https://github.com/axona-net/axona-protocol) |
| Group chat | [axona-net/axona-chat](https://github.com/axona-net/axona-chat) → <https://axona.chat> |
| Documentation | [axona-net/axona-docs](https://github.com/axona-net/axona-docs) |

## License

MIT
