
Flanger Abstractions
####################
These abstractions are audio-rate flanger effects. Flanging is acheived when two audio signals that are delayed from one another are mixed together. The effect is sweeping sound (comb filtering) that changes based on the amount of delay between the two siganls.
Any audio signals that are passed through the abstraction will come out with the flanger effect applied. The delay between signals is controlled via the third inlet. The second inlet controls the dry/wet mix of the effect so controls the overall amount of flanging that is applied to the signal.

The abstraction has two versions, `ControlRate` and `AudioRate`. `ControlRate` abstractions are controlled by a control rate signal (like a slider object) and `B` is controlled by an audio rate signal (like an analog input).

.. image:: ./imgs/flanger.svg
  :alt: Illustration of abstraction.

Repository
**********
The abstractions can be found on `github. <https://github.com/theleadingzero/pure-data-bela-tutorials/blob/master/abstractions/echoA~.pd>`_


Inlets
******
Left inlet is for the audio signal that you want to be put through the flanger effect. 

The second inlet expects a control or audio rate signal (depending on the version of the abstraction) and controls the wet/dry balance of the effect meaning the total amount of flanging added to the signal. 

The third inlet expects a control rate signal and control the time division of the flanger effect which is the amount of time that the signal is delayed by. This is related to the overall bpm of the project (for more information on this open the abstraction). 


Outlets
*******
Left outlet is the audio signal with the flanger effect applied.
