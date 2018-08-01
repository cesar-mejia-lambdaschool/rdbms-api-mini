# Luis Notes's

## Access RDB from Node

- raw or native driver.
- query builder.
- Object Relational Mapper (ORM)

## Knex (is a query builder)

- Protects against SQL Injection.
- Connection pooling.
- Seeding data.
- Supports promises, callbacks, streams.
- Schema builder. Use DDL statements like create table, drop table.
- Query Builder with a clean JS api.
- Standardization. Normalies DB dialects.

## How to use it

- install it, `npm install knex`
- install a db driver `npm install sqlite3`
- initialize knex `knex init`

## Tables

Create the following tables for the Zoos and Bears collection.

Zoos Table should have the following columns:

id: primary key, automincrements.
name: unique, alphanumeric up to 255 characters long.
created_at: should automatically default to the current date and time.
Bears Table should have the following columns:

id: primary key, automincrements.
zooId: an integer that relates this table to the zoos table. Enforce data integrity.
species: unique, alphanumeric up to 80 characters long.
latinName: alphanumeric up to 80 characters long.
createdAt: should automatically default to the current date and time.
