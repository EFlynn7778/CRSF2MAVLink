# CRSF2MAVLink

CRSF (Crossfire/ELRS) Telemetry to MAVLink Telemetry converter.

Implemented for use with Automatic Antenna Trackers, or a bridge between CRSF and any other MAVLink compatible device such as MissionPlanner running on a PC etc. 

CRSF Sensors are limited compared to MAVLink, so only those that can be translated are sent over MAVLink. The remainder can be set/sent as statc values.

MAVLink messages sent are, Heartbeat, Status, GPS, HUD, ATTITUDE

Some of the data types sent over MAVLink may be incorrect as they differ from CRSF to MAVLink. i.e. CRSF sends Gspeed as KM/h and MAVLink expects M/s. I Only validated the ones I am currently using, and a few others. I will update later with full validation.

This was implemented on a Teensy 4.0 due to plentiful hardware serial ports, but is Arduino compatible and should compile for just about anything with a few chages.


Based on code by David Wyss(mavlink) and Rob Thomson(CRSF)
