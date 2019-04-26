# cakeDecorator

# Thinking more about the reach goals & getting our baseline ready! 4/24/2019

We have been talking to our mentor for a while and we are thinking about how to integrate our reach goals into our project. One feasible idea we had was to introduce a push button functionality, which would take in user input thus would potentially change the speed of the stepper motor thus the speed at which the syringe pushes down the frosting, or the speed at which the stepper motor attached to the turntable turns.

# New reach goal added & new RPL laser cutted mechanism! 4/22/2019

After talking to our project mentor, we have decided to update our reach goal to further integrate the microcontroller mbed into our project, we have ordered a OV7670 camera with CMOS and FIFO integration to be hooked up onto the MBED and as a reach goal, would do color detection on our cake, determining if the cake has frosting spread out evenly, which would serve as a redundancy check and provide the feedback mechanism needed so that the syringe can operate based on the feedback generated from the camera view. 

We have modified our stepper motor code to account for the functionality of the single stepper motor, attached to a little slot we designed for it connected to the vertical gear, which sits stable in the syringe. 

# Milestone 2 & recent developments! 4/19/2019

Our milestone 2 was to build the 3D printing mechanism using stepper motors and our microcontroller circuit. We have attached the stepper motor to the mbed and made the necessary connections. We have also laser cutted our new CAD, we have improved our vertical gear with stabilizer MDF pieces cut with the RPL lab as well, and ensured that we have a empty spot where the stepper motor can stay in within the MDF. 

![Image of First Build](https://deryavuz.github.com/cakeDecorator/final1.png)

# Our initial developments & Milestone 1! 4/17/2019

We are building a cake decorator with a turntable and two decorator types, one for the sprinkles and the other for the frosting itself. We are using a syringe for our frosting spreader mechanism, tied to a stepper motor and powered by the turning motion of the stepper. Our turntable, as both of our baseline goals, will be turning with a stepper motor as well. 

We have built our syringe structure with a vertical gear involved, which will serve to push the frosting down towards the hole on the bottom of the syringe to decorate the cake. The syringe is not stable as of now but we will stabilize it using the new CAD's that we will make and also will work in RPL.

A stepper motor is attached to the arc of the vertical gear, to automate the turning motion.

We have built our syringe in the RPL lab but our first prototype was not as we expected it to be: the syringe mechanism was not working well, the vertical gear was not fit into the place, there was no room for the stepper motor to stand while controllig the vertical gear.

# Introduction & Goal statement! 4/4/2019

We plan on making a automated cake decorator that places frosting and sprinkle patterns on a baked cake. The cake will be placed on top of a “plate” that moves along a mechanical coordinate-system based track/conveyor belt . The design is based on user-inputted designs (i.e. sprinkles in a circle, sprinkles in a rectangle, frosting, frosting peaks at center, frosting circle, etc.). Given this input, our plate will move along the tracks, and for circular designs, the plate will spin from servo movement and ping-sensors that track distance. We plan on making a servo-controlled syringe to squeeze out the frosting and deposit other toppings.


