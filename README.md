Like me, most of you would have struggled to add a new 3d model to the body tracking ARkit.


![alt text](https://github.com/Mouleeswarran/Unity-AR-Foundation---Body/blob/3ecad73837ecb10dd5bb2ed048d6bcbb2df826bc/Screenshot%20(297).png)

AR Foundation Sample Project: 
https://github.com/Unity-Technologies/arfoundation-samples 

This one contains a prefab, so tried to recreate the same number of joints for my rig but I encountered that the whole body is rotated 180 degrees, 
if we change it in prefab after importing it doesn't work.

Apple documentation:
https://developer.apple.com/documentation/arkit/content_anchors/rigging_a_model_for_motion_capture

this one also didn't work, after we tried to recreate the Rig finally made this one.
I got the transform value dump of each joint and will attach here.

Dont's :
Never rename the joints.
Never change the transform values of the rig, either position or rotation, it either flips or messes the mesh.

Do's
Change the position of the 3d model with another rig and position it according to the main rig and then bind it.
Always have an eye on the scale with the sample model.
