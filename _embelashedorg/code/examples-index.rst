Pure Data Examples
##################
It's always easier to modify or edit than to start with a blank page, so this is a collection of Pure Data examples that provide some simple interaction and functionality.


All examples can be found in the `pure-data-bela-tutorials Github repository <https://github.com/theleadingzero/pure-data-bela-tutorials>`_, in the folder ``examples``.


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
Examples 01 through 04 are to be run on a laptop, not on Bela. However, note that you need to install the abstractions with Pure Data using the above instructins. All other examples are intended for running on Bela.

The examples roughly build on each other and become more complex as their starting number increases. Most need at least one sensor attached to Bela. All only use either the Bela scope and/or audio as the sole output, no other actuation like LEDs or motors are used. It is entirely possible to add them yourself.


Pd Basics on a Computer
=======================
These patches are to be run on a computer to introduce some basic functionality of Pd.

`1_Playing an Audio File in PD <https://github.com/theleadingzero/pure-data-bela-tutorials/tree/master/examples/1_Playing%20an%20Audio%20File%20in%20PD>`_ - Try changing the wav file being played to another file within the ``samples`` folder that you downloaded.

`2_Playing an Audio File when Above a Threshold <https://github.com/theleadingzero/pure-data-bela-tutorials/tree/master/examples/2_Playing%20an%20Audio%20File%20when%20Above%20a%20Threshold>`_ - Move the slider above a threshold to trigger audio playback. Try to adjust threshold to a higher or lower value.

`3_Add and control an Audio Effect <https://github.com/theleadingzero/pure-data-bela-tutorials/tree/master/examples/3_Add%20and%20Control%20an%20Audio%20Effect>`_ - Add an audio effect to the wav file as it is playing back. Try changing out the effects for one of the ones unconnected at the bottom of the patch.

`4_Playing Two Audio Samples and Controlling Audio Effects <https://github.com/theleadingzero/pure-data-bela-tutorials/tree/master/examples/4_Playing%20Two%20Audio%20Samples%20and%20Controlling%20Audio%20Effects>`_ - Playing and mixing two audio files at the same time. Try changing the audio files and effects.


Pd Basics on Bela
=================
`5_Use Belascope to View Interactions with Analogue Sensors <https://github.com/theleadingzero/pure-data-bela-tutorials/tree/master/examples/5_Use%20Belascope%20to%20View%20Interactions%20with%20Analogue%20Sensors>`_

`6_Playing Audio Files Based on Analogue Sensor <https://github.com/theleadingzero/pure-data-bela-tutorials/tree/master/examples/6_Playing%20Audio%20File%20Based%20on%20Analogue%20Sensor>`_

`7_Control Audio Effect Based on Analogue Sensor <https://github.com/theleadingzero/pure-data-bela-tutorials/tree/master/examples/7_Control%20Audio%20Effect%20Based%20on%20Analogue%20Sensor>`_

`8_Multiple Files Effects <https://github.com/theleadingzero/pure-data-bela-tutorials/tree/master/examples/8_Multiple_Files_Effects>`_


Audio Synthesis
===============

Microphone Input
================


Advanced Sensors
================


Communication
=============
