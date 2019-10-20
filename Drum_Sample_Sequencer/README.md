### Axoloti Drum Sample Sequencer
_Created by The Tuesday Night Machines in September 2018_

License: CC-BY-NC-SA

#### Files:
- _TTNM_DrumSeq_v07.axp:_ This is the project file for editing in the Axoloti Patcher software
- _start.bin:_ A compiled autostart file containing the synth which you may place in the root of your Axoloti's microSD card to play with it right away
- _TTNM_DrumSeq_MIDImix_Mapping.midimix:_ The correct mapping filae for your Akai Midimix controller
- _TTNM_DrumSeq_MIDImix_Mapping.png:_ A screenshot of the Akai Midimix controller mapping

#### Description:
This is a drum sample sequencer made for live performances. It requires an [Akai Midimix](https://www.akaipro.com/midimix) USB-MIDI controller to work as it is.

There are six voices (samples) which can each be sequenced individually. The sequencer is not a linear step sequencer, but one based on clock divisions. For each voice you can set two clock division factors to trigger the voice's sample. For example every fourth beat and every tenth beat. This trigger pattern can then also be shifted in time, for example four beats behind the clock, potentially resulting in a completely different feeling of the overall rhythm.

In addition to this clock division sequencer, there is also a probability trigger generator per voice. You simply set a probability between 0% and 100% if a sample trigger should happen on the current beat and a random number generator will then determine the result (trigger or no trigger). 

Triggers of both sequencers are combined by OR logic and each sequecner has its own MUTE button per voice.

The result can quickly become very crazy and off-beat of course, so there is a "quantized mute" master fader, which lets you adjust wether all sample triggers are sounding or only those on even beats. You can select between every trigger, or every 2nd, 4th or 8th trigger.

Additionally you can select one of four different samples per voice with dedicated knobs and there is also two master effects (LPF and distortion).

Enjoy and let me know if you use this project :)

_hello@nightmachines.tv_
