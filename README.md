# BeachSafety
Virginia Beach Makerbot competition  2018


## Prototype Parts List

Note Prices may be considerably lower if ordered via the slow boat.


| Item Name       | Quantity   | Price  | Total|
|-----------------|:----------:|-------:|-----:|
| Arduino Nano    | 2          |  3.50  |  7.00|
| LED Matrix      | 1          |  8.00  |  8.00|
| NEO-6M GPS      | 2          | 15.00  | 30.00|
| NRF905 Wireless | 2          |  9.00  | 18.00|
| MPU9250 Compass | 1          |  8.50  |  8.50|
| Batteries       | 2          |  5.00  | 10.00|
| Wires           | 30         |   .05  |  1.50|


## Resources

Compass Library 
https://github.com/asukiaaa/MPU9250_asukiaaa

GPS Library
https://github.com/SlashDevin/NeoGPS

LED Matrix Library
https://github.com/bartoszbielawski/LEDMatrixDriver
or
https://github.com/t3chguy/arudino-maxmatrix-library/tree/master/MaxMatrix

Wireless Radio Library
http://www.airspayce.com/mikem/arduino/RadioHead/classRH__NRF905.html

http://www.electrodragon.com/w/NRF905

https://github.com/athombv/homey-arduino-nrf905/blob/master/doc/arduino_nRF905_wiring.png

http://www.zonnepanelen.wouterlood.com/arduino-bare-basics/arduino-passing-temperature-readings-to-a-neighbor-arduino-three-ways-of-serial-communication/


### Wireless
The inexpensive 433mhz module did not have enough range to be effective, we are upgrading to the NRF905 Wireless Radio Transceiver.

### GPS

We do not need cellular connectivity so to reduce cost, physical size, and battery usage we are now using the NEO 6-M GPS module.


## Technical Challenge

Goal: Calculate Distance between two wireless GPS units.

Steps

Person 1's device (Sending Unit)

1. Read GPS
2. Send coordinates over wireless

Persons 2's device (Receiveing Unit)

1. Find North on our compass so we have a bearing to reference against
2. Recieve GPS coordinates over wireless
3. Read local GPS coordinates
4. Calculate Distance
5. Calculate Direction (Bearing)
5. Dispaly Visual Representation of distance and direction by making LED Lights light up.

We might need an accelerometer/gyroscope/compass to help with our direction visualization


### Display 

We need a simple durable cost effective display. 

LED's are durable, inexpensive, and easy to wire up.  
Having a screen, like a cell phone, may allow for more features, but screens are more difficult to program, they cost more, and are not as durable.

![Ghostbusters](https://github.com/ericrohlfs/beachsafety/raw/master/Ghostbusters2.jpg)


### Sketches

