# Digital Clock with Alarm

This simulink model represents a logic gate implementation of a simple digital clock with alarm feature. Device has 6-digit display (hours, minutes and seconds; the time range is from 00:00:00 to 23:59:59) shared between the clock and alarm. There is a dedicated lamp showing a state of the alarm (off, armed or active).


# Configuration and usage

To switch between the clock subsystem and alarm subsystem, use the *Clock/Alarm* switch.

To set time, hold the *SetTime* button or flip the *SetTime* switch to the top position (this is dependent on physical implementation of the *SetTime* input) and press the *Hour*, *Minute* or *Second* buttons. To reset the time to zero, press the *Reset* button. Time will be set/reset for the clock subsystem or alarm subsystem, depending on the position of the *Clock/Alarm* switch. The rest of the system will stay unaffected.

After the time is set, release the *SetTime* button or flip the *SetTime* switch to the bottom position.

Once time is set, alarm can be switched to standby mode by flipping the *Arm/Disarm* switch to top position (lamp blinks). Then the system waits until clock time equals to alarm time. When times match, the alarm is activated (lamp is on). To deactive it, set the *Arm/Disarm* switch to bottom position (lamp is off).

*AlarmOutput* can be used as a trigger signal for an external device (switch on radio, detonate bomb, ...).


# Model Overview
For more details please see [Clock.pdf](./Docs/Clock.pdf).
![Clock (top view)](./Docs/Clock_TopView.png "Digital Clock with Alarm (top view)")




