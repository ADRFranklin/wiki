---
title: GetVehicleDistanceFromPoint
description: This function can be used to calculate the distance (as a float) between a vehicle and another map coordinate.
tags: ['vehicle']
---

# GetVehicleDistanceFromPoint

<TagLinks />

::: warning

This function was added in SA-MP 0.3c R3 and will not work in earlier versions!

:::

## Description

This function can be used to calculate the distance (as a float) between a vehicle and another map coordinate. This can be useful to detect how far a vehicle away is from a location.


| Name | Description |
|------|-------------|
|vehicleid | The ID of the vehicle to calculate the distance for.|
|Float:X | The X map coordinate.|
|Float:Y | The Y map coordinate.|
|Float:Z | The Z map coordinate.|


## Returns

A float containing the distance from the point specified in the coordinates.


## Examples


```c
/* when the player types 'vendingmachine' in to the chat box, they'll see this.*/
public OnPlayerText(playerid, text[])
{
	if(strcmp(text, "vendingmachine", true) == 0)
	{
		new
		    Float: fDistance = GetVehicleDistanceFromPoint(GetPlayerVehicleID(playerid), 237.9, 115.6, 1010.2),
		    szMessage[44];
 
		format(szMessage, sizeof(szMessage), "You're %f away from our vending machine.", fDistance);
		SendClientMessage(playerid, 0xA9C4E4FF, szMessage);
	}
	return 0;
}
```


## Related Functions


-  GetPlayerDistanceFromPoint: Get the distance between a player and a point.
-  GetVehiclePos: Get the position of a vehicle.