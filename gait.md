([Home](index))
# Gait tuning


## Stepper5
`Engine` is `Stepper5` field in `<MoveenStepper5>` component. It contains most of the settings related to gait style.  

#### CogUpDown
Center Of Gravity, -1 - bottom, 1 - head

#### CogAngle
Rotate around Center Of Gravity

#### CogForce
Push force to compensate Center Of Gravity

#### BodyLenHelp
Body helps steps length, or opposes rotation (-1 - clumsy, +1 - agile)

#### HipFlexibility
Hip flexibility relatively to the body

#### HipPosRel
Hip position relative to the body (TODO refactor)

#### Jumpy
Force to move body up-down with steps

#### DownOnStep
0.5 - lower body between lands, 1 - no lowering, 1.5 - higher between lands (unnatural)

#### LeadingLegRight
Logical right leg to calculate gait (even for multipeds)

#### LeadingLegLeft
Logical left leg to calculate gait (even for multipeds)



## Step2
#### FootPlatformHeight
Height of foot base

#### StepSpeedMin
Minimal leg stepping speed

#### StepSpeedBodyMul
Leg stepping speed X body speed dependency

#### UndockPause
Pause between leg decided to step, and it actually ups (0 for very light walk, 0.2 and more to add more weight)

#### Step height
Step height is important thing to tune. From the one end, you don't want your model to walk like a heron.
From the other - it doesn't supposed to cling to any ledge. You can tune it with two parameters `Undock Initial Strength` and `Undock Time`.


