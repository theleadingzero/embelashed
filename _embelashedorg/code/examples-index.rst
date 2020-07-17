Pure Data Examples
##################
It's always easier to modify or edit than to start with a blank page, so this is a collection of Pure Data (Pd) examples that provide some simple interaction and functionality.

All examples can be found in the `pure-data-bela-tutorials Github repository <https://github.com/theleadingzero/pure-data-bela-tutorials>`_, in the folder ``examples``.

Additional guidance on how to code using Pure Data on Bela is available in the `Bela documentation <https://learn.bela.io/using-bela/languages/pure-data/>`_.


Installation
************
Download the `pure-data-bela-tutorials Github repository <https://github.com/theleadingzero/pure-data-bela-tutorials>`_ to any desired location on your computer.

To run the example patches in Pure Data on your computer, add the path of the ``abstractions`` folder to Pure Data through the ``Pd -> Preferences -> Path...`` menu. You then will need to quit restart Pure Data.

To run on a Bela board:

* `either` copy the needed abstractions in the downloaded ``abstractions`` to the local project folder, 
* `or` ``scp`` the abstractions folder to ``~/Bela/Projects/pd-externals/``;
* `or` in the IDE, create a new project called ``pd-externals`` and upload the ``.pd`` files in the ``abstractions`` folder to the project. If a project with that name already exists, just upload the abstractions to that project.

Then create a new Pd project in the Bela IDE and upload the contents of the example project folder - this always includes a ``_main.pd`` and may includes some additional files.


Overview of Examples
********************
Examples 01 through 04 are to be run on a laptop, not on a Bela board. However, note that you need to install the abstractions with Pure Data using the above instructions. All other examples are intended for running on Bela and will not work on a laptop.

The examples roughly build on each other and become more complex as their starting number increases. Most need at least one sensor attached to Bela. All only use either the Bela scope and/or audio as the sole output, no other actuation such as LEDs or motors are used, though it is entirely possible to add them yourself.


Pd Basics on a Computer
=======================
These patches are to be run on a computer before adding a Bela to introduce some basic functionality of Pd.

`1_Playing an Audio File in PD <https://github.com/theleadingzero/pure-data-bela-tutorials/tree/master/examples/01_Playing%20an%20Audio%20File%20in%20PD>`_ 

*Summary:* Plays a wav file. The volume and playback speed (pitch) can be controlled.

*Sensor Inputs:* None, controlled using the mouse.

*Learning Challenge:* Change the wav file being played to another file within the ``samples`` folder that you downloaded.

`2_Playing an Audio File when Above a Threshold <https://github.com/theleadingzero/pure-data-bela-tutorials/tree/master/examples/02_Playing%20an%20Audio%20File%20when%20Above%20a%20Threshold>`_ 

*Summary:* Plays a wav file when the slider is above the threshold set in the message. Move the slider above a threshold to trigger audio playback.

*Sensor Inputs:* None, controlled using the mouse. 

*Learning Challenge:*  Adjust threshold to a higher or lower value.

`3_Add and control an Audio Effect <https://github.com/theleadingzero/pure-data-bela-tutorials/tree/master/examples/03_Add%20and%20Control%20an%20Audio%20Effect>`_ 

*Summary:* Adds an audio effect to the wav file as it is playing back. 

*Sensor Inputs:* None, controlled using the mouse.

*Learning Challenge:* Try changing out the effects for one of the ones unconnected at the bottom of the patch.

`4_Playing Two Audio Samples and Controlling Audio Effects <https://github.com/theleadingzero/pure-data-bela-tutorials/tree/master/examples/04_Playing%20Two%20Audio%20Samples%20and%20Controlling%20Audio%20Effects>`_ 

*Summary:* Plays and mixes two audio files at the same time. 

*Sensor Inputs:* None, controlled using the mouse.

*Learning Challenge:* Try changing the audio files that are triggered. Look are what audio files are already included in the ``abstractions`` folder. Change the effects being applied - there are additional, unused effects at the bottom of the patch.

Pd Basics on Bela
=================
`5_Use Belascope to View Interactions with Analogue Sensors <https://github.com/theleadingzero/pure-data-bela-tutorials/tree/master/examples/05_Use%20Belascope%20to%20View%20Interactions%20with%20Analogue%20Sensors>`_

*Summary:* Display the values of two input sensors in real-time as you interact with them. To see how to open the oscilloscope, refer to from around `0:58 of this video <https://www.youtube.com/watch?v=AoP7rPAMpvk&t=58s>`_ from the Bela team. Note that this is an older video showing an older version of the IDE, but the general steps are the same. 

*Sensor Inputs:* Two analogue sensors connected to S0 and S1 on the Bela Paper Capelet or Analogue 0 and 1 directly into the Bela board.

*Learning Challenge:* Figure out which coloured line corresponds to each sensor channel.

`6_Playing Audio Files Based on Analogue Sensor <https://github.com/theleadingzero/pure-data-bela-tutorials/tree/master/examples/06_Playing%20Audio%20File%20Based%20on%20Analogue%20Sensor>`_

*Summary:* Start playing an audio file when a sensor goes above a threshold value. Plays up to two different audio files, each associated with a different sensor.

*Sensor Inputs:* Two analogue sensors connected to S0 and S1 on the Bela Paper Capelet or Analogue 0 and 1 directly into the Bela board.

*Learning Challenge:* Change the threshold values to make the sensors more sensitive so that they trigger the audio playback easier.

`7_Control Audio Effect Based on Analogue Sensor <https://github.com/theleadingzero/pure-data-bela-tutorials/tree/master/examples/07_Control%20Audio%20Effect%20Based%20on%20Analogue%20Sensor>`_

*Summary:* Trigger the playback of an audio when the sensor on the first channel goes above the threshold and then at the same time control how much of an audio effect is applied to the output via a second analogue sensor.

*Sensor Inputs:* Two analogue sensors connected to S0 and S1 on the Bela Paper Capelet or Analogue 0 and 1 directly into the Bela board.

*Learning Challenge:* Customise the patch - change the audio file, audio effect, and threshold sensitivity.

`8_Multiple Files Effects <https://github.com/theleadingzero/pure-data-bela-tutorials/tree/master/examples/08_Multiple_Files_Effects>`_

*Summary:* Like the previous example, except four sensors to trigger four different audio files and then another four sensors to independently control audio effects on each file. This patch is to primarily show how to mix multiple audio file outputs together.

*Sensor Inputs:* Note, the Bela Paper Capelet cannot support all 8 sensors at the same time. You will need to change the sensor input channels to match your setup. This patch can be used unchanged with the Bela directly, eight analogue sensors connected Analogue 0 through 7.

*Learning Challenge:* Delete two of the audio file series of patches so that the patch works with only 4 sensors. Take care with how the audio is being mixed to its final output.


Microphone Input
================
`9_Mic Test <https://github.com/theleadingzero/pure-data-bela-tutorials/tree/master/examples/09_Mic%20Test>`_

*Summary:* Live microphone input with an audio delay effect controlled by two sensors which control the delay time and feedback.

*Sensor Inputs:* Mic on left audio input and two analogue sensors connected to S0 and S1 on the Bela Paper Capelet or Analogue 0 and 1 directly into the Bela board.


`10_Live Sampler <https://github.com/theleadingzero/pure-data-bela-tutorials/blob/master/examples/10_Live%20Sampler>`_

*Summary:* Records an audio signal, stores it, and then triggers its playback. An additional sensor changes the playback speed (pitch).

*Sensor Inputs:* Mic on left audio input and the following sensors:

    * Digital 0 starts and stops the recording

    * Analogue 1 starts and stop playback

    * Analogue 2 controls the playback speed

    * Analogue 3 controls amount of echo effect applied



Audio Synthesis
===============
`11_Karplus-Strong <https://github.com/theleadingzero/pure-data-bela-tutorials/tree/master/examples/11_Karplus-Strong>`_

*Summary:* String synthesiser which doesn't use any samples, but generates the sound mathematically.

*Sensor Inputs:* Sensor on Analogue 1 which will change values very quickly, like a piezo. Sensor on Analogue 2 changes the length of the virtual string. Sensor on Analogue 3 changes the tone of the string. 


`12_Rubber Duckie <https://github.com/theleadingzero/pure-data-bela-tutorials/tree/master/examples/12_Rubber%20Duckie>`_

*Summary:* Physical model of the sound of air being squeezed out of an object like a rubber duckie. Does not use any sound samples, but generates the audio mathematically.

*Sensor Inputs:* One sensor on Analogue 1 which will change values very quickly, like a piezo.


`13_FM-Synthesis <https://github.com/theleadingzero/pure-data-bela-tutorials/tree/master/examples/13_FM-synthesis>`_

*Summary:* FM synthesiser controlled by three analogue sensors.

*Sensor Inputs:* Three analogue sensors on the first three analogue inputs.



