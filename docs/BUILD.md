# Fabrication and build notes

## Before ordering

Use a 5 V DC supply. Confirm the trimmer value, photoresistor selection and component footprints with the designer. The published inventory is incomplete for exact reproduction. PCB thickness, copper weight, finish and original fabrication settings are not supplied.

The manufacturing ZIP contains top/bottom copper, silkscreen, solder-mask and paste files, a board outline/document layer, and plated/non-plated drill files. Preserve the archive contents. Check the board house's preview for outline, layer alignment and drills. The ZIP is a bare-board fabrication export, not a complete assembly order.

## Assembly and verification

- Identify LED polarity and verify the chosen LED datasheet against the footprint.
- Confirm MOSFET pinout, capacitor polarity and component ratings.
- Inspect for solder bridges and check supply-to-ground resistance before power-up.
- Use a current-limited bench supply set to 5 V DC and monitor current and heating.
- Test each bank and adjust the trimmer while shading and illuminating the sensor.
- Verify camera clearance, electrical isolation and mounting before installing the camera.

A replacement photoresistor may change the adjustment range and light response. Do not describe an arbitrary substitute as equivalent without testing.

## Record a reproducible test

Record supply voltage, total current with all banks active, trimmer value, sensor identification where possible, response in light/dark conditions and temperature after sustained operation. Add photographs showing illumination and the camera installed when available.
