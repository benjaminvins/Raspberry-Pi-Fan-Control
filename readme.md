# Raspberry Pi Fan Control

Simple Python and shell scripts to run a fan based on CPU temperature for your Raspberry Pi. 

## The Setup

This setup uses GPIO pin 18 with cheap and reliable NPN Transistor (BC337). 

**Wiring Diagram**
![Raspberry Pi Fan Wiring Diagram](https://github.com/vollmann-ariel/Raspberry-Pi-Fan-Control/blob/master/Circuit.png)

## Running on Boot

Here's how to run this script automatically on boot:
- Modify the shell script to ensure you have the correct path _run-fan.py_.
- Make the files executable using _sudo chmod a+x run-fan.py_ and _sudo chmod a+x launcher.sh_.
- Use crontab (or another method) to execute _launcher.sh_ on boot. 

### Helpful Links
- [How to control a fan to cool the CPU of your RaspBerryPi](https://hackernoon.com/how-to-control-a-fan-to-cool-the-cpu-of-your-raspberrypi-3313b6e7f92c)
- [Five Ways To Run a Program On Your Raspberry Pi At Startup](https://www.dexterindustries.com/howto/run-a-program-on-your-raspberry-pi-at-startup/)
