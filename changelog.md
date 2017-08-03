




**PLANNED RC  (08.09.17)**
* performance testing scene
* "sitting in mech" scene


**PLANNED EAP (25.08.17)**
* custom leg structure
* automatic rigging
 

**EAP 4** _04.08.17_

+ demo scene
  + terrain
  + bipeds (slow, big, fast, mech)
  + multipeds (tripod, fast 4, big 4, 6)
   
* better bipedal walking and external forces reaction

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

- 10 bugs


**EAP 3** _(10.07.17)_

* better ground detector customization
* template improvements
- anim root rotation (minor bug)
- index out of bounds (minor bug)
+ undo
+ multiple legs editing

