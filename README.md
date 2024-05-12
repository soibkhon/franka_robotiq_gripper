# franka_robotiq_gripper


In order to connect the robotiq 2F-85 gripper with the custom mount the settings in the Franka FCI had to be changed

.![Screenshot from 2024-05-13 02-47-19](https://github.com/soibkhon/franka_robotiq_gripper/assets/57484946/6f0f8adf-60d9-4782-acb4-c0d1bf93be0f)

The base numbers were taken from the gripper manual and the measurements of custom mount added, the weight was calculated manually.

The mount is 0.05m and it was added to Z axis of the Center of mass vector, also the distance between the mounting point of end-effector untill the gripping point centre was measured and added to the translational matrix. The end-effector is rotated about -45 degrees, it was counted into the translational matrix too.
