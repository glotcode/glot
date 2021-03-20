# glot
an open source pastebin with runnable snippets and API.


### Components

| Name                                                   | Description
|:-------------------------------------------------------|:------------------------------|
| [glot-www](https://github.com/glotcode/glot-www)       | glot.io website and API       |
| [docker-run](https://github.com/glotcode/docker-run)   | Code runner api               |
| [glot-images](https://github.com/glotcode/glot-images) | Docker images                 |
| [code-runner](https://github.com/glotcode/code-runner) | Code runner                   |


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
