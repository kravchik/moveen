([Home](index))

[Future plans](roadmap)

## DONE



**RC 1** _16.09.17_

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



**EAP 4** _04.08.17_

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



**EAP 3** _(10.07.17)_

* better ground detector customization
* template improvements
- anim root rotation (minor bug)
- index out of bounds (minor bug)
+ undo
+ multiple legs editing

