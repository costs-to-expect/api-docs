[API Sections](../Sections.md)
[Resource types](../resource-types/GET.md)
[Resource type](../resource-type/GET.md)
[Resources](../resources/GET.md)
[Resource](../resource/GET.md)

# Items (Budget) - GET

Return the items collection for the given resource.

The `budget` item type is used to define items that appear on a budget, a definition of the item and the frequency with which is repeats.

## Request

**URL** : `/v3/resource-types/{resource_type_id}/resources/{resource_id}/items`

**Method** : `GET`

**Parameters** :

Parameter | Type | Default | Description | Example
---|---|---|---|---
limit | integer | 25 | Limit the collection | limit=25
offset | integer | 0 | Limit offset | offset=0
sort | string | | Sort collection | sort=field1:asc|field2:desc

## Response

**Code** : `200 OK`

**Content** : 
```json
[
    
    ...
]
```
