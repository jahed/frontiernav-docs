---
description: How FrontierNav's data is structured.
---

# Data Model

If you want to start contributing data to FrontierNav, it's worth knowing how the data is structured.

FrontierNav uses a graph data model for its data which consists of the following concepts. Depending on where and how they're used, they can use different names but still mean the same thing.

* Entity Type \(Table, Category, Relation, Schema\)
* Relationship Type \(Inner Table, Nested Table\)
* Property \(Column, Field, Attribute\)
* Entity \(Row, Entry, Page, Tuple, Node, Vertex\)
* Relationship \(Link, Reference, Edge\)
* Data \(Cell, Value\)

## Entity Type

Entity Types _define_ the structure of Entities using Properties. An Item is an Entity Type, whereas a Small Potion is an Entity.

## Relationship Type

Relationship Types _define_ a link between two Entity Types in one direction. So **Enemies drop Items** and **Items are droppped by Enemies** is one Relationship Type as they mean the same thing.

The first Entity Type _owns_ the Relationship Type, so it can point to as many other Entity Types as it wants. However, the linked Entity Types can only point to the first. So Enemies can drop Items and Weapons, but Weapons can't then be dropped by Treasure Chests. To do that, you'll need another Relationship Type owned by Treasure Chests.

## Property

Properties _define_ the structure of an Entity's Data. For example, an Item has a **price** which is a **number**.

Properties can also _define_ the structure of a Relationship's Data. For example, an Enemy drops an Item at a certain **rate**.

### Property Types

The types of values Properties can define are currently limited to the following:

* Text \("Hello", "A sentence", **string**\)
* Number \(0, 1, 2, 3, **number**\)
* Boolean \(yes/no, true/false, **boolean**\)
* Relationship \(references a RelationshipType\)
* Tunnel \(references a Relationship Property **entrance** and a corresponding Property **exit**\)
  * Useful for re-using data from other Entity Types without having to repeat yourself.
* Attachment \(references a file like an **image**\)

## Entity

An Entity is something that _exists_ in the game world. A Character, Item, Enemy, Mission are all Entity Types, whereas "The Hero", "Small Potion", "Defeat the Dragon" are Entities.

## Relationship

A Relationship _links_ two Entities together. Both Entities will refer to the Relationship in their Data to link them together. For example, **Black Dragons drop Dragon Scales**.

## Data

Data _describes_ an Entity. Where Properties define the structure of Data, Data contains the values. For example, a Small Potion has a **price** of **200** gold.

Similarly, Data helps _describe_ a Relationship: Black Dragons have an **80%** chance to drop Dragon Scales.

