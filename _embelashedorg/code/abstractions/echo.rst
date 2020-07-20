
Echo Abstractions
#################
These abstractions are audio-rate echo effects. Any audio signals that are passed through the abstraction will come out delayed by an amount that is controlled via the third inlet. The second inlet controls the dry/wet mix of the effect so controls the overall amount of echo that is applied to the signal.

The abstraction has two versions, `ControlRate` and `AudioRate`. `ControlRate` abstractions are controlled by a control rate signal (like a slider object) and `B` is controlled by an audio rate signal (like an analog input).

.. image:: ./imgs/echo.svg
  :alt: Illustration of abstraction.


Repository
**********
The abstractions can be found on `github. <https://github.com/theleadingzero/pure-data-bela-tutorials/blob/master/abstractions/echoA~.pd>`_


Inlets
******
Left inlet is for the audio signal that you want to be put through the echo effect. 

The second inlet expects a control or audio rate signal (depending on the version of the abstraction) and controls the wet/dry balance of the effect meaning the total amount of echo added to the signal. 

The third inlet expects a control rate signal and control the time division of the echo effect which is the amount of time that the signal is delayed by. This is related to the overall bpm of the project (for more information on this open the abstraction). 


Outlets
*******
Left outlet is the audio signal with the echo effect applied.
