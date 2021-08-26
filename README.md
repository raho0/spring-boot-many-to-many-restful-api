# spring-boot-many-to-many-restful-api
| field     | type              | description                                                  | default | example      |
| --------- | ----------------- | ------------------------------------------------------------ | ------- | ------------ |
| tags      | String (required) | A comma separated list of tags.                              | N/A     | science,tech |
| sortBy    | String (optional) | The field to sort the posts by. The acceptable fields are: <br>● id <br>● reads <br>● likes <br>● popularity | id      | popularity   |
| direction | String (optional) | The direction for sorting. The acceptable fields are: <br>● desc <br>● asc | asc     | asc          |

Example: 

```
http://localhost:8080/api/posts?tags=history,tech&sortBy=likes&di
```

```json
[
    {
        "id": 2,
        "author": "Zackery Turner",
        "likes": 469,
        "popularity": 0.68,
        "reads": 90406,
        "tags": [
            "startups",
            "tech",
            "history"
        ]
    },
    {
        "id": 1,
        "author": "Rylee Paul",
        "likes": 960,
        "popularity": 0.13,
        "reads": 50361,
        "tags": [
            "tech",
            "health"
        ]
    }
]
```

