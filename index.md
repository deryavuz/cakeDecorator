# Frosty: The Cake Decorator!
# Frosty is a pancake decorating machine, with various types of sprinkles, frosting and decorations as options for customization.

# Parts List / Current and Updating!

**Mechanical (These are mostly RPL’ed with laser cutters.)**
1) Approximately ~30 sheets combined of MDF and Acrylic<br />
_~10 sheets of Acrylic, ¼ inch and ⅛ inch varying in size, smoke and black color<br />
~15 sheets of MDF, ¼ inch, smoke color._<br />
2) Vertical gears cut from ⅛ inch black color Acrylic<br />
3) Fake cake cut from ⅛ inch black <br />
4) Sprinkle decorators cut from ⅛ inch MDF smoke color<br />
5) Linear Actuator with metal frames. <br />
**Electronical**<br />
1) 2 stepper motors (NEMA 17 bipolar 1.65"x1.65"x1.57" 4-wire) Datasheet: https://www.omc-stepperonline.com/download/23HS45-4204S.pdf <br />
2) 1 continuous rotation Servo Motor (SunFounder Metal Gear Digital RC Servo) Datasheet: http://wiki.sunfounder.cc/index.php?title=55g_Metal_Gear_Servo <br />
3) MBED LPC1768 Microcontroller Unit. Datasheet: https://www.nxp.com/docs/en/data-sheet/LPC1769_68_67_66_65_64_63.pdf<br />
4) Push Buttons (C&K Switches, Tactile Switch) 
Datasheet: https://www.mouser.com/datasheet/2/60/pts645-1382776.pdf<br />
5) LM741 Op Amps (x2) Datasheet: http://www.ti.com/lit/ds/symlink/lm741.pdf <br />
6) Panasonic Relay DS2E-S-12 Non-Latching Relay Datasheet: https://docs-emea.rs-online.com/webdocs/1061/0900766b81061f6a.pdf <br />
7) IRF510PBF IRF510 Power MOSFET N-Channel Datasheet: https://www.amazon.com/IRF510PBF-IRF510-Power-N-Channel-transistor/dp/B00I6IAGCA <br />


# What we have learned from this project! 5/5/2019

It is really important to think about a feasible design for the idea had in mind before proceeding full on with the production of this design and bringing it to life. We have struggled a lot and lost a lot of time in the process of trying to make the vertical gear work in the syringe structure, and couldn't get it to apply enough pressure until we got the actuator. One of the lessons we have learned is to better design our product, at least have a better idea of its features and do more extensive research about it and visualize it better. <br /> 
Although we were not able to demonstrate a complete product with our reach goals included in it, we have put so much effort into testing and making our product, long hours spent with testing and adapting our design choices. Sometimes we had to toss everything and start over from the beginning, and recut our entire project. <br /> 

# Reach Demo Recap and our Reflections on our Design 5/3/2019

At this point, our final product looks so much more different than how it looked in the first place when we have just started working on it.  

We have presented our final product which was partly unfinished due to technical difficulties and design choices which will be explained further in this section. Our final demo-ed product can be seen in the pictures: it involves the linear actuator squeezing out the frosting bag, the servo making 45-degree angled rotations back and forth to allow the sprinkles to come out, the vertical gear tied to the stepper motor moving the spreader blade up and down to spread the frosting over the cake, and the fake-cake we have cut from RPL turning on our turntable with the stepper motor attached to it. To supply power for the linear actuator and to ensure that it moves up and down in a certain range we have determined so that it could apply appropriate pressure to the frosting bag to squeeze frosting out of the little hole we have drilled in RPL into the base, we needed to supply 1A at the very least to the actuator, which operated on 12Volts. Thus we had to build an H-Bridge to amplify our signal voltage the output of which we would connect to the actuator and integrate our H-Bridge with our MBED which could move the actuator only to one direction: upwards or downwards.  <br /> 

Due to the time constraints, we were not able to further work on the project to perfect it but our next step would be to mimic the H-Bridge structure for the opposite side of movement for the actuator, so we would build another H-Bridge exactly like the one we have got to work for the upwards movement of the actuator so we would achieve continuous movement to push the frosting down out the hole in the bag. <br /> 

# Reach Demo: Problems we have faced 5/2/2019


1) We have stuck with a faulty design structure from the beginning which was the vertical gear syringe structure and tried to improve it in many ways. The mounting of the syringe to the base was almost impossible, since the holes of the base were hard for the syringe to go through to stabilize, and this design choice made filling the syringe really hard. Also the syringe did not have enough power and couldn't provide enough pressure to squeeze the frosting out. <br />  
2) The linear actuator idea and the actual mechanism was provided to us very late in the project's process (approximately two days before the demo was due) thus we did not really have the time nor the expertise to operate the mechanism properly and test it with our previous setup with the steppers and the servo, thus integrate it into our system. <br /> 
3) The actuator got physically stuck right before the demo, and we were unable to get it to move although the other parts of our project were functioning: the turntable was turning with the stepper motor, sprinkles were getting scattered over the fake-cake with the servo motor, and the vertical gear was lowering the spreader blade. Thus our demo was incomplete and we felt really disappointed by that.
<br /> 


# Our Next Goals for the Reach Demo & changing our designs! 4/30/2019

1) Get the linear actuator to work in such a way that it moves up and down in a calibrated speed, integrated with the MBED if possible, through an H-Bridge or some other relay-powered circuit structure. <br />
2) Get the vertical gear structure working in such a way that a spreader blade should be attached to it, and the gear shout lower it up and down towards the cake when prompted. <br />
3) Change the base and mount it below the actuator.<br />
4) Put the servo motor and the stepper motor on the new base, and calibrate the spreading blade lowering with the turning of the turntable, also get the servo motor turning in the range we want to turn so that sprinkles can fall through the little slit that opens up and closes with the movement state. <br />

# Baseline demo progress & Feedback 4/27/2019

We plan to demo our syringe and our turntable working in full function, with a little slit cut into our base to spread the frosting as the syringe pushes it down, and the turntable turns thus we do not have to use the plastic spreader which can stay attached.

We plan to demo our syringe and our turntable working in full function, with a little slit cut into our base to spread the frosting as the syringe pushes it down, and the turntable turns thus we do not have to use the plastic spreader which can stay attached. 
Our baseline demo did not meet the par just yet, and we have decided to switch our design a lot to make this project work the way we want it to work : produce cake decorations!<br />

We have acquired a linear actuator from last year's projects which we have placed out base on top and then mounted it to a stand. Our work in this design is explained further in the reach demo section.<br />


# Thinking more about the reach goals & getting our baseline ready! 4/24/2019

We have been talking to our mentor for a while and we are thinking about how to integrate our reach goals into our project. One feasible idea we had was to introduce a push button functionality, which would take in user input thus would potentially change the speed of the stepper motor thus the speed at which the syringe pushes down the frosting, or the speed at which the stepper motor attached to the turntable turns.

# New reach goal added & new RPL laser cutted mechanism! 4/22/2019

After talking to our project mentor, we have decided to update our reach goal to further integrate the microcontroller mbed into our project, we have ordered a OV7670 camera with CMOS and FIFO integration to be hooked up onto the MBED and as a reach goal, would do color detection on our cake, determining if the cake has frosting spread out evenly, which would serve as a redundancy check and provide the feedback mechanism needed so that the syringe can operate based on the feedback generated from the camera view. 

We have modified our stepper motor code to account for the functionality of the single stepper motor, attached to a little slot we designed for it connected to the vertical gear, which sits stable in the syringe. 

# Milestone 2 & recent developments! 4/19/2019

Our milestone 2 was to build the 3D printing mechanism using stepper motors and our microcontroller circuit. We have attached the stepper motor to the mbed and made the necessary connections. We have also laser cutted our new CAD, we have improved our vertical gear with stabilizer MDF pieces cut with the RPL lab as well, and ensured that we have a empty spot where the stepper motor can stay in within the MDF. 

![Image of First Build](https://deryavuz.github.com/cakeDecorator/final1.jpg)

# Our initial developments & Milestone 1! 4/17/2019

We are building a cake decorator with a turntable and two decorator types, one for the sprinkles and the other for the frosting itself. We are using a syringe for our frosting spreader mechanism, tied to a stepper motor and powered by the turning motion of the stepper. Our turntable, as both of our baseline goals, will be turning with a stepper motor as well. 

We have built our syringe structure with a vertical gear involved, which will serve to push the frosting down towards the hole on the bottom of the syringe to decorate the cake. The syringe is not stable as of now but we will stabilize it using the new CAD's that we will make and also will work in RPL.

A stepper motor is attached to the arc of the vertical gear, to automate the turning motion.

We have built our syringe in the RPL lab but our first prototype was not as we expected it to be: the syringe mechanism was not working well, the vertical gear was not fit into the place, there was no room for the stepper motor to stand while controllig the vertical gear.

# Conceptual Clarifications & Ideas and Goals 4/4/2019

Frosty is a pancake decorating machine, with various types of sprinkles, frosting and decorations as options for customization. We plan on making a automated cake decorator that places frosting and sprinkle patterns on a baked cake, a thinner care like a pancake or a cookie cake. The cake will be placed on top of a “plate” that moves along a mechanical turnrtable, controlled by a stepper motor. We have designed a syringe mechanism using gears to be controlled by a stepper motor to squeeze frosting on the cake. A servo-controlled sprinkle chooser mechanism will let us use toppings of our choice depending on the hole size: cereal, sprinkles etc. 

# Introduction & Goal statement! 4/4/2019

We plan on making a automated cake decorator that places frosting and sprinkle patterns on a baked cake. The cake will be placed on top of a “plate” that moves along a mechanical coordinate-system based track/conveyor belt . The design is based on user-inputted designs (i.e. sprinkles in a circle, sprinkles in a rectangle, frosting, frosting peaks at center, frosting circle, etc.). Given this input, our plate will move along the tracks, and for circular designs, the plate will spin from servo movement and ping-sensors that track distance. We plan on making a servo-controlled syringe to squeeze out the frosting and deposit other toppings.


