# glot
an open source code playground.


### Components

| Name                                                      | Description
|:----------------------------------------------------------|:----------------------------------------|
| [glot-app](https://github.com/glotcode/glot-app)          | glot.io website                         |
| [glot-images](https://github.com/glotcode/glot-languages) | Language definitions and docker images  |
| [docker-run](https://github.com/glotcode/docker-run)      | Code runner api                         |
| [code-runner](https://github.com/glotcode/code-runner)    | Code runner                             |


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
