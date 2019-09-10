# IDD-Fa18-Lab1: Blink!

**A lab report by Ryan Curtis (rec284)**

> Include your responses to the bold questions on your own fork of the lab activities. Include snippets of code that explain what you did. Deliverables are due next Tuesday. Post your lab reports as `README.md` pages on your GitHub, and post a link to that on your main class hub page.

We've copied the questions from the lab here. Answer them below!

## Part A. Set Up a Breadboard

[photo of my breadboard setup here](https://github.com/rec285/IDD-Fa18-Lab1/blob/master/%25TjRBDY3QCO%25vnap%25sAe%2Bw.jpg)


## Part B. Manually Blink a LED

**a. What color stripes are on a 100 Ohm resistor?**
 100 Ohm resistors have Brown, Black, Brown, then a fourth strip the tolerance. 
 220 Ohm resistors have Red, Red, Brown, then a fourth strip the tolerance. 
 
**b. What do you have to do to light your LED?**
You have to connect power to the resistor and then in the cathode end of the LED. And then connect the anode end of the LED to ground. And then to light the LED, press the button.

## Part C. Blink a LED using Arduino

### 1. Blink the on-board LED

**a. What line(s) of code do you need to change to make the LED blink (like, at all)?**
Lines 28, 33, and 35 need to be changed to have correct pin instead of the built-in LED (in this case, pin 9).

**b. What line(s) of code do you need to change to change the rate of blinking?**
Lines 34 and 36 should be changed to adjust the rate of blinking, a lower number for faster blinking.

**c. What circuit element would you want to add to protect the board and external LED?**
A resistor of addequate resistance should be added to reduce the voltage across the LED and protect the LED and board from burning.
 
**d. At what delay can you no longer *perceive* the LED blinking? How can you prove to yourself that it is, in fact, still blinking?**
At a delay of about 10, you can no longer perceive the blinking. To prove it is blinking, move the LED rapidly in front of you and you will see the LED lit up in spots along the path instead of being continuously on.

**e. Modify the code to make your LED blink your way. Save your new blink code to your lab 1 repository, with a link on the README.md.**
[link to RyanBlink](https://github.com/rec285/IDD-Fa18-Lab1/blob/master/%25TjRBDY3QCO%25vnap%25sAe%2Bw.jpg)

### 2. Blink your LED

**Make a video of your LED blinking, and add it to your lab submission.**

[link to your video here](https://www.youtube.com/watch?v=kRT70IpYGFc&feature=youtu.be)


## Part D. Manually fade an LED

**a. Are you able to get the LED to glow the whole turning range of the potentiometer? Why or why not?**
No because the potentiometer won't be able to turn the LED all the way off and if you set the resistance to 0 the LED will burn.

## Part E. Fade an LED using Arduino

**a. What do you have to modify to make the code control the circuit you've built on your breadboard?**
You have to change the led pin number to be 11 to match the pin connected on the breadboard.

**b. What is analogWrite()? How is that different than digitalWrite()?**
analogWrite() can set a value in between the range of the high and low values where as digitalWrite() can only set high or low and not anything in between.

## Part F. FRANKENLIGHT!!!

### 1. Take apart your electronic device, and draw a schematic of what is inside. 
[photo 1](https://github.com/rec285/IDD-Fa18-Lab1/blob/master/C27s0ZwuSIqoYWnF51CTiw.jpg)
[photo 2](https://github.com/rec285/IDD-Fa18-Lab1/blob/master/UxEomkh4Svefdt5gU0e7BQ.jpg)
[diagram](https://github.com/rec285/IDD-Fa18-Lab1/blob/master/J0lfBY%25OQaOVowN%2Bv15YJg.jpg)

**a. Is there computation in your device? Where is it? What do you think is happening inside the "computer?"**
Yes! There is a lot of computation in this device because it is a computer. The computation primamrily happens in the processors in the center of the green motherboard. There is also computation in a smaller chip under the screen. Inside the computer, power comes from the battery and is then sent to the components where the processor takes any inputs from the keyboard or ports or any other sensors and computes what to do. The fan keeps the computer cool and the processor sends information to the screen to be displayed.

**b. Are there sensors on your device? How do they work? How is the sensed information conveyed to other portions of the device?**
Yes, the keyboard and trackpad are sensors and they work as a collection of buttons and the trackpad is a touch capacitor that responds to touch in the electromagnetic field. It is then sent to the I/O bus to be processed by the CPU and then sent out to other output components.

**c. How is the device powered? Is there any transformation or regulation of the power? How is that done? What voltages are used throughout the system?**
There is an battery powering the computer and is supplied by a charger through one of the ports on the computer. The power is regulated on board with a transformer and outputs voltages between ~2V and ~40V.

**d. Is information stored in your device? Where? How?**
Information is stored on the device in the solid state drive/disk as well as in memory. They are chips on the motherboard.

### 2. Using your schematic, figure out where a good point would be to hijack your device and implant an LED.

**Describe what you did here.**
I used the multimeter to find a point on the motherboard that had a consistent voltage of about 2V to be able to power the LED but not burn it. I then placed the LED in the breadboard and used two jumper wires on the breadboard to connect to the device and complete the circut so that the current flows through the LED.

### 3. Build your light!

**Make a video showing off your Frankenlight.**
[video](https://youtu.be/oUdTV-QPLNc)

**Include any schematics or photos in your lab write-up.**
