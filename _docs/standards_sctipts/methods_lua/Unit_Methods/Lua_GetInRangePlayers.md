---
title: Lua_GetInRangePlayers
type: unit_methods
layout: single_markdown
position: 27
---

# Lua GetInRangePlayers

## Description

Returns a table of player objects, close to pUnit.

## Syntax

```
array = pUnit:GetInRangePlayers()
```

## Example 1

```
function ListNearestPlayer(pUnit)
  for i,pPlayer in pairs(pUnit:GetInRangePlayers()) do
    print(pPlayer:GetName())
  end
end
```

## Example 2

```
function Boss(pUnit, Event)
local targets = pUnit:GetInRangePlayers()
 pUnit:FullCastSpellOnTarget(###, targets)
end
```