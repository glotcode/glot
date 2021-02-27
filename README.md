# glot
an open source pastebin with runnable snippets and API.


### Services
- [glot-www](https://github.com/glotcode/glot-www) - glot.io website
- [docker-run](https://github.com/glotcode/docker-run) - code runner api
- [glot-run](https://github.com/glotcode/glot-run) - docker run user management
- [code-runner](https://github.com/glotcode/code-runner) - code runner tool
- [glot-images](https://github.com/glotcode/glot-images) - docker images


### Overview
          glot.io                     run.glot.io
    ┌──────────────────┐   http   ┌──────────────────┐
    │     glot-www     │─────────▶│     glot-run     │
    └──────────────────┘          └──────────────────┘
              │                             │
              │                        http │
              ▼                             ▼
    ┌──────────────────┐          ┌──────────────────┐
    │    postgresql    │          │    docker-run    │
    └──────────────────┘          └──────────────────┘
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
