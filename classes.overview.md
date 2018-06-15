([Home](https://kravchik.github.io/moveen/))

WIP

# Classes overview

## Main
#### MoveenStepper5
The cornerstone of the whole library. Contains logic for stepping and pelvis+body animation. Most of the features advertised - located here.
* GameObject where this component is located also has to contain SurfaceDetector and RigidBody components.
* Somewhere in this hierarchy has to be located two or more MoveenStep2 components which will be used to complete walker layout.
#### MoveenStep2
The component that describes one leg properties. Step sizes, speed, etc. You need at least two of these for MoveenStepper5 to work.

Also, you need to have `MoveenSkelSimplestTarget or MoveenSkelLimb1 or MoveenSkelLimb2` on the same GameObject in order to define length, IK, and output for rigging.

## IK
#### MoveenSkelLimb1
#### MoveenSkelLimb2
#### MoveenSkelSimplestTarget

## Move/cam controls

#### MoveenBridle1
#### MoveControl1
#### MoveControl2
#### MoveControl3
#### MoveControl4
#### MoveControl5

## Surface detectors
Surface detectors - implement surface detection for the MoveenStepper5. Must be located on the same GameObject. You can implement your own version with more simple or more complex detection which can utilize specifics of your game. For example, it can be 2D or utilize some sort of grid search. Or the one with specific leg placement and orientation.

#### MoveenSurfaceDetector1
This is the simplest version for example purposes. It loads GC but contains less 10 lines of logic.

#### MoveenSurfaceDetector2
Production ready version. Not pollutes memory, has some properties for fine-tuning.


## Other

#### MoveenScaleHelper
#### GlobalMotor
#### LocalMotor
#### FireControl1
#### FireControl2
#### DirControl
#### EverythingStarter
#### HitScanner
#### HitScannerMouse
#### HitCalculator1
#### SoundStarter
#### Startable
#### StartableMonoBehaviour
...





