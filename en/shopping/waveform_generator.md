# Waveform generator considerations

## Introduction
Target: Function/signal/waveform generator. Ideally 0-30 MHz or better.
<br>
I think  30 MHz will suffice for me for the following reasons:
- I can upconvert signals up to 4 GHz with a mixer and an oscillator that I own, and get other for ever higher frequencies, so this bandwidth is more relevant as far as modulation or sweep is concerned rather than actual final frequency of the signal
- I can use a NanoVNA that I own to cover the rest of the test cases that I foresee I might encounter

## Glossary

- FRA = Frequency Response Analysis, used interchangeably with Bode Plot

## Models

### Siglent SDG1032X

Pros:
- Very good interface
- Very good software support
- Compatible with Siglent SDS1104X-E for FRA
