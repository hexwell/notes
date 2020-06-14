# Measuring RF with an oscilloscope

In order to measure RF signals with an oscilloscope and calculate their power it seems like they need to be terminated in a known impedance termination.
- For low power signals (below the peak to peak voltage rating of the oscilloscope and the termination) it should be enough to use a BNC T splitter with the inputs connected to the termination, the scope and the DUT (device under test)
- For high power signals (exceeding the oscilloscope or termination rating) it is mandatory to use a sampler between the oscilloscope and the splitter an appropriate power rating termination, otherwise the oscilloscope and the termination can get damaged.

## Math

Since we are measuring a power quantity we use the ten-log-ten formula ([Wikipedia explanation](https://en.wikipedia.org/wiki/Decibel#Power_quantities)). The power measurements comes form the dB value of the ratio between the power and 1 mW (since dB are a measure of ratios). The RMS voltage is used to calculate the power because the signal is AC ([Explanation](https://www.analog.com/en/technical-articles/measurement-control-rf-power-parti.html)).

	I = U(Vrms) / Impedance
	P(W) = U(Vrms) * I
	P(dBm) = 10 log10(P(W) / 1 mW)

	Compacted:

	P(dBm) = 10 log10(U(Vrms) ^ 2 / Impedance / 1 mW)

## Note for Siglent SDS1000X-E

This scope's FFT function has built in power measurements. It works with the above formula and thus it require user input for the external impedance (through the "Vertical" menu)
