# VSR for VATSIM


![header](https://user-images.githubusercontent.com/4178804/215447464-ea34c0fd-3ea4-48aa-a2db-6bd687268cae.png)


VSR is a toolbar app that helps the virtual pilot flying on VATSIM and Beyond. Real time info is provided in the cockpit for controllers and airports. You can receive and send VATSIM messages, and request a pre-departure clearance via ACARS/CPDLC or VATSIM messaaging. 

<a href="https://www.youtube.com/watch?v=Xp72yo8IUcY" target="_blank">Promo Video</a>

## Key Features
* Tabular and map views on online VATSIM controllers and traffic

* <a href="https://youtu.be/TYVWbhAM090?si=C68EsT_JKcB2AJyu&t=251" target="_blank">Airport views</a> with online stations, <a href="https://www.youtube.com/watch?v=8KpESDNXBe8" target="_blank">CTAF frequencies</a> and traffic.

* Airport <a href="https://youtu.be/cYkBaya7wHU" target="_blank">weather</a> (no key required).

* <a href="https://youtu.be/W9IA8t_TeN4" target="_blank">Change to a frequency</a> with a single click, or place a frequency on standby ready to change when requested to by ATC.

* Send & receive messages to and from the VATSIM network using vPilot.

* Import Simbrief and VATSIM <a href="https://www.youtube.com/watch?v=q0iAoEC4zIU" target="_blank">flight plans</a> to help with aircraft and flight setup.

* Request and receive ACARS CDPLC <a href="https://youtu.be/TYVWbhAM090?si=tPDElzI452YTO-If&t=12" target="_blank">Pre-departure clearances messages</a>, even if your aircraft isn't equipped with ACARS.

* <a href="https://youtu.be/TYVWbhAM090?si=TedPsMZiZBL21Ie8&t=96" target="_blank">Change Transponder code</a> from a message (such as PDC), with a single click.

* <a href="https://youtu.be/TYVWbhAM090?si=VjYQuC3VUTjVkdmg&t=158" target="_blank">Change Altimeter</a> from METAR or ATIS.

* <a href="https://youtu.be/TYVWbhAM090?si=VjYQuC3VUTjVkdmg&t=180" target="_blank">Display Beyond ATC messages</a> (experimental beta feature).

This app is not associated or endorsed by the VATSIM Network.

## Links

* <a href="https://www.youtube.com/watch?v=Xp72yo8IUcY" target="_blank">Promo Video</a>

* <a href="https://www.youtube.com/playlist?list=PLPLro718J3KbW5_OcYUoJ8daLQOIuKvSc" target="_blank">Features Playlist</a>

* <a href="https://github.com/daveblackuk/VSR/releases/tag/VSR" target="_blank">Latest Release</a>

* <a href="https://docs.vsrsoftware.com" target="_blank">Documentation</a>

* <a href="https://www.youtube.com/playlist?list=PLPLro718J3Ka5t9TzFSH_9cL2-bKV70zh" target="_blank">Tutorials</a>

* <a href="https://discord.gg/AGnazfDwYZ" target="_blank">Discord</a>


## Getting Started

The [installer programme](https://youtu.be/dQLiLrA36kM) will:

* Install latest release of the server
* Install latest release of the VSR Toolbar app
* Install latest release of the VSR/vPilot messaging DLL (and check it is installed correctly)
* Install new vPilot inbound message sounds 
* Enable configuration of the server with simBrief, VATSIM details

<a href="https://www.youtube.com/watch?v=dQLiLrA36kM&list=PLPLro718J3Ka5t9TzFSH_9cL2-bKV70zh" target="_blank"> Installer Video </a>
  
Download the zip file under latest release link on the right, unzip & run vsrinstaller,exe from the unzipped folder, as shown:

<img width="821" alt="image" src="https://user-images.githubusercontent.com/4178804/211213117-ba93578d-f1b6-4702-bf6d-a35f03f3c73e.png">


### Dependencies

* Microsoft Flight Simulator 2020
* Windows 10 and above
* [vPilot](https://vpilot.rosscarlson.dev/) to connect to VATSIM and relay messages 
* SimConnect

### Installing

* Download zip, unzip and run latest installer

### Executing program

* Run the VSR.EXE in the vs-radio-toolbar\server directory to start the app
* Start MSFS 2020, start a flight, click on VSR headset icon in the toolbat to launch the app
* A splash screen will load, if the server is correctly installed and running it will be displayed

### Architecture

![image](https://github.com/daveblackuk/VSR/assets/4178804/e6be756a-11fd-4cda-b2b8-877714790413)



## Authors

* David Black (main server and app)
* Craig Farrell (vPilot plug-in)


### Buy me a Coffee

<a href="https://www.buymeacoffee.com/deltabravozulu" target="_blank"><img width="100" alt="bmc-logo-yellow" src="https://user-images.githubusercontent.com/4178804/178282683-2d1195e1-7582-4ab5-aee3-9b57305e795c.png"></a>

## Discord channel

https://discord.gg/AGnazfDwYZ


## Acknowledgments

* Craig Farrell for developing the vPilot plug-in
* The [Leaflet](https://leafletjs.com/) map libraries 
* The [Tabulator](http://tabulator.info/) framework
* The [VAT-Spy](https://github.com/vatsimnetwork/vatspy-data-project) data project
* Maximus and others for helping [simplify](https://github.com/bymaximus/msfs2020-toolbar-window-template/issues/22) the MSFS toolbar app environment 
* Ross Carlson's [vPilot project](https://vpilot.rosscarlson.dev/) 
* Last but not least, the amazing group of people who joined and Beta programme and tested this thing until it was good to go !




