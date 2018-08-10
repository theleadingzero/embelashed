# **Vibration Sensor**
## **What does the sensor do?**
The piezo can sense vibration, such as knocking or sound waves. It measures the vibration by converting it into electrical voltage. In some cases, this sensor can also be used as a small audio transducer.

## **How do you embed the sensor onto paper?**
You will need:
- paper template
- piezo sensor   
- 2 strips of copper tape   
- wire cutters
- 1 mega ohm resistor (aka 1mΩ)  
- soldering equipment

<img src="./imgs/Piezo_small.png" width="600" />

**Suggested sequence for making**
- Cut the copper tape in half lengthwise with a pair of scissors
<img src="./imgs/cut_24_0-18.gif"/>

- Stick the copper tape to the paper template
<img src="./imgs/piezo-tape_18_0-18.gif"/>

- Cut the piezo insulation to expose the wire using a pair of wire cutters
<img src="./imgs/piezo-wire_18_0-18.gif"/>

- Solder components and fold to fit to the breakout board connector. Need help with soldering? Feel free to ask someone if you are at a workshop, or adafruit [have a good soldering guide](https://learn.adafruit.com/adafruit-guide-excellent-soldering/making-a-good-solder-joint). Always wear protective glasses.
<img src="./imgs/piezo-solder_18_0-18.gif"/>

> **Handy hint!**  
>There are two wires connected with piezo, the black wire should be connected to the "ground", the red one should be connected to the "input".
>Make folds in the copper tape to keep a continuous connection.

<img src="./imgs/folding.png" width="400" />

>**Some technical info**
>We are using a "pull-down" resistor so that we can know the state of the sensor signal. Find out more about this [here](http://cnmat.berkeley.edu/recipe/how_and_why_add_pull_and_pull_down_resistors_microcontroller_i_o_).

## **What kind of interactions or movement can you sense?**
**1. Environment**  
Piezos can sense when they are hit against objects.  
<img src="./imgs/hit.gif" width="300" />

**2. Movement**  
Knocking, shaking, flipping, tapping…and more!  
<img src="./imgs/knock.gif" width="300" />

> **Handy hint!**  
>If you feel the piezo is too sensitive to realise your intended interaction, replace the 1M ohm resistor with a lower resistor value such as 100K ohm resistor, the less resistance used in the circuit, the less sensitive your piezo will be.
