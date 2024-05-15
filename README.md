# VSR for VATSIM


MSFS 2020 toolbar app for VATSIM

![header](https://user-images.githubusercontent.com/4178804/215447464-ea34c0fd-3ea4-48aa-a2db-6bd687268cae.png)


<a href="https://www.youtube.com/watch?v=Xp72yo8IUcY"  target="_blank"> 
Click to play promo video </a>

Documentation:  https://docs.vsrsoftware.com 

Release 0.8.1.5 Fixes the rendering issue and also introduces many new features including a workaround for the VR bug, CTAF support and importantly no further need for a weather key.

This playlist contains demos for many of the new features:


<a href="https://www.youtube.com/playlist?list=PLPLro718J3KbW5_OcYUoJ8daLQOIuKvSc"  target="_blank"> This playlist contains demos for many of the new features </a>

<p>
Please note that as of 1st February, 2024 Asobo have introduced a bug so that VSR cannot tell if it is in VR mode; therefore the zoom function is not working correctly when you switch. One workaround is to edit the config in non VR mode and change default zoom to the same value you have for VR zoom (between 2.5 and 4) . This will have an effect of zooming at that level for non VR sessions. 
  
Release 0.8.1.5 has a new button on the bottom 


## Description

VSR is a toolbar app for Microsoft Flight Simulator 2020 that allows you to check which air traffic controllers are online when flying on the VATSIM Network. You can easily change to a frequency with a single click, or place a frequency on standby ready to change when requested to by ATC. The app also send & receives messages to and from the VATSIM network.

This app is not associated or endorsed by the VATSIM Network

## Getting Started

*** Please note ***

The install process is now via an installer programme, this will:

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
* Newtonsoft.json.dll (for messaging) - installed with vPilot
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




