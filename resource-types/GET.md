# Resource types - GET

View your resource types, access to resource types is controlled by two mechanisms, public status and whether you are permitted user.

If a resource type is set to 'public' everyone has read access. Write access to a resource and all the dependant routes and endpoints are limted to the permitted users. 

The user that creates a resource type is the permitted user, the API allows there to be multiple permitted users per resource type, assigned via the permitted users endpoint.

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
item-type | | Filter by itype type | item-type=2AP1axw6L7


## Response

**Code** : `200 OK`

**Content** : 
```json
[
    {
        "id": "d185Q15grY",
        "name": "Blackborough boys",
        "description": "The Blackborough children, Jack and Niall",
        "data": null,
        "created": "2018-09-06 22:04:23",
        "public": true,
        "item_type": {
            "uri": "/v3/item-types/OqZwKX16bW",
            "id": "OqZwKX16bW",
            "name": "allocated-expense",
            "description": "Expenses with an allocation rate"
        },
        "resources": {
            "uri": "/v3/resource-types/Z9YJMxawpG/resources",
            "count": 2
        }
    }
]
```