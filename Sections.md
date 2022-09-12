# API sections

There is an OPTIONS endpoint for each route, the largely include this documention. Although we strive to ensure the documentation is up to date, the OPTIONS request responses always have the most accurate data.

## Entry point

Start here.

- [GET](GET.md)

## Authentication

## Changelog

View all the releases.

- [GET]

## Resource types

In the Costs to Expect API there are three core levels, resource types -> resources -> items.

Items are the individual items defined by the resource type, these could be expenses, items on your Budget or board games for our scoring App.

Resources are the names for the collections, lists or trackers.

Resource types are the base and where we define the item type as well as permitted users and public visibility status.

Any categories and subcategories defined for a resource type are shared among all the resources. Different item types use categories and subcategories in different ways. For the 'allocated-expense' item type, category and subcategories are the expense type, for the 'game' item type, categories are the available players.

- [GET](/resource-types/GET.md)
- [POST](/resource-types/POST.md)

### Resource type

An individual resource type.

- [GET](/resource-type/GET.md)
- [PATCH](/resource-type/PATCH.md)
- [DELETE](/resource-type/DELETE.md)

## Currencies

## Item types

## Resources

Resources act as the groups or containers for items. An item subtype gets set when a resource is created, these allow additional control at the item level. With our game trackers, you define the item type on the resource as "game" and then at the resource level you can further set the specific game, for example "Yahtzee" or "Yatzy".

- [GET](/resources/GET.md)
- [POST](/resources/POST.md)

## Resource

An individual resource.

- [GET](/resource/GET.md)
- [PATCH](resource/PATCH.md)
- [DELETE](/resource/DELETE.md)

## Item subtypes

## Categories

## Subcategories

## Permitted users

## Partial transfers

## Items

## Item categories

## Item subcategories

## Item partial transfer

## Item transfer

## Error log

## Cache
