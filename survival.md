## Survival guide
### Animated object structure example
* some external `GameObject`
  * Stepper (`GameObject` with `MoveenStepper5`)
    * Leg (`GameObject` with `MoveenSkelLeg1`
    * Leg (`GameObject` with `MoveenSkelLeg1`
  * Body (`GameObject` wtith `RigidBody`)
    * Body meshes
    * Leg meshes
    * Leg meshes
  * Target (any `GameObject`)

### Restrictions
* Legs must be contained as direct children of Stepper
* Stepper must contain 2 or more Legs in its hierarchy
* it is not a good idea to have any objects inside Stepper except Leg *(TODO, generate a warning)*.
* Body geometry must be located inside Body, as it is the only way animation will be provided to it

There are no other restrictions, Body and Target can be located anywhere in a hierarchy.

Body geometry plays two roles:
* it contains `RigidBody` component, which is used by the animation engine both to collect external forces and to produce reactions
* it contains body meshes
  
To connect Leg meshes - you need to connect them manually to `MoveenSkelLeg1.BonesGeometry` properties (with proper ordering).  

