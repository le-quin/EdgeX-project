# EdgeX-project
For the Intel EdgeX coding competition, this repo will hold the code for our device controller.

Connecting Smart Shades/Blinds, Smart Thermostat/Heating equipment, and Smart Water Controller to make it simpler to take care of indoor plants. The user can control all these setting on their phone and maybe get alerts when the plant may be in danger (according to their own specifications, getting too much sun, or underwatered, etc.). Too ambitious to connect it to a database or to automate it, but these concepts can be expanded on later.

Languages and Tools used:

-C++
-Docker
-REST APIs

Deliverable is due August 7th!


WHAT WE KNOW RIGHT NOW!

-we are making a device controller that will communicate with the EdgeX REST Device Service

-How things will work now, is that command to control the Matter device will come in through REST.  The REST device service will then send that command to the new .CPP EdgeX Matter Controller (THAT WE WILL CREATE).  That controller will communicate to the Matter Hub (i.e. Samsungs Smart Hub) to issue that command (.i.e. “Turn on light”).  Acknowledgments will then be sent back through the same path.

