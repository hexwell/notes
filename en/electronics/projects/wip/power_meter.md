Power meter
===========

This project consists of a current transformer connected to an Arduino
via a burden resistor. The transformer is attached to one of the master
live wires in my house and the Arduino senses the voltage on the
resistor in order to calculate the current power usage.

Parts list
----------

-   ~~Arduino Pro Micro~~
-   ~~NRF24L01+PA+LNA (with RFAXIS chip)~~
-   ~~2 x 100 kΩ resistors~~
-   ~~3.3 V Regulator~~
-   ~~3 x 10 μF capacitors (ceramic, more durable)~~
-   SCT-013-000V
-   Female 3.5 mm audio jack
-   Female USB B port
-   Perf board
-   Female headers

TODO
----

-   Put grounded tin foil around NRF24 as suggested by SamyK
    (<https://youtu.be/1NBNrgTEwq0?t=760>)
-   Measure USB current consumption of final build

Design
------

### Current sensor

The current sensor needs a bias voltage in order to be in the range of
the Arduino ADC during negative cycles, so a voltage divider with two
100 kΩ resistors and a 10 μF capacitor to GND is added. The sensor
should be placed between the voltage divider and the Arduino pin. In
order to get the real value the sensor should be read RMS, as different
loads can have different current waveforms.

### Power supply

-   The NRF24L01 operates on 3.3 V and it needs a power supply. A
    regulator is used to obtain the 3.3 V and a 10 μF capacitor should
    be placed between the power lines.
-   The ADC of the Arduino requires a stable supply to make precise
    measurements. A 10 μF capacitor should be placed between the Arduino
    power rails.

### Energy efficiency

The Arduino LEDs can be desoldered to same some mA.

### Connectors

-   Female 3.5 mm audio jack input for SCT current transform
-   USB B port for power and programming (passthrough to Arduino USB)
-   SMA female connector for antenna

Questioning the whole thing
===========================

Measuring power using just a current transformer is probably not really
precise. Other possible options are using the power measurement of the
power meter directly via it\'s IR port, but that would require a lot of
work since the protocol needs to be reverse engineered. Irony of sorts,
Italy\'s energy company\'s meter is named OpenMeter.