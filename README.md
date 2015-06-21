# glot
an open source pastebin with runnable snippets and API.


### Components
- [glot-www](https://github.com/prasmussen/glot-www)
- [glot-snippets](https://github.com/prasmussen/glot-snippets)
- [glot-run](https://github.com/prasmussen/glot-run)
- [glot-code-runner](https://github.com/prasmussen/glot-code-runner)
- [glot-containers](https://github.com/prasmussen/glot-containers)

### Overview
      snippets.glot.io                  glot.io                     run.glot.io
    ┌──────────────────┐   http   ┌──────────────────┐   http   ┌──────────────────┐
    │  glot-snippets   │◀─────────│     glot-www     │─────────▶│     glot-run     │
    └──────────────────┘          └──────────────────┘          └──────────────────┘
              │                             │                             │
         http │                             │                        http │
              ▼                             ▼                             ▼
    ┌──────────────────┐          ┌──────────────────┐          ┌ ─ ─ ─ ─ ─ ─ ─ ─ ─
    │     couchdb      │          │    postgresql    │                 docker      │
    └──────────────────┘          └──────────────────┘          └ ─ ─ ─ ─ ─ ─ ─ ─ ─


##### docker
    ┌────────────────────────┐
    │    glot-containers     │
    │  ┌──────────────────┐  │
    │  │ glot-code-runner │  │
    │  └──────────────────┘  │
    └────────────────────────┘
