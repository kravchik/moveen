Moveen (working title) - the engine for automatic animation of any models.
You just connect your model, and it comes alive.
The engine controls it in real-time, which includes:
stepping on any surface and at any speed, responding to recoils, hits and other external influences,
a wide range of settings for the gaits and a smooth transition between walking modes, etc.
With it, the animator can forget about the routine work on general animation and focus on game-specific animations.

Although the animation of animals looks good, I'm now focusing on debugging animations for robots.

Currently, it is only available as an **asset for Unity**. And, it is in the alpha testing mode, and a link will come later. Stay tuned.

## Example

{% include youtubePlayer.html id="nTG1xY4QfNU" %}
{% include youtubePlayer.html id="mJUFvYGpS9o" %}

## Getting started (Unity)
0. unpack Moveen archive into Assets directory of your project (while there is no Asset store entry yet)
1. create **Moveen biped** or **Moveen Quadruped** template (GameObject menu or Inspector "create" menu or inspector right click menu) 
1. click play button (you can control the model by moving "target" GameObject)
1. (optional)
  * connect meshes of your model ([rigging](rigging))
  * OR press `MoveenStepper5<Create from skeleton>` button (it will create draft geometry corresponding to the skeleton, which you can use as a base for sketches) 



## Features
* tunable walking animations
* bipeds and multipeds
* 1-2 knee leg types
* reaction to recoil and external force
* any surface relief
* animation of body, legs, and hip (optionally)
* any walking/running style
* smooth walking mode transition 
* no legs "sliding"

## Upcoming features
* better bipedal behaviour
* simpler rigging system
* jump / jumping run
* "sitting in mech" demo
* other leg structure types
* Java version
* Unreal port

## Known issues:
* RigidBody for the body can only have weight = 1
* not following cs code convention

## More info 

[Rigging](rigging)

[Animation struture](structure)

[Gait tuning](gait)


More examples and current progress:
* [Youtube](https://www.youtube.com/channel/UCUM1pDB_Ccst8HQFOwYs38A)
* [Twitter](https://twitter.com/ykravchik)

Unity assets with best robot models out there (I am using them for some showcases):
* [Mech Constructor: Spiders and Tanks](https://www.assetstore.unity3d.com/en/#!/content/54074)
* [Mech Constructor: Light and Medium Robots](https://www.assetstore.unity3d.com/en/#!/content/39969)

{% include vk.button.html %}
