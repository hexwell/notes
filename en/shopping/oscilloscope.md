# Oscilloscopes considerations

Oscilloscope rundown summary

## Introduction

Target: small bench-top analog-only digital oscilloscope

## Glossary

- FRA = Frequency Response Analysis, used interchangeably with Bode Plot

## Brands

The offerings from the following brands have been considered:

- Siglent
- Rigol
- Keysight
- Tektronix
- Rohde & Schwarz
- Teledyne LeCroy

**11/20 update:**

I discovered Yokogawa as a brand of oscilloscopes. I do not integrate this rundown
with them as they are very very expensive.

## Siglent

Siglent's design and mission (with their low cost entry hardware) are good.

Series offering target oscilloscopes:

- SDS1000DL (too low bandwidth)
- SDS1000CML+ (not interested in deep memory)
- SDS1000CFL (the SDS1000X-E are better designed and support heatmap view)
- SDS1000X-E
- SDS1000X+ (a bit expensive, old button layout, not really interested in the generator without FRA)
- SDS2000X-E (a bit expensive, not interested in more sample rate and memory)
- SDS1000X-U (cheaper variant of SDS1000X-E without logic analizer capabilities and fancy features)

Models considered:

### SDS1102X-E

Cons:
- 2 channels only (this weight a lot)
- No FRA capability (this weight a lot)
- Old button layout (both bottom and left panels) (this weights little)

Pros: (all of these weight little)
- Aligned connectors
- Calibration port design
- Calibration port naming
- Clean chin

### SDS1104X-E

Cons:
- Unaligned connectors (this weights little)

Pros:
- Features for price
- FRA capability
- 4 color button LEDs (this weights little)

Notes:
- It makes total sense for this model to have the calibration port like it does. It would be difficult to move it where the SDS1102X-E has it without removing channels. No clear view on where it would be more convenient also. The design of the calibration port is appropriate with this placement.
- Elongating the chin to match the top one is not possible as long as the calibration port is there
- The back cover has a recess on the sides compared to the SDS1102X-E, probably for handling

### SDS1204X-E

Same hardware as SDS1104X-E, that can be unlocked to 200 MHz bandwidth, so no reason to consider this.

## Rigol

Series offering target oscilloscopes:

- 1000
- 1000Z
- 2000
- 4000

Design and build quality (even on the high end) are unsatisfactory. The oscilloscope needs to be decent looking and sturdy built. Also it seems like they have a lot of bugs in their firmware ([link](https://www.youtube.com/watch?v=UDGsZcAWgL8)). Rigol out.

## Keysight

The company does great stuff in the hardware, software and content compartment, as well as collaborating with the community and focusing a lot on learning. Their firmwares are an example, as they include a lot of explanations and they name things in a way that is more aligned with my views on naming (like the Bode Plot function named "Frequency Response Analysis")

Series offering target oscilloscopes:

- InfiniiVision 1000X

Cons:
- Very expensive
- Round shape design (this weights little)

Pros:
- High sample rate (2Msps)
- Wave generator option on all models
- Rubberized knobs (this weights little)
- Buttons disposition, LEDs colors, and symbols use in the interface (this weights little)
- Nice front end - [teardown](https://youtu.be/9KcOQsVxtoU?t=1274)

## Tektronix

Their MDO are very nice, considering a future spectrum analyzer purchase (although out of target now). Their interface is very clean

Series offering target oscilloscopes:

- TBS1000B
- TBS2000B

To get what other offer with Tek the prices are excessively too high.

## Rohde & Schwarz

Series offering target oscilloscopes:

- RTC1000
- RTB2000

To get what other offer with R&S the prices are excessively too high.

## Teledyne LeCroy

The low ends products of LeCroy are rebranded Siglents

## Conclusions

- The Siglent SDS1104X-E is the oscilloscope of choice. It has a great price for the features.
- A 2 channels Keysight InfiniiVision 1000X oscilloscope might be considered in the future, for its ability to do FRA with the internal generator and for Keysight firmware (The DSOX1102G might suffice since all the internal wave generator cap at 20 MHz)
- A Tektronix MDO might be considered in the spectrum analyzer rundown
