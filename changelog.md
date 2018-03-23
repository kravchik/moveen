([Home](https://kravchik.github.io/moveen/))

[Future plans](roadmap)

## DONE


**v0.82** _23.03.2018_ **runtime skeleton change, important bug-fix**
* tunings, bug-fixes, (including bug with scirpt disable)
* runtime skeleton change
  * runtime leg addition/removal, layout recalculation
  * leg remove + ragdoll
  * leg enable/disable + ragdoll


**v0.81** _16.02.2018_ **new model, tunings, bug-fixes**

* new model: walking gun
* bugs, tunings:
  * limb2 - minLength calculation
  * cursors and aiming refactoring
  * hit scanner (collider ignore hierarchy, dir choosing)
  * -MoveControl5 dir
  * add children button
  * -legs shimmer in some cases
  * better leg pull
  * warning about being in rage, >0, <0, outside of range
  * warning if two rigidbodies are available
  * removed targetUnderground
  * just fired flag
  * -can't move AND rotate a model initially (gizmos and initial setups)
  * -repaint gizmo when rescaling
  * ctr+z in Limb1/Limb2


**v0.8** _08.01.2018_ **directory structure, new scenes, changed joints**

* changed directory structure (Moveen -> Plugins/YK/MoveEn)
* refactored joints children
  * children are moved in editor and in runtime
  * joint never moves by itself
* new scenes
  * simple gun scene
  * top-down arcade
  * MoveControl3
  * MoveControl5
  * simple npc: walk and idle, simple npc: run away
* 2 new models
* 14 tunings and bug fixes 


**v0.79** _16.12.2017_ **removed "beta" status, little fixes, raised price**
* removed "beta" status 
* some fixes
* raised price

**v0.78** _07.12.2017_ **improved limbs editing, performance scene**
* performance
  * performance testing scene
  * removed some runtime memory allocations
* far simpler limbs editing
  * editing helper for MoveenLimb1, MoveenLimb2
  * simplified inspector for MoveenLimb1, MoveenLimb2
  * better limbs visualization
  * Step2.detachedComfortPosRel checkbox (comfort position was detached by default which caused show-stopping if you didn't know that it has to be positioned)
  * refactored gizmos (cleaner code, less rendering)
* MoveenScaleHelper
* some bugs and refactorings 

**v0.75** _23.11.2017_ **guns, sounds, top-down shooter**

* [ragdoll is usable now](https://youtu.be/TddJ_kJamoQ)
* guns
  * gun/hit recoil systems
  * gun fire/aim controller, hitscanner 
  * effect starters 
  * direction controller (for guns and heads)
* [example scene: top-down physical shooter with big mechs (first version)](https://youtu.be/WG4nE5XKLjY)
  * top-down camera controller
  ? stepping events (dust and sound)
  * focus grabber
* 11 prototype sounds
* some bugs fixed

**v0.7** _04.11.2017_ **run, jump, motors, prefabs** 

* large upgrade for stepping  
  * [run and jump](https://youtu.be/lqBbf8qNfAo)
  * better stepping

* [Motors](motors)
  * [vertical/horizontal/rotation](https://youtu.be/GG179F6PSwo) 

* new prefabs for prototyping
  * 2 bodies
  * 11 bones
  * 3 feet
  * 3 guns
  * 2 hips
  
* scene tuning  
* new models with animation templates
  * fast 10m battle mech               
  * [heavy 10m battle mech](https://youtu.be/u9Q6-sILuAo)
  * [fast 5m mech](https://youtu.be/lqBbf8qNfAo)
  * heavy 5m mech

* debug features  
  * visual log for stepping  
  * dials for stepping  

* legs now can be childed in hip
* bend legs in the air
* bugs and tunings

[Full info](change06to07)

**v0.6** _19.10.2017_ **on the store**
* on the store

**RC 2** _29.09.2017_
* automatic ragdoll creation
* transition from/to animation
* transition from/to ragdoll
* common animation mixer
* MoveenTransformCopier
* simpler body structure
* refactored ordered tick 
* triangle counter in Bezier mesh
* more tooltips
* fixed bunch of bugs

**RC 1** _16.09.2017_

* THIS VERSION CONTAINS IMPORTANT MODEL-UPGRADER
* **much more stability in stepping!**
  * better stepping, rotating, jumping
  * better stepping on too-steep slopes
  * predictable stepping in complex bridges, ridges, low ceilings, stairs, etc. (tough one)
  * extended surface detector
* **joints as a separate system**
  * extended elbow2 possibilities
  * added joint primitives, that can be used separately from whole stepping system!
  * you can compose completely new limb structure from joint primitives
  * you can use both "coded" (high performance) and "editor-composed" (easy to do) solutions
  * structures can be used both as limbs and as dynamic decorations for them
* joint primitives
  * sushi
  * hydraulic
  * empty limb (for editor-composed, and for third-party solutions)
  * bezier
    * extendible bezier
    * bezier mesh
      * different start/end radiuses
      * start/end caps
      * custom or Unity normals
      * smart/fast twisting
    * bones
    * prefab 
* better rotation speed limit for MoveControl1 
* ordered execution MonoBehaviour
* reliable limb length limit system
* scene about three strange prototypes
* scene about custom joint structures
* UpdateProto Model and Fill ProtoModel buttons
* surface detectors now use memory friendly solution
* scenes tuning
* production ready directory system
* bugs



**EAP 4** _04.08.2017_

- 12 bugs

+ demo scene (Unity 5.6.0) [(video)](https://twitter.com/ykravchik/status/893830650314338304)
  + terrain
  + bipeds (slow, big, fast, mech)
  + multipeds (tripod, fast 4, big 4, 6)
   
* better bipedal walking and external forces reaction [(video)](https://www.facebook.com/moveengine/videos/1906656052928603/)

+ more gait parameters

* templates tuning

+ bunch of little improvements
    + forbid legs tangling
    + both legs behind -> step (for running-jumping)
    + assert leading leg left, leading leg right
    + comfort radiuses through leg len ratio
    + mass doesn't affect gait
    + show step trajectory, on/off (особенно важно для больших)
    + different up-down for bipeds
    + MoveControl1
      + incline body by legs
      + better height dif handling



**EAP 3** _(10.07.2017)_

* better ground detector customization
* template improvements
- anim root rotation (minor bug)
- index out of bounds (minor bug)
+ undo
+ multiple legs editing

