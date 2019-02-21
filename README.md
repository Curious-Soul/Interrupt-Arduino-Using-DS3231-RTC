# Interrupt-Arduino-Using-DS3231-RTC

The RTC DS 3231 (which works on the I2C protocol) is used to wake up Arduino UNO board from sleep using an interrupt. 
When the alarm occurs an interrupt is being triggered on the INT pin of the RTC and this interrupt wakes up the Arduino from sleep.

The Arduino Uno is given an interrupt using the RTC alarm interrupt. Here we have used an RTC named as DS3231 and it works on I@C protocol.
It requires a VCC of about 2.3-5.5V and the SCL , SDA (RTC) are connected to the SCL, SDA (Arduino Uno) respectively. 
Whereas, the !(INT/SQW) output is connected to the pin 2 of the Arduino. It is an active low pin and we get an interrupt on this pin 
whenever the time on the RTC and the time keeping registers of the RTC match.
There is a Vbat pin where we can connect our external battery to power the RTC module.

<p align="center">
<img width="300" height="200" src="https://github.com/Curious-Soul/Interrupt-Arduino-Using-DS3231-RTC/blob/master/DS3231-Chip.PNG">
</p>

<br>

<p align="center">
<img width="600" height="450" src="https://github.com/Curious-Soul/Interrupt-Arduino-Using-DS3231-RTC/blob/master/DS3231.PNG">
</p>

<br>

<p align="center">
<img width="800" height="450" src="https://github.com/Curious-Soul/Interrupt-Arduino-Using-DS3231-RTC/blob/master/Working.PNG">
</p>

Video: https://www.youtube.com/watch?v=8S07tx7tc18
