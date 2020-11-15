---
description: How to edit Sidebars.
---

# Editing Sidebars

The layout of the Sidebar for any given Entity is based on the order and configuration of its Properties. You can modify the order using the Entity Type Editor, and you can change each Property by using the Data Tables and pressing **RightClick** on a Column Head.

Some layouts are hardcoded, but these will be migrated to allow anyone to change them in the future.

## Standard Properties

Some Properties come standard with every Entity. These have fixed positions on the Sidebar and can't be moved. These are:

* Name - Always in the heading.
* Thumbnail - Always in the heading.
* Image - Legacy. Always at the top of the body.
* Icon - Not visible in sidebar. Only used in tags and map markers.
* Spoiler - Work in progress. Not visible in sidebar. People with spoilers hidden will not see the sidebar.

## Renaming Properties

You can rename a Property's name to be more human friendly. Unlike IDs, Property names don't have to be unique.

## Hidden Properties

You can hide Properties from the Sidebar by marking them as Hidden. This is useful for Properties that are used for aiding editors such as datamined identifiers.

## List Properties

By default, Relationship Properties will be shown as:

* A single row if there's one relationship.
* Multiple Entity Rows if there's more than one relationship.
* Hidden if there are no relationships.

To ensure the Sidebar always renders Entity Rows for a Property, even if there's only one, mark it as a List.

## Ordering Relationships

By default, Relationships in a List are ordered by the target Entity's **name** Property. You can change this to any other Property, in either ascending or descending order.

