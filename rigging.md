([Home](https://kravchik.github.io/moveen/))
# Moveen rigging

Moveen rigging is rather easy. You need to add legs of the appropriate types and then combine position of the skeleton and your model. A result should look like this: 

![Goal](/images/rigging1b.png)

Then just connect GameObjects representing your meshes or bones to matching bones of the skeleton. An example of the process:  

![Tutorial 1](/images/tutorial01.png)

The only detail here is that you don't have full control over the pose of the skeleton.
You need to place bones to appropriate positions but with somewhat indirect control over them.

For the MoveenSkelLeg1 type of leg, you can control leg base, two axes, target position and two bone lengths.

![Rigging SkelLeg1](/images/rigging.leg1.png)

For the MoveenSkelLeg2 type of leg, you can control leg base, two axes, target position, three bone lengths, and style slider.

![Rigging SkelLeg2](/images/rigging.leg2.png)

It is done that way because we need to place skeleton into the comfort position using parameters engine uses to control it.




