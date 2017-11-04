([Home](https://kravchik.github.io/moveen/))
# Motors

`MotorBean` gathers parameters that describe a character of the abstract movement. They correspond to the real-life motor and its control. 

    distanceToSpeed - converts distance between current position and wanted position
    maxSpeed        - limits maximum speed
    speedDifToAccel - calculates acceleration needed to achieve this speed
    maxAccel        - limits maximum acceleration

Important notice, we are not talking here about force but instead about acceleration. Because of this, you can change the mass of your `RigidBody` and do no changes to the motors.

[Example of currently available presets](https://youtu.be/GG179F6PSwo).

Horizontal, vertical and rotation motors are located in `Stepper5`. Jump motor is located in `MoveControl1` - it is because jumping is actually, achieved by modification of `Stepper5.verticalMotor`.





