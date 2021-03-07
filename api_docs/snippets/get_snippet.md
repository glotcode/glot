## Get snippet

##### Get snippet
    curl --request GET \
         --url 'https://glot.io/api/snippets/e2tx9nh4fh'

### Example response data
    {
      "id": "e2tx9nh4fh",
      "url": "https://glot.io/api/snippets/e2tx9nh4fh",
      "created": "2015-04-23T22:03:11Z",
      "modified": "2015-04-23T22:03:11Z",
      "files_hash": "9bdd2b79fafbf81313a79b1df1be5c2671422307",
      "language": "haskell",
      "title": "Hello world",
      "public": true,
      "owner": "anonymous",
      "files": [
        {
          "name": "main.hs",
          "content": "main = putStrLn \"Hello World!\""
        }
      ]
    }
