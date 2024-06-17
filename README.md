# VSR for VATSIM


![header](https://user-images.githubusercontent.com/4178804/215447464-ea34c0fd-3ea4-48aa-a2db-6bd687268cae.png)


## Key Features

VSR is a toolbar app for Microsoft Flight Simulator 2020 that allows you to check which air traffic controllers are online when flying on the VATSIM Network.  

* Tabular and map views on online VATSIM controllers and traffic

* Airport views with online stations, CTAF frequencies, weather (no key required) & traffic 

* Change to a frequency with a single click, or place a frequency on standby ready to change when requested to by ATC. 

* Send & receive messages to and from the VATSIM network using vPilot.

* Request and receive ACARS CDPLC Pre-departure clearances messages, even if your aircraft isn't equiped with ACARS.

* Change Transponder code from a messages (such as PDC), with a single click

* Change Altimeter from METAR or ATIS

* Display Beyond ATC messages (experimental beta feature)

This app is not associated or endorsed by the VATSIM Network

## Links

* Promo Video: https://www.youtube.com/watch?v=Xp72yo8IUcY

* Features Playlist: https://www.youtube.com/playlist?list=PLPLro718J3KbW5_OcYUoJ8daLQOIuKvSc

* Latest Release: https://github.com/daveblackuk/VSR/releases/tag/VSR

* Documentation:  https://docs.vsrsoftware.com 


## Getting Started

The installer programme will:

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

[https://discord.gg/MJ6fBfYfNR](https://discord.gg/RVrp5HSPVu)


## Acknowledgments

* Craig Farrell for developing the vPilot plug-in
* The [Leaflet](https://leafletjs.com/) map libraries 
* The [Tabulator](http://tabulator.info/) framework
* The [VAT-Spy](https://github.com/vatsimnetwork/vatspy-data-project) data project
* Maximus and others for helping [simplify](https://github.com/bymaximus/msfs2020-toolbar-window-template/issues/22) the MSFS toolbar app environment 
* Ross Carlson's [vPilot project](https://vpilot.rosscarlson.dev/) 
* Last but not least, the amazing group of people who joined and Beta programme and tested this thing until it was good to go !




