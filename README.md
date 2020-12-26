# glot
an open source pastebin with runnable snippets and API.


### Services
- [glot-www](https://github.com/prasmussen/glot-www) - glot.io website
- [glot-snippets](https://github.com/prasmussen/glot-snippets) - snippets api
- [docker-run](https://github.com/glotcode/docker-run) - code runner api
- [glot-run](https://github.com/glotcode/glot-run) - docker run user management
- [code-runner](https://github.com/glotcode/code-runner) - code runner tool
- [glot-images](https://github.com/glotcode/glot-images) - docker images


### Overview
      snippets.glot.io                  glot.io                     run.glot.io
    ┌──────────────────┐   http   ┌──────────────────┐   http   ┌──────────────────┐
    │  glot-snippets   │◀─────────│     glot-www     │─────────▶│     glot-run     │
    └──────────────────┘          └──────────────────┘          └──────────────────┘
              │                             │                             │
         http │                             │                        http │
              ▼                             ▼                             ▼
    ┌──────────────────┐          ┌──────────────────┐          ┌──────────────────┐
    │     couchdb      │          │    postgresql    │          │    docker-run    │
    └──────────────────┘          └──────────────────┘          └──────────────────┘
                                                                          │
                                                                          │
                                                                          ▼
                                                                ┌ ─ ─ ─ ─ ─ ─ ─ ─ ─
                                                                       docker      │
                                                                └ ─ ─ ─ ─ ─ ─ ─ ─ ─
##### docker
    ┌────────────────────────┐
    │      glot-images       │
    │  ┌──────────────────┐  │
    │  │   code-runner    │  │
    │  └──────────────────┘  │
    └────────────────────────┘
