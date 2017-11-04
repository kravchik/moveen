([Home](https://kravchik.github.io/moveen/))

## Changelog for 0.7 and upgrade

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


### Upgrade
### New scenario
It is a new "Getting started" scenario I will advertise. As parameters count and ranges didn't stabilize yet, it is advised to choose a model from provided ones and modify them as needed. It is instead of creating a model from scratch, which is still (and will be) possible, but not the easiest way yet.

### Motors
As new motors are grouping and replacing a bunch of old parameters, you need to make these updates for your models. You can easily do this by the button `Stepper5.Upgrade v0.6->v0.7`.
Here are changes that will be done. Notice how old parameters maps to new ones and how new ones are brought in.

    horizontalMotor.distanceToSpeed <= approachSpeedMultiplier
    horizontalMotor.maxSpeed        
    horizontalMotor.speedDifToAccel <= approachAccelerationMultiplier
    horizontalMotor.maxAccel        <= maxAcceleration
                    
    verticalMotor.distanceToSpeed   <= jumpy
    verticalMotor.maxSpeed
    verticalMotor.speedDifToAccel   <= jumpy2
    verticalMotor.maxAccel          <= maxAcceleration
                    
    rotationMotor.distanceToSpeed   <= gaitRotSpeedMul;
    rotationMotor.maxSpeed
    rotationMotor.speedDifToAccel   <= gaitRotForceMul;
    rotationMotor.maxAccel

Horizontal, vertical and rotation motors are located in `Stepper5`. Jump motor is located in `MoveControl1` - it is because jumping is actually, achieved by modification of `Stepper5.verticalMotor`.










