([Home](https://kravchik.github.io/moveen/))
## Animation structure

It is advised to look at template models as they incorporate best howtos.
### Creating structure by hand
1. create `GameObject` with `MoveenStepper5` component
2. add needed number of legs as its children. Each leg is a `GameObject` with `MoveenStep2` and skeleton component (`MoveenSkelLeg1` for example)
3. connect meshes for each leg, for each bone ([rigging](rigging))
4. Add `RigidBody` component (or you can use another `GameObject` with `RigidBody` connected via `MoveenStepper5.body`)
5. create `GameObject` and connect it to the `MoveenStepper5` as `target`

To connect Leg meshes - you need to connect them manually to `MoveenSkelLeg1.BonesGeometry` (or `MoveenSkelLeg2.BonesGeometry`) properties (with proper ordering).  

Result should look similar to this:

![Tutorial 1](/images/tutorial01.png)

### Animated object structure example
* some external `GameObject`
  * Stepper (`GameObject` with `MoveenStepper5`)
    * Leg (`GameObject` with `MoveenSkelLeg1`)
    * Leg (`GameObject` with `MoveenSkelLeg1`)
  * Body (`GameObject` wtith `RigidBody`)
    * Body meshes
    * Leg meshes
    * Leg meshes
  * Target (any `GameObject`)

TODO: hip

### Restrictions
* Legs must be contained as children of Stepper
* Stepper must contain 2 or more Legs in its hierarchy
  
