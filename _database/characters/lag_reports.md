---
title: lag_reports
type: characterdb
category: L
layout: single_markdown
---

# lag_reports
This table contains lag reports submitted by players.

## Structure

Field                       | Type        | Default             | Comment
--------------------------- | ----------- | ------------------- | -------
[lag_id](#lag_id)           | int(10)     |                     |        
[player](#player)           | int(10)     |                     |        
[account](#account)         | int(10)     |                     |        
[lag_type](#lag_type)       | smallint(2) |                     |        
[map_id](#map_id)           | int(5)      | 0                   |        
[position_x](#position_x)   | float       | 0                   |        
[position_y](#position_y)   | float       | 0                   |        
[position_z](#position_z)   | float       | 0                   |        
[timestamp](#timestamp)     | timestamp   | CURRENT_TIMESTAMP   | 

### lag_id

The unique ID of the lag report.

This field is automatically incremented for each new report.

### player

The character GUID of the player who submitted the lag report.

### account

The account ID of the player who submitted the lag report.

### lag_type

The type of lag reported by the player.

    0 = Loot
    1 = Auctionshouse
    2 = Mail
    3 = Chat
    4 = Movement
    5 = Spells

### map_id

The ID of the map where the lag was detected.

### position_x

The X coordinate of the player when the lag was reported.

### position_y

The Y coordinate of the player when the lag was reported.

### position_z

The Z coordinate of the player when the lag was reported.

### timestamp

The date and time when the lag report was created.