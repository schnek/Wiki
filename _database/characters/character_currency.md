---
title: character_currency
type: characterdb
category: C
layout: single_markdown
---

# character_currency
This table contains the currencies stored for characters.

## Structure

Field                                 | Type                | Default | Comment
------------------------------------- | ------------------- | ------- | ----------------------------------------------------------
[guid](#guid)                         | int(10) unsigned    |         | Character GUID from the `characters` table.
[currency](#currency)                 | int(10) unsigned    |         | Currency ID.
[quantity](#quantity)                 | int(10) unsigned    | 0       | Current currency quantity.
[weekly_quantity](#weekly_quantity)   | int(10) unsigned    | 0       | Currency quantity earned during the current weekly period.
[tracked_quantity](#tracked_quantity) | int(10) unsigned    | 0       | Tracked currency quantity.
[flags](#flags)                       | tinyint(3) unsigned | 0       | Currency flags.

### guid

The character GUID from the `characters` table.

### currency

The currency ID.

### quantity

The current amount of the currency owned by the character.

### weekly_quantity

The amount of currency earned during the current weekly period.

### tracked_quantity

The amount of currency tracked for the character.

### flags

Flags associated with the currency.
