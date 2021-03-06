---
title: IsActorInvulnerable
description: Check if an actor is invulnerable.
tags: []
---

# IsActorInvulnerable

<TagLinks />

::: warning

This function was added in SA-MP 0.3.7 and will not work in earlier versions!

:::

## Description

Check if an actor is invulnerable.


| Name | Description |
|------|-------------|
|actorid | The ID of the actor to check.|


## Returns

 1: The actor is invulnerable.

 0: The actor is vulnerable.


## Examples


```c
new MyActor;
 
public OnGameModeInit()
{
    MyActor = CreateActor(179, 316.1, -134.0, 999.6, 90.0); // Actor as a salesperson in Ammunation.
    if(IsActorInvulnerable(MyActor))
    {
        print("Actor is invulnerable.");
    }
    else
    {
        print("Actor is vulnerable.");
    }
    return 1;
}
```


## Related Functions


-  CreateActor: Create an actor (static NPC).
-  SetActorInvulnerable: Set actor invulnerable.
-  SetActorHealth: Set the health of an actor.