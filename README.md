# glot
an open source pastebin with runnable snippets and API.


### Components
- [glot-www](https://github.com/prasmussen/glot-www) - glot.io website
- [glot-snippets](https://github.com/prasmussen/glot-snippets) - snippets api
- [glot-run](https://github.com/prasmussen/glot-run) - code runner api
- [glot-code-runner](https://github.com/prasmussen/glot-code-runner) - code runner tool
- [glot-containers](https://github.com/prasmussen/glot-containers) - docker containers

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

### Instructions for adding a new language
[https://github.com/prasmussen/glot/wiki/Instructions-for-adding-a-new-language-to-glot.io](https://github.com/prasmussen/glot/wiki/Instructions-for-adding-a-new-language-to-glot.io)
