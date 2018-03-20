[Moveen](https://kravchik.github.io/moveen/) (working title) - the engine for automatic animation of any models.
You just connect your model, and it comes alive.
The engine controls it in real-time, which includes:
stepping on any surface and at any speed, responding to recoils, hits and other external influences,
a wide range of settings for the gaits and a smooth transition between walking modes, etc.

With it, game-developer can considerably reduce expenses, as 90% of animations for any model is already done. Let alone technical aspects - animation transitions, runtime reactions, etc.
Animators at the same time can forget about the routine work on general animations and focus on the real art (emotes, game-specific animations, detailed movements, etc.).

_Although the animation of animals looks good, I'm now focusing on debugging animations for robots._

Currently, it is only available as an [**asset for Unity**](https://www.assetstore.unity3d.com/en/?utm_source=gh1#!/content/101452)

* [Unity Asset Store page](https://www.assetstore.unity3d.com/en/?utm_source=gh2#!/content/101452)
* [Forum](https://forum.unity.com/threads/released-moveen-automatic-animation.510063/)
* [**Tutorials**](tutorials)
* [Twitter](https://twitter.com/ykravchik)
* [Facebook](https://www.facebook.com/moveengine/)
* [Youtube](https://www.youtube.com/channel/UCUM1pDB_Ccst8HQFOwYs38A)
* [Changelog](changelog)
* [Roadmap](roadmap)


## Example

{% include youtubePlayer.html id="nTG1xY4QfNU" %}
{% include youtubePlayer.html id="mJUFvYGpS9o" %}


## Getting started (Unity)
### Scenario 1
1. find the closest model to what you need in "Different skels and sizes" scene and copy it to your scene
2. click play button. You can control the model by moving "target" GameObject either directly or by script supplied (currently, it is `MoveControl1`)
3. connect meshes of your model ([rigging](rigging))

_If there is no template corresponding to your needs and you can't modify present ones to match - let me know! I'll try to help you with tuning, and possibly even add template model to the library._

### Scenario 2 (extended level)
1. create **Moveen biped** or **Moveen Quadruped** template (GameObject menu or Inspector "create" menu or inspector right click menu) 
_TODO: replace menu entries with prefabs_
2. click play button (you can control the model by moving "target" GameObject)
3. tune sizes, structure, and parameters. Look at parameters in completed template models (in scenes supplied) to get an idea how to achieve the desired behavior.
4. (OPTIONAL)
    * press `MoveenStepper5<Create from skeleton>` button (it will create draft geometry corresponding to the skeleton, which you can use as a base for prototyping) 
    * OR connect meshes of your model ([rigging](rigging))

### Common tips
* _you can apply any forces to the `RigidBody` of the animation. It could be collisions, recoils, hits, or anything. Animation engine will react appropriately_
* _you can use geometry prefabs from the library to prototype layout, silhouette, and animation even before actual mesh modeling_


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
[Changelog](changelog), [Future plans](roadmap)


* jump / jumping run
* "sitting in mech" demo
* Java version
* Unreal port




## Known issues:
* not following cs code convention

## More info 

[Unity Asset Store page](https://www.assetstore.unity3d.com/en/?utm_source=gh3#!/content/101452)

[Forum](https://forum.unity.com/threads/released-moveen-automatic-animation.510063/)

[**Tutorials**](tutorials)

[Project page amd online documentation](https://kravchik.github.io/moveen/)

[Rigging](rigging)

[Animation struture](structure)

[Gait tuning](gait)


More examples and current progress:
* [Facebook](https://www.facebook.com/moveengine/)
* [Youtube](https://www.youtube.com/channel/UCUM1pDB_Ccst8HQFOwYs38A)
* [Twitter](https://twitter.com/ykravchik)

Unity assets with best robot models out there (I am using them for some showcases):
* [Mech Constructor: Spiders and Tanks](https://www.assetstore.unity3d.com/en/?utm_source=moveengh#!/content/54074)
* [Mech Constructor: Light and Medium Robots](https://www.assetstore.unity3d.com/en/?utm_source=moveengh#!/content/39969)

