# Gate Delay


The circuit here is based on the [Yusynth Gate Delay](https://yusynth.net/Modular/EN/GATEDELAY/index.html) with minor tweaks to make it more Eurorack friendly. The changes I've made are thus:
* Selected resistors appropriate for +/-12V rails,
* Added polarity protection so that a backward power header doesn't fry anything (twin series schotty diodes: BAT54SL),
* Full surface mount design,
* Preseve gate duration in the delay.

The maximum delay is approximately 250ms, although by changing some resistor or capacitor values you may be able to extend that by quite a degree. I kept the delay to a moderate value to prevent distortion in delay duration. The main enhancement here over the original circuit is that the duration of the output gate mimicks the duration of the input gate. The output duration can be slightly longer than the input when the delay is set to high values.

The Yusynth page is a treasure trove of information about this circuit that I am too amateur to claim as my own; please read that outstanding page before using this circuit. The page provides many details and other implementations of this circuit that you may find suitable.

The KiCAD project here uses the library/footprints [found in my companion repo](https://github.com/thismatters/EurorackKiCAD).


## Width

12hp on an Intellijel 1U rack.

## Inputs

Jack for Gate

Potentiometer for delay duration

## Outputs

LED to indicate gate output

Jacks:
- Gate
- Slew (Logarithmic)

## Vendors

There are part numbers in the [BOM](gate-delay.csv) for many of the parts (not for basic passives though) at the following vendors:

* [Mouser](https://www.mouser.com): Needs no introduction. Get your ICs from here (or [digikey](https://www.digikey.com)).
* [Tayda Electronics](https://www.taydaelectronics.com/): Good supplier for passive components; audio jacks, and potentiometers. Their audio jacks are slightly smaller than the thonkiconn from thonk.
* [Love My Switches](https://lovemyswitches.com/): Has [really good knobs](https://lovemyswitches.com/anodized-aluminum-knob-the-lo-fi-1-4-smooth-shaft-12-5mm-od/) to go on those potentiometers!
* [OSHPark](https://oshpark.com/): Fast and (relatively) cheap PCB manufacturer. Prototype run pending.
