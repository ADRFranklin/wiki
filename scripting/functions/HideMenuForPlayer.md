---
title: HideMenuForPlayer
description: Hides a menu for a player.
tags: ['player', 'menu']
---

# HideMenuForPlayer

<TagLinks />

## Description

Hides a menu for a player.


| Name | Description |
|------|-------------|
|menuid | The ID of the menu to hide. Returned by CreateMenu and passed to OnPlayerSelectedMenuRow.|
|playerid | The ID of the player that the menu will be hidden for.|


## Returns

 1: The function was executed successfully. 

 0: The function failed to execute. 


## Examples


```c
if(strcmp(cmdtext, "/menuhide", true) == 0)
{
    new Menu:myMenu = GetPlayerMenu(playerid);
    HideMenuForPlayer(myMenu, playerid);
    return 1;
}
```


## Notes

::: tip

Crashes the both server and player if an invalid menu ID given.

:::


## Related Functions


-  ShowMenuForPlayer: Show a menu for a player.
-  AddMenuItem: Add an item to a menu.
-  SetMenuColumnHeader: Set the header for one of the columns in a menu.
-  CreateMenu: Create a menu.