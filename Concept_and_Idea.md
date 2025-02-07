# Idea


millis() function is used to control the timing of the traffic light cycle rather than delay function as it will help us to perform other tasks simultaneously, if required, without delay.

The ON time for all the three lights can be changed as per requirement by changing the respective values in the code.

When the PUSH button is pressed due to the if condition the system will immediately turn red. A delay time of 3000ms is given after which the normal cycle will perform again.

while loop has been used to implement the logic with millis() function. 


# Concept


Arduino is a micro-controller that performs a single set of task only at a time.

It has 6 Analog pins and 13 Digital pins. To control the glowing of bulb requires only ON and OFF conditions. That's why all the three bulbs are connected to digital pins for output.

Similarly a push button has two states only i.e ON and OFF and hence connected to digital pin.

