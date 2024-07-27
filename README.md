# Four-Gears-in-Cinema-4D

# Description 
In this project, 4 gears are connected to move together using Cinema 4D. The total ratio of the 4 gears is 18:1. 

# Steps 
## 1. Choosing the number of teeth in each gear 
In this project, the ratio is required to be 18. The ratio calculation for 4 gears is done using the following formula: 
```
(T2/T1) ∙ (T3/T2) ∙ (T4/T3)
```
Since we’ll be using Cinema 4D, the minimum number of teeth a gear can have is 5. In this case, the T2 and T3 will each have their reciprocal, so we can cancel them and have a final formula of T4/T1 which should equal 18. T2 and T3 can be chosen as any value (if the only value we care about is the total ratio).
```
(a/T1) ∙ (b/a) ∙ (T4/b) = 18 
T4/T1 = 18 
T4/5 = 18 
T4 = 90
``` 
The values of T2 and T3 were chosen here to be 20 and 50, respectively. 

## 2. Building the gears in Cinema 4D 
**a.**	 Add a cogwheel from create – spline --  cogwheel. <br />
**b.**	 Change the number of teeth to desired. <br /> 
**c.**	 Add a cylinder, change its orientation to +Z, and place it at the center of the cogwheel. <br />
**d.**	 Add an **Extrude** and add the cogwheel under it. <br />
**e.**	 **Make** both the cogwheel and the cylinder **editable**. (ensure you do all the desired edits before this step) <br />
**f.**	 Click on the **Extrude**, and add a tag to it by going to Tags – Simulation tags -- **Rigid body**. <br />
**g.**	 Click on the **cylinder**, and add a tag to it by going to Tags – simulation tags -- **collider body**. <br />
**h.**	 For the cylinder, go to **shape** and change it to **Moving mesh**.  <br />
**i.**	 Add a connector by going to **Simulate** in the toolbar -- **Dynamics** -- **Connector**. Add the extrude and the cylinder in objects A and B in the connector. Make 
         sure to place the connector at the center of the cylinder, it will show up in the perspective.  <br />
**j.**	 Now add a motor by going to **Simulate** in the toolbar -- **Dynamics** -- **Motor**. Add the extrude in object A. Make sure to place the motor at the center of the 
         cylinder, it will show up in the perspective.  <br />
**k.**	 Finally, change the angular speed as desired and run the animation. The wheel will start rotating.  <br />

These steps are for one gear, repeat them 3 more times, except for the motor, only one motor is needed. Make sure to place the gears close to each other with their teeth aligned correctly to move together. 

# Results 
The final result of the gears should look similar to the ones in the figure below. 

![image](https://github.com/user-attachments/assets/c0268492-a427-4a1a-a6b4-5d62fa40a69c)
<br />

![image](https://github.com/user-attachments/assets/8e155a50-c40e-4f6c-a035-c996e9582d9f)

<br /> 
You can change the colours of the gears to make them clearer maybe, or more "viewable" than all having the same colour with the background.
<br /> 



<img width="500" alt="image" src="https://github.com/user-attachments/assets/011813e9-f17a-4d85-99d6-118d73bd50e5">

