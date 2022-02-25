---
title: "Projectiles"
slug: "projectiles"
hidden: false
createdAt: "2020-05-26T05:54:41.881Z"
updatedAt: "2020-05-26T15:15:50.197Z"
---
* Projectile Assets are fired by Entities using the Gun Component, or can be fired with MBScript / Wiring.
* They can be 'HitScan' projectiles, that do a raycast and damage on anything hit, or can have physics and a Launch Velocity set.
* They can have a Muzzleflash <<glossary:Effect Asset>>. And a "ProjectileEffectOnDestroyed" to do [Effects](doc:effects) when the projectile is destroyed, such as explosions.
* They can have a Fire Sound [AudioClip](doc:audioclip) 
* New Projectile assets can be created ingame by cloning a existing asset, or creating a new one and setting it's 'Base'
* Effect assets in the Creation mod can have new components added to them.


[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/34db184-Projectiles.png",
        "Projectiles.png",
        2616,
        1172,
        "#244f62"
      ],
      "caption": "A Arrow projectile asset with Launch Velocity / Physics, and a Hitscan one for bullet damage."
    }
  ]
}
[/block]