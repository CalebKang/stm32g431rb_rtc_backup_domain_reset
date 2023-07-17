# How to reset RTC domain control register and Backup registers

When VBAT has 150mV ~ 1,550mV range during Power on reset, backup domain would not reset correctly.

It causes the RTC to do unintended behavior. For example, PA2 set as ADC can operate as a low speed clock output.
This example can be very useful if your application dosen't connect a battery to VBAT.

This example resets the Backup domain and disables the LSCOEN bit.
