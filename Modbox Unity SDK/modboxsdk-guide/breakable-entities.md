---
title: "Breakable Entities"
slug: "breakable-entities"
hidden: false
createdAt: "2020-05-25T05:28:15.982Z"
updatedAt: "2020-05-26T14:21:39.638Z"
---
Entities can break ('Die') by damage (if they have EntityDamageSystem, or their PhysicsMaterial has a 'break on damage' amount, damage then done by explosions/sword/knife). They can also break by force if 'Break On Impact Speed' is set in their physics material (like for Glass)

A easy way to set up destruction is add your Destroyed parts to the game object, and set them as inactive. Then use the 'EntOnDeathParts' component and add those parts to the 'ActivateAndDisconnectOnDestroyed' list. When the entity breaks it will deactive itself, then active these.

Another option is the 'EntShatterOnDeath' which will procedurally generate the shattered mesh parts. This is normally only used for simple primitives.