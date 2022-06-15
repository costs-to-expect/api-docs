# Resource types

View your resource types, access to resource types is controlled by two mechanisms, public status and write permission.

If a resource type is set to 'public' everuone has read access. Write access to a resource and all the dependant routes and endpoints are limted to permitted users. 

The user that creates a resource type is the permitted user, the API allows there to be multiple permitted users per resource type, assigned at the permitted users endpoint.

## Request

**URL** : `/v2/resource-types/`

**Method** : `GET`

**Parameters** :

Parameter | Default | Description | Example
---|---|---|---
collection | | Override pagination and return the entire collection | collection=true
limit | 25 | Limit the collection | limit=25
offset | 0 | Limit offset | offset=0
search | | Search collection fields | field1:partial_search_term\|field2:partial_search_term
sort | | Sort collection | field1:asc|field2:desc


## Response

**Code** : `200 OK`

**Content** : 
```json
[
    {
        "id": "d185Q15grY",
        "name": "Blackborough boys",
        "description": "The Blackborough children, Jack and Niall",
        "created": "2018-09-06 22:04:23",
        "public": true,
        "item_type": {
            "id": "OqZwKX16bW",
            "name": "allocated-expense",
            "description": "Expenses with an allocation rate"
        },
        "resources": {
            "count": 2
        }
    }
]
```