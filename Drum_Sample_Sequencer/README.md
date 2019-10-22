### Axoloti Drum Sample Sequencer
_Created by The Tuesday Night Machines in September 2018_

License: CC-BY-NC-SA

#### Files:
- _TTNM_DrumSeq_v07.axp:_ This is the project file for editing in the Axoloti Patcher software
- _start.bin:_ A compiled autostart file containing the synth which you may place in the root of your Axoloti's microSD card to play with it right away
- _TTNM_DrumSeq_MIDImix_Mapping.midimix:_ The correct mapping filae for your Akai Midimix controller
- _TTNM_DrumSeq_MIDImix_Mapping.png:_ A screenshot of the Akai Midimix controller mapping
- _TTNM_DrumSeq_MIDImix_Labels.jpg:_ A screenshot of the Akai Midimix with labels for the knobs and buttons

#### Description:
This is a drum sample sequencer made for live performances. It requires an [Akai Midimix](https://www.akaipro.com/midimix) USB-MIDI controller to work as it is.

There are six voices (samples) which can each be sequenced individually. The main sequencer is not a linear step sequencer, but one based on clock divisions of an incoming MIDI clock signal - which is required! The incoming 24ppq MIDI clock is divided by 3 before it is further processed by the user, resulting in eight pulses per quarter note.

For each voice you can set two clock division factors to trigger the voice's sample. For example every fourth pulse and every tenth pulse. This trigger pattern can then also be shifted in time, for example four pulses behind the clock, potentially resulting in a completely different feeling of the overall rhythm. You can easily edit the clock division factors in Tables 01 and 02.

In addition to this clock division sequencer, there is also a probability trigger generator per voice. You simply set a probability between 0% and 100% if a sample trigger should happen on the current pulse and a random number generator will then determine the result (trigger or no trigger). 

Triggers of both sequencers are combined by OR logic and each sequencer has its own MUTE button per voice.

The result can quickly become very crazy and off-beat of course, so there is a "quantized mute" master fader, which lets you adjust wether all sample triggers are sounding or only those on even pulses. You can select between sample triggers on every pulse or every 2nd, 4th or 8th pulse (i.e. every quarter). You can edit this too in the masterfader table.

Additionally you can select one of four different samples per voice with dedicated knobs and there is also two master effects (LPF and distortion, also easy to change if you want to). Samples are in .raw format ... I think 44.1kHz, 16bit, mono ... check the Axoloti documentation if that shouldn't work. I also uploaded samples here, which you can use for testing.

I posted a short video demo of an earlier version of this project on Instagram:

[https://www.instagram.com/p/BnI6q0fgm8S/](https://www.instagram.com/p/BnI6q0fgm8S/)

In this early version the Axoloti didn't play samples by itself, but sequenced the AudioThingies DoubleDrummer drum synth via MIDI. This version does not exist like this anymore for me to share, but you can easily add MIDI sequencing yourself. Scroll down in the Axoloti Patcher until you see the sample player modules at the bottom and simply exchange them for MIDI Out Note modules.

Enjoy and let me know if you use this project :)

_hello@nightmachines.tv_


