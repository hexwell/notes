# Power supplies considerations

## Quick theory note

There are two kinds of bench power supplies designs:

|Type|Description|
|-|-|
| Linear | Transformer to lower voltage, FBR and filtering |
| Switching | PWM with power transistor, decoupling transformer, FBR and filtering. |

## Introduction

Target:
Lab bench power supply, with these features:
- Linear design
- SCP (Short Circuit Protection)
- C.V. (Constant Voltage)
- C.C. (Constant Current)

And possibly:
- OVP (Over Voltage Protection)
- OCP (Over Current Protection)-
- OTP (Over Temperature Protection)

## Brands

- Keysight
- Keithley
- Siglent
- Korad
- Rigol
- GW Instek
- Rohde & Schwarz

## Models

### Siglent SPD3303X-E

Pros:
- Very good interface
- Very good software support
- Very low noise
- 3 CH
- OCP added in latest firmware (30/05/2021)
- Has knob

Cons:
- No OVP
- ~~No OCP~~
- No OTP
- Expensive

EEVBlog review (warning: not this exact model!):
https://www.youtube.com/watch?v=mdOauVzY9OU
<br>
MarcoReps review (warning: not this exact model!):
https://www.youtube.com/watch?v=H-BiphMqp5g

### Korad KA3005P

Pros:

- Cheap
- Has knob
- OVP
- OCP

Cons:

- 1 CH
- Noisy
- Old fashioned display (low importance)

EEVBlog Teardown:
https://www.youtube.com/watch?v=g94mpom2Ahs
