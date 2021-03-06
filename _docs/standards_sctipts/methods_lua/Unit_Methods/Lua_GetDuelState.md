---
title: Mooo
type: unit_methods
layout: single_markdown
position: 16
---

# Lua GetDuelState

## Description

Will indicate if the unit is in a duel state.

## Syntax

```
int State = pPlayer:GetDuelState()
```

Will return:

---- | ------
 0   | Requested
 1   | Started
 2   | Finished

## Usage/Example

```
wombat = pPlayer:GetDuelState()
if wombat == 0 then
```

```
wombat = pPlayer:GetDuelState()
if wombat == 1 then
```

```
wombat = pPlayer:GetDuelState()
if wombat == 2 then
```

Another example:

```
function OnEnterWorld(event, pPlayer)
wombat = pPlayer:GetDuelState()
if wombat == 0 then
pPlayer:PlayerSendChatMessage(12, 0, "I'm requesting a duel!")
elseif wombat == 1 then
pPlayer:PlayerSendChatMessage(12, 0, "I started a duel!")
elseif wombat == 2 then
pPlayer:PlayerSendChatMessage(12, 0, "I finished!")
end
end
 
RegisterServerHook(4, "OnEnterWorld")
```