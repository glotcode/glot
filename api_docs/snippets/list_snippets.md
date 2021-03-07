## Listing snippets

### List public snippets

##### List snippets
    curl --request GET \
         --url 'https://glot.io/api/snippets'

##### List snippets on page 5 with 3 snippets per page
    curl --request GET \
         --url 'https://glot.io/api/snippets?page=5&per_page=3'

##### List snippets by owner
    curl --request GET \
         --url 'https://glot.io/api/snippets?owner=anonymous'

##### List snippets by language
    curl --request GET \
         --url 'https://glot.io/api/snippets?language=erlang'

##### List snippets by owner by language
    curl --request GET \
         --url 'https://glot.io/api/snippets?owner=anonymous&language=erlang'


### List your snippets (requires api token)

##### List your snippets
    curl --request GET \
         --header 'Authorization: Token 0123456-789a-bcde-f012-3456789abcde' \
         --url 'https://glot.io/api/snippets'

##### List your snippets on page 5 with 3 snippets per page
    curl --request GET \
         --header 'Authorization: Token 0123456-789a-bcde-f012-3456789abcde' \
         --url 'https://glot.io/api/snippets?page=5&per_page=3'

##### List your snippets by language
    curl --request GET \
         --header 'Authorization: Token 0123456-789a-bcde-f012-3456789abcde' \
         --url 'https://glot.io/api/snippets?language=erlang'


### Example response data
    [
      {
        "url": "https://glot.io/api/snippets/e2txam1f3x",
        "id": "e2txam1f3x",
        "created": "2015-04-23T22:04:09Z",
        "modified": "2015-04-23T22:04:09Z",
        "language": "php",
        "title": "Hello world",
        "public": true,
        "owner": "anonymous",
        "files_hash": "7d87ee5fa673a6260abc705d56ac7b35b457f566"
      },
      {
        "url": "https://glot.io/api/snippets/e2txa5itxb",
        "id": "e2txa5itxb",
        "created": "2015-04-23T22:03:41Z",
        "modified": "2015-04-23T22:03:41Z",
        "language": "perl",
        "title": "Hello world",
        "public": true,
        "owner": "anonymous",
        "files_hash": "20f74f4277cafb12cd46e68008574dc92c5be35e"
      }
    ]


### Pagination
Information about pagination is provided by the [Link](http://tools.ietf.org/html/rfc5988) header in the response.
Pagination is controlled by the `page` and `per_page` query parameters. `page` must be >= 1, and `per_page` must
be <= 100. If the `per_page` parameter is not given it defaults to 100.

#### Example link header
    link: <https://glot.io/api/snippets?page=16&per_page=2>; rel="next",
          <https://glot.io/snippets?page=18&per_page=2>; rel="last",
          <https://glot.io/snippets?page=14&per_page=2>; rel="prev",
          <https://glot.io/snippets?page=1&per_page=2>; rel="first"
