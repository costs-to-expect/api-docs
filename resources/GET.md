# Resources - GET

View your resources, this will be every resource that exists below the selected resource type.

## Request

**URL** : `/v3/resource-types/{resource_type_id}/resources`

**Method** : `GET`

**Parameters** :

Parameter | Type | Default | Description | Example
---|---|---|---|---
collection | boolean | false | Override pagination and return the entire collection | collection=true
limit | integer | 25 | Limit the collection | limit=25
offset | integer | 0 | Limit offset | offset=0
search | string | | Search collection fields | field1:partial_search_term\|field2:partial_search_term
sort | string | | Sort collection | field1:asc|field2:desc
item-subtype | string | | Filter by itype type | item-subtype=a56kbWV82n


## Response

**Code** : `200 OK`

**Content** : 
```json
[
    {
        "id": "Eq9g6BgJL0",
        "name": "Niall",
        "description": "Niall James Blackborough, born on the 22nd April 2019 at 17:46, these are all the expenses we have recorded for him.",
        "data": {
            "birth": "2019-04-22"
        },
        "created": "2019-04-07 11:26:10",
        "item_subtype": {
            "uri": "/v3/item-types/OqZwKX16bW/item-subtypes/a56kbWV82n",
            "id": "a56kbWV82n",
            "name": "default",
            "description": "Default behaviour for the allocated-exense type"
        }
    }
]
```
