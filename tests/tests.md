# THAT 1646 ests Performed.

## Single-ended output.

__Setup__:

* THAT 1646 powered from +/- 12VDC
* 5Vpp, 500 Hz sine wave applied to board input.
* Oscilloscope watching + & - outputs (tip & ring)

__Method__:

With outputs otherwise floating, verify that differential signals are each 5Vpp.

Then short ring to ground.  Tip should double in amplitude, supply current shouldn't change discernibly.  Remove short.

Short tip to ground.  Ring should double in amplitude, supply current shouldn't change discernibly. Remove short.

## Short circuit current/ output protection.

__Repeat previous setup.__

__Method__:

Short both outputs to ground.  Verify that supply current maxes at less than 70 mA.

(DUT measured 60 mA on either rail, 0 mA ground current)

## Output Clamp Verification.

__Setup__:


__Method__:

Apply 10 mSec +10V pulse to tip.  Observe voltage at tip & pin 8 -- it should be clamped to approx 6.4V.  

Continue observing, and vary positive supply rail slowly upwards from 5 VDC to 20 VDC.  When supply reaches approx 12 VDC, clamping action should disappear.

Repeat for ring & pin 1.

Repeat all above, verifying -10VDC pulses on tip and ring are clamped to lower supply rail.

## Output DC Offset

__Setup:__

* THAT 1646 powered from +/-12 VDC.
* THAT board input shorted to ground.

__Method:__

Use voltmeter to observe DC values from tip to sleeve and ring to sleeve.

(DUT measured +1 mV at tip, -1 mV at ring.)

## Distortion Levels

__Setup:__

__Method:__
