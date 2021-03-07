## Create snippet

##### Create anonymous snippet
    curl --request POST \
         --header 'Content-type: application/json' \
         --data '{"language": "python", "title": "test", "public": true, "files": [{"name": "main.py", "content": "print(42)"}]}' \
         --url 'https://glot.io/api/snippets'

##### Create snippet (requires api token)
    curl --request POST \
         --header 'Authorization: Token 0123456-789a-bcde-f012-3456789abcde' \
         --header 'Content-type: application/json' \
         --data '{"language": "python", "title": "test", "public": false, "files": [{"name": "main.py", "content": "print(42)"}]}' \
         --url 'https://glot.io/api/snippets'

### Example request data
    {
      "language": "python",
      "title": "test",
      "public": false,
      "files": [
        {
          "name": "main.py",
          "content": "print(42)"
        }
      ]
    }

### Example response data
    {
      "id": "e374w14ai4",
      "url": "https://glot.io/api/snippets/e374w14ai4",
      "created": "2015-05-05T21:38:36Z",
      "modified": "2015-05-05T21:38:36Z",
      "files_hash": "<deprecated>",
      "language": "python",
      "title": "test",
      "public": true,
      "owner": "anonymous",
      "files": [
        {
          "name": "main.py",
          "content": "print(42)"
        }
      ]
    }
