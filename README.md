# glot
an open source code playground.


### Components

| Name                                                   | Description
|:-------------------------------------------------------|:------------------------------|
| [glot-app](https://github.com/glotcode/glot-app)       | glot.io website               |
| [docker-run](https://github.com/glotcode/docker-run)   | Code runner api               |
| [glot-images](https://github.com/glotcode/glot-images) | Docker images                 |
| [code-runner](https://github.com/glotcode/code-runner) | Code runner                   |


### Overview
```
                   glot.io
             ┌──────────────────┐
             │     glot-app     │
             └──────────────────┘
                      │
                      │
                      ▼
             ┌──────────────────┐
             │    docker-run    │
             └──────────────────┘
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
