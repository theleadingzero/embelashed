# **Pressure sensor**
## **What does the sensor do?**
The black plastic sheet is pressure-sensitive conductive sheet, also known as Velostat. It can detect force pressed on its surface. The conductivity changes when the pressure on it changes. It is flexible and can be used in paper circuitry.

## **How do you embed the sensor onto paper?**
You'll need:

- Paper template
- Square of Velostat that fits to the paper templates
- 3 strips of copper tape
- 2 squares of copper pad
- Masking tape
- 1k ohm resistor
- Soldering equipment

<img src="./imgs/velo1_small2.png" width="600" />

<img src="./imgs/velo2_small.png" width="600" />    

**Suggested sequence for making**
- Cut the copper tape in half lengthwise with a pair of scissors
<img src="./imgs/cut_24_0-18.gif"/>

- Stick the copper tape to the paper template
<img src="./imgs/velo-tape_18_0-18.gif"/>

- Stick down the copper pads so that they overlap the copper tape
<img src="./imgs/velo-pad_18_0-18.gif"/>

- Solder the resistor and the copper pad to the tape. Need help with soldering? Feel free to ask someone if you are at a workshop, or adafruit [have a good soldering guide](https://learn.adafruit.com/adafruit-guide-excellent-soldering/making-a-good-solder-joint). Always wear protective glasses.
<img src="./imgs/velo-solder_18_0-18.gif"/>

- Cut the velostat to be 1-2mm larger than the copper and sandwich it in between the two copper pads. You can use a small piece of tape to secure it.
<img src="./imgs/velo-velo_18_0-18.gif"/>

>**Handy hint!**
>Pasting the masking tape around the sensor is not only fixing Velostat, but also secure the circuitry from short circuits. Attaching the two parts of circuit using the non-conductive tape will be more convenient for you to embed the sensor to your prototype.

>**Some technical info**
>We are using a "pull-down" resistor so that we can know the state of the sensor signal. Find out more about this [here](http://cnmat.berkeley.edu/recipe/how_and_why_add_pull_and_pull_down_resistors_microcontroller_i_o_).

## **What kind of interactions or movement can you sense?**
### 1. Movement  
You can sense pressing or pushing.  
<img src="./imgs/pressure.gif" width="300" />

### 2. Cooperation
It is a pressure sensor so can sense contact between people.  
<img src="./imgs/TOUCH.gif" width="300" />

### 3. Environment  
You could sense leaning or bumping against objects, sitting on a chair or all kinds of things!
