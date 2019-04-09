Pure Data Abstractions
######################
These are Pure Data abstractions - blocks of code meant to be used in a larger patch. They are not necessary at all and patches can be written without them just using Pd-vanilla objects, but these are some common functions that may be useful.

All abstractions can be found in the `pure-data-bela-tutorials Github repository <https://github.com/theleadingzero/pure-data-bela-tutorials>`_, in the folder ``abstractions``.

See the supporting examples to see some of the abstractions used in a larger Pure Data patch.


Installation
************
To use these abstractions in Pure Data on your computer, add the path of the ``abstractions`` folder to Pure Data through the ``Pd -> Preferences -> Path...`` menu. You then will need to quit and restart Pure Data.

To run on a Bela board:

* `either` copy the needed abstractions to the local project folder, 
* `or` ``scp`` the abstractions folder to ``~/Bela/Projects/pd-externals/``;
* `or` in the IDE, create a new project called ``pd-externals`` and upload the ``.pd`` files in the ``abstractions`` folder to the project. If a project with that name already exists, just upload the abstractions to that project.


Input
*****
.. toctree::
   :maxdepth: 1

   abstractions/analogInput
   abstractions/digitalInput
   abstractions/audioInput



Output
******
.. toctree::
   :maxdepth: 1

   abstractions/output
   abstractions/scope


Control and Logic
*****************
.. toctree::
   :maxdepth: 1

   abstractions/constrain
   abstractions/debounce
   abstractions/map
   abstractions/reverb
   abstractions/setSensorThreshold


Audio Playback and Effects
**************************
.. toctree::
   :maxdepth: 1

   abstractions/distortion
   abstractions/echo
   abstractions/filter
   abstractions/flanger
   abstractions/mute-below-threshold
   abstractions/playAudioFile
   abstractions/recordAudioFile









