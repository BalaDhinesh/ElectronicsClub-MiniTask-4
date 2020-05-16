# Maze Solving Robot(Troubleshooting)

__Pipeline of this project:__

Analog Reflective Sensor Array Circuit => AT89C51 microcontroller =>  L293D Motor Driver

So , If you've Built a circuit and it doesn't work , then the issue is probably with any of the Above three.

Make sure that the wire connections are made properly. Use multimeter for this to check the connectivity between the terminals.
__First, make sure all the modules have been powered up properly(power LED should light up)__


__If yes,__

Wiring part and power supply to all these modules are perfect.

__If no,__

Check which LED is not glowing up, see if it has enough power. If it has so, then the module has been sorted and we may need to buy a new one.

__IC looks hot?__

Get a new IC since it might have burnt.


## Read the datasheet carefully!
Every circuit element has limitations that should be avoided and are neatly
summarized by the datasheet. If your circuit is not working, it is possible that you have bumped
into one of these limitations and thus the device is not behaving as it should. So you should always check (preferably when
designing the schematic and selecting parts) to make sure that you are using the device correctly.

Does your device do what you think it should?

Are you using it properly?

Do you know what each
pin does and have you connected it appropriately?

Do not assume that you can leave a pin
floating if you aren’t using it.

Did you supply power to the power pins? Are you within the
expected operating regime?

Did you temporarily leave the operating regime and thus destroy the
device?




## Testing the microcontroller
First check whether sufficient power supply is given to the IC and LED light is glowing. If it is not glowing, refer the datasheet for required supply voltage and make connections accordingly. If problem still persists,
__Did you accidentally destroy the IC/Device?__

- This might happen if we give more than maximum amount of supply voltage.
- __Dont worry!__ All our components are cheap. Check in the resources section to buy a new one.

__Also, make sure to not repeat the same mistake in the replaced product!!__ 



Make sure the code has burnt properly to the microcontroller and it is not sorted.
 




## Testing the Motor Driver
__Is the motor moving?__

__If no,__ check whether the motors are rotating. If yes, there are some loose connections between motor and wheels. If no, check the code to test only the rotation of the motor. If problem still persists, consider buying a new one.

__If yes,__ check whether the wheels are moving in the direction as we require. If no, then the problem might be with the Reflective sensor that senses and gives back the wrong information.



## Testing the Reflective Sensor
Read the datasheet carefully and connect accordingly.

Make sure sufficient amount of power has been supplied to the pins and check the continuity using multimeter. If everything is fine, the issue is with the code that we have uploaded. Check the syntax or typo carefully and if it is written correctly, then change the threshold value to see any good news occurs. If problem still persists, we might consider buying a new one. Check the resourses section to get a new one!!

## Resources:

1.Microcontroller: [AT89C51](https://www.tanotis.com/products/microchip-at89c51rc-24pu-8-bit-mcu-8051-family-at89c51-series-microcontrollers-24-mhz-32-kb-512-byte-40-pins-dip?gclid=Cj0KCQjwnv71BRCOARIsAIkxW9Ffutxhf4v3fp8Y4zDpi6YADGJV1NbKa32D-whK-9y_JijnM0JstEIaApQlEALw_wcB)

2.Motor Driver: [L293D](https://robu.in/product/l293d-motor-driver-module/?gclid=Cj0KCQjwnv71BRCOARIsAIkxW9EoYF7OFAE4hsqs8PjDzywUW9RfuoxLQ7uP0Y4wb7D9r7cbll7G4TAaAvM-EALw_wcB)

3.Reflective Sensor: [RLS-08](https://robu.in/product/smartelex-rls-08-analog-digital-line-sensor-array/?gclid=Cj0KCQjwnv71BRCOARIsAIkxW9EVLeEhqiyeVCzqHhnChUcinQUSzdu4r99Kg8aHQXvWzn9UlngtjbsaAnZDEALw_wcB)
