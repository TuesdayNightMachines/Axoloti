### Axoloti AxoControl Random Sequencer
_Created by The Tuesday Night Machines and VLK in August 2017_

License: CC-BY-NC-SA

#### Files:
- _TTNM-VLK_RandomSeq_Info.jpg:_ An image explaining some of the functionality
- _TTNM-VLK_RandomSeq__v05.axp:_ This is the project file for editing in the Axoloti Patcher software
- _start.bin:_ A compiled autostart file containing the synth which you may place in the root of your Axoloti's microSD card to play with it right away

#### Description:
This is a wild MIDI sequencer I made for VLK. You will need the [Music Thing AxoControl](https://www.thonk.co.uk/shop/axoc/) for this to work as it is.

Check the _TTNM-VLK_RandomSeq_Info.jpg_ image to see how some of the features are mapped to the controls and ports of the Axoloti and AxoControl. The project file is also very well documented using comments!

There are three tracks sending randomzied CC data:
- Track A on CC2
- Track B on CC3
- Track C on CC4

You select one of those tracks with the three AxoControl push buttons.

Flicking the joystick up or clicking it creates a new eight-step random CC sequence on the selected track. This can also be done by sending a trigger pulse into the right (ring) audio input channel or by sending any CC1 value on MIDI channel 1 into the DIN port.

Flicking the joystick down will constantly randomize the CCs of the current track, so there will be no repeating pattern. Flick it down again to switch back to the normal, looping eight-step sequence mode.

The currently selected track's CC data is also sent on CC10.

A a four-step CC sequence is sent on CC5, which can be set by the four step knobs (see _TTNM-VLK_RandomSeq_Info.jpg_).

Button S1 on the Axoloti switches between internal clock or external clock, which can be both MIDI clock sent to the DIN port and analog clock pulses sent into the left (tip) audio input. Both clock signals are combined, which can get fun.

There is also a gate sequencer built-in sending note-on/off data for specific MIDI notes:
- Note numbers 30 to 34: clock divisions of internal or external clock
- Note number 35: 50/50 chance random gates

All MIDI data is sent from the DIN port on channel 1.

The audio output is also used:
- Left: Sine wave with frequencies set by the currently sleected track's CC data
- Right: Sine wave with frequncies set by the four-step sequencer's CC data
Use this for example as a non-musical FM source.

Again, check the project file. It has a lot of comments.

Enjoy and let me know if you use this project :)

_hello@nightmachines.tv_
