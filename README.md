# glot
an open source pastebin with runnable snippets and API.


### Services
- [glot-www](https://github.com/glotcode/glot-www) - glot.io website
- [docker-run](https://github.com/glotcode/docker-run) - code runner api
- [glot-images](https://github.com/glotcode/glot-images) - docker images
- [code-runner](https://github.com/glotcode/code-runner) - code runner


### Overview
```
                   glot.io
┌────────────────────────────────────────────┐
│                  glot-www                  │
└────────────────────────────────────────────┘
          │                         │
          │                         │
          ▼                         ▼
┌──────────────────┐      ┌──────────────────┐
│    postgresql    │      │    docker-run    │
└──────────────────┘      └──────────────────┘
                                    │
                                    │
                                    ▼
                       ┌─────────────────────────┐
                       │         docker          │
                       │  ┌───────────────────┐  │
                       │  │    glot-images    │  │
                       │  │  ┌─────────────┐  │  │
                       │  │  │ code-runner │  │  │
                       │  │  └─────────────┘  │  │
                       │  └───────────────────┘  │
                       └─────────────────────────┘
```
