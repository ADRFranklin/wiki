---
title: LinkVehicleToInterior
description: Links a vehicle to an interior.
tags: ['vehicle']
---

# LinkVehicleToInterior

<TagLinks />

## Description

Links a vehicle to an interior. Vehicles can only be seen by players in the same interior (SetPlayerInterior).


| Name | Description |
|------|-------------|
|vehicleid | The ID of the vehicle to link to an interior.|
|interiorid | The Interior ID to link it to.|


## Returns

 1: The function was executed successfully. 

 0: The function failed to execute. This means the vehicle does not exist.


## Examples


```c
public OnGameModeInit()
{
    new vehicle1 = AddStaticVehicle(559, 2543.7505, -21.8345, 27.1899, 52.6054, -1, -1);
    LinkVehicleToInterior(vehicle1, 6);
}
```


## Related Functions


-  SetVehicleVirtualWorld: Set the virtual world of a vehicle.
-  SetPlayerInterior: Set a player's interior.