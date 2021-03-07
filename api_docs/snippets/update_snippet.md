## Update snippet


##### Update snippet (requires api token)
    curl --request PUT \
         --header 'Authorization: Token 0123456-789a-bcde-f012-3456789abcde' \
         --header 'Content-type: application/json' \
         --data '{"language": "python", "title": "test - updated", "public": false, "files": [{"name": "main.py", "content": "print(42)"}]}' \
         --url 'https://glot.io/api/snippets/e374yxuw49'

### Example request data
    {
      "language": "python",
      "title": "test - updated",
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
      "id": "e374yxuw49",
      "url": "https://glot.io/api/snippets/e374yxuw49",
      "created": "2015-05-05T21:41:32Z",
      "modified": "2015-05-05T21:41:53Z",
      "files_hash": "f55a5b888fa89b60b8eb5e71cc0d18aeb50e8c81",
      "language": "python",
      "title": "test - updated",
      "public": false,
      "owner": "427ca0e3-b254-4e97-9326-88c814758af5",
      "files": [
        {
          "name": "main.py",
          "content": "print(42)"
        }
      ]
    }
