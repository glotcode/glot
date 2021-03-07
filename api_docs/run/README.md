## Run API

### Overview
| Action                              | Method | Route                       | Requires token |
|:------------------------------------|:-------|:----------------------------|:---------------|
| [List languages](list_languages.md) | GET    | /api/run                    | No             |
| [List versions](list_versions.md)   | GET    | /api/run/:language          | No             |
| [Run code](run.md)                  | POST   | /api/run/:language/:version | Yes            |
