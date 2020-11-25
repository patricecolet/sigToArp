# sigToArp
SigToArp VST FX outputing MIDI arpeggio from a chord detected in audio signal.

Unzip [sigToArp](https://github.com/patricecolet/sigToArp/raw/main/sigToArp.zip) archive into VST plugins folder

# Installation instruction 
This plugin is a PureData patch running through Camomile. 
More instruction for every platform are available here:

https://github.com/pierreguillot/Camomile/wiki/How-to-install-plugins

# How to use it

In your Daw send audio signal where chords have to be detected at the input of sigToArp,
and send MIDI outputted by sigToArp to a VST or external MIDI instrument.


Chord's fundamental must be the lowest note, and fifth must be there for more accuracy.

Chords detected:

Major, minor, sus2, sus4, diminished, add9, madd9, add11, madd11, add6, madd6, 7, m7, 7b5, augmented,
m7b5, 7M, m7M, 7M, °, 7sus2, 7sus4, 6sus2, 6sus4, 6add9, m6add9, 7add9, 7b9 m7add9, 7Madd9, m7add9,
6add11, m6add11, 7add11, m7add11, 7M#11, 13, 13b9, m13, 13b, m13b.

Set threshold between audio input attack and sustain level indicated by the white dot below the setting.
Hop is the analyzing window size, set it lower to decrease latency, and higher for more precision.
Peaks is the number of partials to detect, set it lower to decrease latency, higher to detect more chords.

Version: 1.0
Author: Patrice Colet
