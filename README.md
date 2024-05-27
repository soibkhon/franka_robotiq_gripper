# franka_robotiq_gripper


In order to connect the robotiq 2F-85 gripper with the custom mount the settings in the Franka FCI had to be changed

.![Screenshot from 2024-05-13 02-47-19](https://github.com/soibkhon/franka_robotiq_gripper/assets/57484946/6f0f8adf-60d9-4782-acb4-c0d1bf93be0f)

The base numbers were taken from the gripper manual and the measurements of custom mount added, the weight was calculated manually.

Intertia matrix is taken from the manual

The mount is 0.05m and it was added to Z axis of the Center of mass vector, also the distance between the mounting point of end-effector untill the gripping point centre was measured and added to the translational matrix. The end-effector is rotated about -45 degrees, it was counted into the translational matrix too.
![image](https://github.com/soibkhon/franka_robotiq_gripper/assets/57484946/7899021d-c4c7-4a5f-9f92-c49ad9cff1e2)
![image](https://github.com/soibkhon/franka_robotiq_gripper/assets/57484946/6e1d21f5-e202-4d67-8b75-43b149431b5a)


**FrankaHW: Failed to initialize libfranka robot. libfranka: Incompatible library version (server version: 4, library version: 5). Please check https://frankaemika.github.io for Panda system updates or choose a libfranka version that uses the server version 4 from the table at https://frankaemika.github.io/docs/compatibility.html .**

If you face above error checkout this compatibility list: https://frankaemika.github.io/docs/compatibility.html
In my case I needed to install the libfranka 0.8.0 version for everything to work fine, no other versions worked for me
