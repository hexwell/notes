# USB C PD All The Things!

Using cheap USB PD sinks from AliExpress it is possible to add USB C to a lot of appliances.

## Design guidelines

### Device types

The first thing to understand about the device we are trying to modify is it's original intended use. Objects fall into one of the following categories. For each category I will provide design guidelines tailored to it.

- HH - Battery powered hand held devices. Examples: Baofeng, Multimeter, Labeler, Component tester
- PS - Power supplied desk devices. Examples: Baofeng charger

### HH Devices

This kind of devices must preserve their untethered, battery powered feature. It is also desirable for the charger to be integrated with the device, as that would be one less device to carry, which is always better.

These devices might come in two varieties:
- Using standard disposable batteries. Examples: Multimeter, Labler, Component tester
- Using custom rechargeable batteries and a custom charger. Examples: Baofeng

#### First case

The first statement is particularly of interest for this variety, as they cannot have the batteries replaced by USB PD, even tho that though might seem appeling at a first glance. What would instead be good is for them to a battery and a recharegeable one, and so by convenient means, like USB. So these device, contrary to what one might think upon first observation, require not only one but two modification:
1) Convert the disposable battery to a rechargeable one
2) Add USB charger, possibly integrated in the device

- For devices using 9V batteries, usb chargeable ones can be easily purchased on the internet solving the problem completely with an off the shelf solution.
- For devices using stick battery further investigation is needed. (Usb chargeable stick batteries are available but charging them would be unconvenient as for some devices up to 6 usb ports and cables would be needed)
- Devices that accept DC inputs double as PS devices. It may or may not be desirable to still do the battery hack

#### Second case

These devices need, depending on the level of effort one's willing to put into this, one of two things:
- A complete battery replacement by another one featuring an integrated usb charger. The DC input option from PS Devices might apply here as well
- A modification of the charger to add USB PD as a power supply, this would be a PS device

### PS Devices

These devices just need to be modified to be able to have their power supplied by USB PD, as well as from their own wall adaptor.

#### DC input

These devices might benefit from a direct DC input as they are more likely to be used in raw environments like labs, camps or vehicles where direct DC power mmight be available.
