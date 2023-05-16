# VSR for VATSIM


MSFS 2020 toolbar app for VATSIM

![header](https://user-images.githubusercontent.com/4178804/215447464-ea34c0fd-3ea4-48aa-a2db-6bd687268cae.png)


<a href="https://www.youtube.com/watch?v=Xp72yo8IUcY"  target="_blank"> 
Click to play promo video </a>

Documentation:  https://docs.vsrsoftware.com 

<H1> IMPORTANT Notice 21st March 2023 </H1>

MSFS SU12 appears to render the fonts in VR incorrectly; there is a fix for VSR available as a beta version under the link on the right

The key consideration is that this is a release of both the server and the toolbar app; the latter has changes that allows for the content to be resized. 
<p>
0.8.1.X will address the SU12 bug; a value of 2.5 in the VR Zoom setting will fix it. Note there are some quirks with resizing, the zoom with mouse wheel on the map for instance needs your cursor to be centred about 25% to the NW of your aircraft!
<p>
A major change is that the configuration is now maintained in the registry - if you are familiar with Regedit then the keys are at: HKEY_CURRENT_USER\SOFTWARE\DeltaBravoZulu\VSR. The server will attempt to import your existing config from config.ini if it is in the same directory.  To reverse and retry the process delete this key. 

New documentation is at https://docs.vsrsoftware.com 
 
<p>
 
<img width="500" alt="image" src="https://user-images.githubusercontent.com/4178804/226694428-eab4abd5-5ab7-4de3-b034-5b2f66ef29cb.png">



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
* Enable configuration of the server with simBrief, VATSIM and CHECKWX data

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




## Authors

* David Black (main server and app)
* Craig Farrell (vPilot plug-in)


### Buy me a Coffee

<a href="https://www.buymeacoffee.com/deltabravozulu" target="_blank"><img width="100" alt="bmc-logo-yellow" src="https://user-images.githubusercontent.com/4178804/178282683-2d1195e1-7582-4ab5-aee3-9b57305e795c.png"></a>

## Discord channel

https://discord.gg/MJ6fBfYfNR


## Acknowledgments

* Craig Farrell for developing the vPilot plug-in
* The [Leaflet](https://leafletjs.com/) map libraries 
* The [Tabulator](http://tabulator.info/) framework
* The [VAT-Spy](https://github.com/vatsimnetwork/vatspy-data-project) data project
* Maximus and others for helping [simplify](https://github.com/bymaximus/msfs2020-toolbar-window-template/issues/22) the MSFS toolbar app environment 
* Ross Carlson's [vPilot project](https://vpilot.rosscarlson.dev/) 
* Last but not least, the amazing group of people who joined and Beta programme and tested this thing until it was good to go !




