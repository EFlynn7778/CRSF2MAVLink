# CRSF2MAVLink
CRSF Telemetry to MAVLink Telemetery Converter

CRSF (Crossfire) Telemetry to MAVLink Telemetry converter.

Implemented for use with Automatic Antenna Trackers, or a bridge between CRSF and any other MAVLink compatible device. 

CRSF Sensors are limited compared to MAVLink, so only those that can be translated are sent over MAVLink

This was implemented on a Teensy 4.0 due to plentiful hardware serial ports, but is Arduino compatible and should compile for just about anything with a few chages.
