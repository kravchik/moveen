([Home](index))


## TODO

**PLANNED RC  _(08.09.17)_**
* performance testing scene
* "sitting in mech" scene


**PLANNED EAP _(25.08.17)_**
* custom leg structure
* automatic rigging
 

## DONE

**EAP 4** _04.08.17_

- 12 bugs

+ demo scene (Unity 5.6.0)
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



**EAP 3** _(10.07.17)_

* better ground detector customization
* template improvements
- anim root rotation (minor bug)
- index out of bounds (minor bug)
+ undo
+ multiple legs editing

