# Raspberry Pi Project
## Traffic Light with guide sounds
#### Student number 2905282

![Screenshot_20250314-020456 Photos](https://github.com/user-attachments/assets/8f0f788e-9af8-40aa-9f3d-8b9f07ccf994)


**Introduction**

The purpose of this project is to make a mini home made *traffic light* and sounds that could act as guide. Traffic lights are an essential part of road systems, they regulate the flow of cars and ensure safety for all drivers. It would be interesting to see such an important system being created at home with the help of the Raspberry Pi. The idea is to make a it so that every 5 seconds, an LED goes from green to yellow to red in an infinite loop. Furthermore, a speaker that let's out sounds to guide depending on the current led light colour. For example, for green, it would let out a "go" sound, for yellow it would let out a "caution" sound, and lastly for red it would let out a "stop" sound two times at the start of each 5 second period. 


**Safety:**
*Note: there is no safety issues with this project, it is extremely safe and poses no threat to the user.*


**Physical -construction:**

The main component of this project is the Raspberry Pi. The Raspberry Pi is a miniature computer that runs on Raspberry Pi OS (linux distribution). It is famously known for creating projects just like this one, the exact model used in this project is the Raspberry Pi 3A. A micro SD card is essential for downloading a raspberry pi imager, which allows us to control the Raspberry Pi without having to use the operating system. By connecting to a headless Pi (without a monitor), it is essential to save log in details as it would be required to connect via hotspot. The connection process to a hotspot network wasn't difficult, it worked on the first couple of tries. The Pi has GPIO pins (A general-purpose input/output), that could act as an input and output port. Jumper wires were connected from the GPIO pins to a breadboard which is a tool used to create temporary circuits, it is used often due to its ease of use and efficiency in creating projects. The jumper wires connected to the Pi were GPIO pins: 22 (green), 27 (yellow) and 17 (red). A tool with three LEDs was connected to the breadboard, that is when the magic happens. A speaker was connected to the Pi through a 3.5 mm port and a USB-A to the laptop for power. The tools were all bought from amazon UK for no more than 40 euros.


*Video that helped with understanding GPIO pins: https://youtu.be/6PuK9fh3aL8?si=VJd7aPW6OBDOtK7C*

*Video that helped construct the project: https://youtu.be/zAxbWTe3P4o?si=sCYA-M_RCvUJIm57*


**Virtual - code:**

Through command prompt (CMD) on windows, the use of the 'nano' command was used to fill in the code for the program. Another code 'python3' was used to initiate the program. 'Pygame' and 'mpg.321' was used to read the sound and output through the connected speaker. When the code initiated, "go.mp3" and "stop.mp3" were swapped despite them being in the right place in the code, a simple fix was to swap them. The "go.mp3", "caution.mp3 and "stop.mp3" had an error, a fix for this was to download new sounds called *"go_fixed.mp3"*, *"caution_fixed.mp3"* and *"stop_fixed.mp3"*. The use of getters and setters, classes and inheritance was used as a way to expand and professionalize the code.


**Ideas for version 2:**

Unfortunately, it wasn't possible to make the program run on boot up. After several attempts with software such as 'systemd' and 'RC.local' it didn't seem to work for this one. It would be nice if the project would immediately start the loop on start up. Furthermore, it would be more interesting if the project had two traffic lights to make an intersection road, the two traffic lights would go against one another, they will display different lights to let cars pass. 



**Video:**



**Conclusion:**

In conclusion, the project successfully worked. The program would have traffic light LED light up every 5 seconds to display a model of a traffic light in an infinite loop, while also having sounds personalized to each LED colour. The Pi project took about 5 hours to construct which can be time consuming but satisfying and worth it in the end. 
