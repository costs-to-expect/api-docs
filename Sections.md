# API Sections

There is an OPTIONS endpoint for each route, they largely include this documentation, or more accurately, this documentation was created from the OPTIONS request responses. Although we strive to ensure the documentation is up to date, the OPTIONS request responses should always have the most accurate information.

We have tried to layout this file to match the structure of the API, for some routes that doesn't make sense, we will probably have tacked them on the end.

## Structure Overview

In the Costs to Expect API there are three levels to the main data, `resource types` -> `resources` -> `items`, please review the sections below for additional information on each entity.

## Routes and Verbs

Below is a title for each route and the corresponding verbs, the OPTIONS verb is not listed however there is an OPTIONS endpoint for each route.

*Typically, in addition to the docs, the GET route for the collection includes an overview.* 

### Entry point

Start here.

- [GET](GET.md)

### Schemas

Schema files for all of our data.

- [Schemas](/schemas/Schemas.md)


### Changelog

View all the releases.

- [GET](/changelog/GET.md)

### Currencies

Currencies collection.

- [GET](/currencies/GET.md)

### Currency

An individual currency.

- [GET](/currency/GET.md)

### Queue

View all tbe jobs on the queue.

- [GET](/queue/GET.md)

### Item types

Item types collection.

- [GET](/item-types/GET.md)

### Item type

An individual item type.

- [GET](/item-type/GET.md)

#### Item subtypes

Item subtypes collection.

- [GET](/item-subtypes/GET.md)

#### Item subtype

An individual item subtype.

- [GET](/item-subtype/GET.md)

### Resource types

Resource type collection.

- [GET](/resource-types/GET.md)
- [POST](/resource-types/POST.md)

### Resource type

An individual resource type.

- [GET](/resource-type/GET.md)
- [PATCH](/resource-type/PATCH.md)
- [DELETE](/resource-type/DELETE.md)

#### Categories

Categories collection.

- [GET](/categories/GET.md)
- [POST](/categories/POST.md)

#### Category

An individual category.

- [GET](/category/GET.md)
- [PATCH](/category/PATCH.md)
- [DELETE](category/DELETE.md)

##### Subcategories

Subcategories collection.

##### Subcategory

An individual subcategory.

#### Resources

Resources collection.

- [GET](/resources/GET.md)
- [POST](/resources/POST.md)

#### Resource

An individual resource.

- [GET](/resource/GET.md)
- [PATCH](resource/PATCH.md)
- [DELETE](/resource/DELETE.md)
