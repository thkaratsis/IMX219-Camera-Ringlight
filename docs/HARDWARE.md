# Hardware reference

The supplied schematic is titled IMX219 RingLight, revision 1.0, dated 2026-05-15. Manufacturing files were exported on 2026-10-27; an export date is not evidence of a new hardware revision.

## Component information

This is a schematic-derived inventory, not a procurement-ready BOM. Verify footprints, ratings and component availability before ordering.

| References | Quantity | Description | Outstanding detail |
| --- | ---: | --- | --- |
| LED1–LED16 | 16 | Warm-white 0805 LEDs, supplier linked in README | Manufacturer part number and ratings |
| R1–R16 | 16 | 330 Ω LED series resistors | Package and power rating |
| U1–U4 | 4 | LED-bank switches | Exact part and footprint |
| Q1 | 1 | IRLZ44 MOSFET in schematic | Confirm full installed suffix and pinout |
| R17 | 1 | 1 MΩ gate pull-down | Package and rating |
| R18 | 1 | 220 Ω gate resistor | Package and rating |
| R19 | 1 | Trimmer | Resistance value and footprint |
| U5 | 1 | Photoresistor | Exact model and resistance curve unknown |
| C1 | 1 | 10 µF gate-to-ground capacitor | Voltage rating, package and polarity |
| C5 | 1 | 100 µF rail capacitor | Voltage rating, package and polarity |
| CN1 | 1 | XH 2.54 two-pin connector in schematic | Confirm actual connector part |
| U6 | 1 reference | Raspberry Pi Camera Module v2 | Camera mounting/clearance verification |

## Electrical notes

Each LED has its own series resistor. The four groups share the MOSFET-controlled return. The light-dependent network biases the gate; the trimmer adjusts its response. C1 introduces smoothing at the gate. This is an analogue circuit, not a specified digital lux threshold or regulated constant-current LED driver.

PAD1, PAD2, PAD3 and PAD4 are labeled +5V, GND, Gate and Drain respectively in the schematic. These are schematic labels, not a verified physical pinout viewed from either board side. CN1 pin 1 is labeled +5V and pin 2 GND in the schematic. Verify continuity and orientation before connection. The designer confirms operation at 5 V. The “FAN 12V” silkscreen does not specify the operating supply; use 5 V DC.

## Validation record

Designer reports that the board has been manufactured and tested. Supplied photographs document the bare and populated board. The designer confirms a test supply of 5 V. No powered photograph, current measurement, illumination measurement, thermal result or camera-fit test was supplied. No independent hardware testing is claimed.
