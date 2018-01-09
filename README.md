# kinematicBoatController
Kinematic boat controller for Unity

## Setup
- Create a GameObject and put the KinematicManager and WaterProviderBasic on it.  
- On your boat object, add the KinematicController, KinematicBuoyancy, and KinematicVehicleBasic components.
-  Optionally, on your camera add the FollowCamBasic component. 

## Notes

This is all still very much a work in progress.  But hopefully it provides at least a starting point for others who need a kinematic boat controller.

KinematicManager.PenetrationTestMask sets which objects should be checked for penetration, and depenetrate from.
KinematicManager.InteractiveObjectMask sets which objects should get pushed away with more force.

Depenetration uses the DepenAccel, DepenDecel, and DepenPushSpeed variables.  However for interactive objects DepenPushSpeed is forced to 1.  Simple and crude.

KinematicBuoyancy has a number of parameters.  Best to just mess around and see what works best.  They are preset to reasonable defaults.
