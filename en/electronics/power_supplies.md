Much of todays electronic equipment runs on DC. <br>
Having a separate DC power supply in each appliance is kind of a waste. <br>
It would be better to have only DC-DC converters in the appliances, and have one DC power supply per group of appliances. <br>

For example on a desk, there could be a single say 48 V DC power supply powering the PC, monitor, printer, and every other appliance that might be present. <br>
This could also be used to charge laptops, mobile phones and other devices (via DC-DC / USB / USB PD converters). <br>
48 V is chosen to limit the waste in cables due to high current.

This also applies to electronics labs, with oscilloscopes, signal generators and other instruments all having their individual power supply whilst being physically close. It certainly applies in a lot of other environments as well.

This concept is, however, not extensible to server racks. There, it's better to have separate power supplies for each server instead of having just a couple of big power supplies for all the rack's servers. <br>
This is because of these reasons:
- Better redundancy
- More manageable (lower electrical complexity, lower risk, etc.)
