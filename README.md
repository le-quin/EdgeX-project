# EdgeX-project
For the Intel 2023 EdgeX coding competition, this repo was supposed to hold the code for our device controller. After a semester of confusion and lack of guidance, we have changed our objective toward something more educational: essentially a beginner's guide to EdgeX, everything that we wish we knew before getting into this competition.

## Our project idea

Connecting Smart Shades/Blinds, Smart Thermostat/Heating equipment, and Smart Water Controller to make it simpler to take care of indoor plants. The user can control all these setting on their phone and maybe get alerts when the plant may be in danger (according to their own specifications, getting too much sun, or underwatered, etc.). Too ambitious to connect it to a database or to automate it, but these concepts can be expanded on later.

### Devices to connect:

-SwitchBot Curtain (with Hub)
-Google Nest Thermostat
-Maybe Smart Lights

### Languages and Tools used:

-C++
-Docker
-REST APIs

### How it should work:
-we are making a device controller that will communicate with the EdgeX REST Device Service

-How things will work now, is that command to control the Matter device will come in through REST.  The REST device service will then send that command to the new .CPP EdgeX Matter Controller (THAT WE WILL CREATE).  That controller will communicate to the Matter Hub (i.e. Samsungs Smart Hub) to issue that command (.i.e. “Turn on light”).  Acknowledgments will then be sent back through the same path.

## Contents of This Repo
This repo contains:
A summary of the EdgeX Foundry Coding Competition
  - Tools used
  - Explanation of Problem
  - Challenge
  - Goals
The Idea we had for our project
  - Demo video of UI
  - Explanation of UI
  - Explanation of our project
Educational portion that exposes newcomers to the ideas and principles of EdgeX 

### Educational Material:
In the Educational Material folder, we include a document briefly explaining edge computing, Matter, and how EdgeX utilizes these concepts. There is also a document that includes links to articles, websites, and videos we found useful throughout the semester.

### User Interface:
In the User Interface folder located in this repository, we have included a video that demonstrates the idea behind our device service UI.
Also included there are: an explanation of what our device service would do and a guide behind the contents of the video. 
