
Reverb Abstractions
###################
This abstraction is an audio-rate reverb effect. This effect adds reverb to an audio signal.

The abstraction has two versions, `ControlRate` and `AudioRate`. `ControlRate` abstractions are controlled by a control rate signal (like a slider object) and `B` is controlled by an audio rate signal (like an analog input).

.. image:: ./imgs/reverb.svg
  :alt: Illustration of abstraction.

Repository
**********
The abstractions can be found on `github. <https://github.com/theleadingzero/pure-data-bela-tutorials/blob/master/abstractions/reverbA~.pd>`_


Inlets
******
Left inlet expects the audio signal that you want to be put through the reverb effect. 

The second inlet expects a control or audio rate signal (depending on the abstraction) and controls the wet/dry balance of the effect.


Outlets
*******
Left outlet is the audio signal with the reverb effect applied.
