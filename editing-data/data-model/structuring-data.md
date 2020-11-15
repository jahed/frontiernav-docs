---
description: How to effectively structure your data.
---

# Structuring Data

{% hint style="warning" %}
This is an advanced topic geared towards maintainers, not contributors.
{% endhint %}

As mentioned previously, FrontierNav uses a graph [data model](./). However, as graphs are extremely flexible and lack restrictions, it helps to view the data in a [relational model](https://en.wikipedia.org/wiki/Relational_model). That is why [Data Tables](../data-tables.md) are the primary interface for editing data.

Initially, adding data is simple: You create tables and add columns to store values. However, as you introduce relationships between tables, you may end up at a point where you need to think about how you want the data to be organised so that everything is linked in an intuitive way for people to navigate. If you've worked with Relational Databases before, like [PostgreSQL](https://en.wikipedia.org/wiki/PostgreSQL) or [MySQL](https://en.wikipedia.org/wiki/MySQL), then this should be familiar. If not, it's easy to get started. Think of it like a puzzle that you need to untangle. This process is known as [normalisation](https://en.wikipedia.org/wiki/Database_normalization). It takes practice but like most things, the more you do it, the easier it gets.

## Useful Links

* [Graph](https://en.wikipedia.org/wiki/Graph_%28abstract_data_type%29) on Wikipedia
* [Graph Database](https://en.wikipedia.org/wiki/Graph_database) on Wikipedia
* [Relational Model](https://en.wikipedia.org/wiki/Relational_model) on Wikipedia
* [Database Normalisation](https://en.wikipedia.org/wiki/Database_normalization) on Wikipedia

