# Cheap FOCer 2 (v1.0)

Low-Cost(around $120 for 5 boards and components) Motor Controller based on the VESC 6

***** caution *******

This is a custom VESC for OpenFFBoard based On Cheap FOCer 2(v1.0)

* Replaced the shunt registers for low current.

* Removed the useless BMI.

* Cleaned up HALL/Encoder lines(for ABN) and COMM lines(for BiSS-C)
  for high frequency signals.(I tested COMM lines only.)

* Added OVP(over voltage protector) for PSU usage.

* Added POWER and MOTOR connector for easy plug.

* Max voltage 50V and max current is 14A.


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

## License

Cheap FOCer 2 is licensed under the Creative Commons Attribution-ShareAlike 4.0 International License. To view a copy of this license, visit <http://creativecommons.org/licenses/by-sa/4.0/.>
