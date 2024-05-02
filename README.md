# Cheap FOCer 2 (v1.0)

Low-Cost(around $120 for 5 boards and components) Motor Controller based on the VESC 6
***** caution *******

This is a custom VESC for OpenFFBoard based On Cheap FOCer 2(v1.0)

.Replaced the shunt registers for low current.

.Removed the useless BMI.

.Cleaned up HALL/Encoder lines(for ABN) and COMM lines(for BiSS-C)
 for high frequency signals.(I tested COMM lines only.)

.Added OVP(over voltage protector) for PSU usage.

.Added POWER and MOTOR connector for easy plug.

.Max voltage 50V and max current is 14A.


U8 and J11 are unused, just for test purpose.

I placed JST connector for USB connection(USB1). The normal USB-C connector is J2, but it costs a little more. You can select J2/USB1(If use USB1, you need a converter from USB I/F to JST PH connector. I used cheap USB hub pcb).



A sample BOM and Position are in prodction folder.

bom.org.csv and position.org.csv are come from KiCad.

I used bom.csv and bom.lcsc.csv to order JLCPCB and LCSC respectively.

I have already had some parts, so you need adjust for your needs(also USB connector I told above).

I used position.csv for JLCPCB order because original one from Kicad has errors for some parts. You need to check the position when you order yours.



## Warning

* This board has been bench tested with MIGE motor(130st-m10010 and 90ST-M04025) and BiSS-C encoder.
 Hardware or firmware flaws could still exist and affect user operation.
* You are liable for any and all controllers built using this design. This product is intended for hobbyists and not intended for commercial use.
* Do not ask the original auther of Cheap FOCer 2 about this board. He has no responsibility about this board at all.

Licens is followd by the parent project.

***** caution *******

Front and Back:

![](source/Images/Front.PNG) ![](source/Images/Back.PNG)

Pin outs:
![](./source/Images/pinout.PNG)

## [Support Thread](https://forum.esk8.news/t/cheap-focer-2-open-source-low-cost-vesc-6-based-esc-prototyped-materials-arrived-for-test-batch/13631/1)

## Guides

* [Ordering Guide](./guides/ordering/readme.md)
* [Assembly Guide](./guides/assembly/readme.md)

## Capabilities

* 35A continuous and 70A peak with good heat sinking. These are real values. Not marketing numbers

* Up to 50.4V(12s) safe operating voltage.  For 20s version take a look at [these FOCers](https://forum.esk8.news/t/some-new-focers-84v-vesc-6-based-controllers/1513).

* Compatible with the VESC Tool for configuration

* Open source enclosure design to come

* “Living” LCSC BOM to come. BOM document to be continuously updated with compatible and stocked components from LCSC

## Advantages over VESC 6

* Significantly lower build and BOM cost

* TO-220 FETs allow for big heat sink attachment for better thermal performance

* 2-layer PCB that enables low-cost manufacturing from JLCPCB

* Designed with JLCPCB’s SMT assembly service in mind

* Added optional ON/OFF connector to turn off control circuitry when controller is not in use

* CAN connector changed to 2-pin to avoid improper connections that can cause damage

* ESD protected I/O

* Hardware open sourced

* Designed with direct meme integration

## Advantages over Cheap FOCer 1

* VESC 6 based instead of VESC 4.12

* Significantly improved layout to reduce current loops and facilitate low-noise operation of both the power stage and control circuitry for more stable operation

* Has IMU for balancing applications

* Lower profile

* Handles lower inductance motors much better

* All components on the top side except MOSFETs

* Addition of JST connectors to replace pin headers for Servo, CAN, COMM, ect.

* Addition of header for unused GPIO pins

* Micro USB

## Disadvantages (that I know of)

* Larger than original VESC 6. Cheap FOCer 2 is about 60mm x 100mm x 14mm without enclosure/heat sink

* Uses custom firmware that’s not currently supported in the VESC project. Will make firmware available on GitHub until Cheap FOCer 2 is added to and supported by the official VESC project.

## Kown Issues


## Warning

* The Cheap FOCer 2 has been bench tested but is still being field tested. Hardware or firmware flaws could still exist and affect user operation.
* You are liable for any and all controllers built using this design. This product is intended for hobbyists and not intended for commercial use.

## License

Cheap FOCer 2 is licensed under the Creative Commons Attribution-ShareAlike 4.0 International License. To view a copy of this license, visit <http://creativecommons.org/licenses/by-sa/4.0/.>
