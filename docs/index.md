# VSR for VATSIM 


MSFS 2020 toolbar app for VATSIM


<a href="https://www.youtube.com/watch?v=Xp72yo8IUcY" target="_blank"> <img width="800" alt="image" src="https://user-images.githubusercontent.com/4178804/178738153-935324aa-7ce9-4857-81c4-af3385934324.png"> </a>

<a href="https://www.youtube.com/watch?v=Xp72yo8IUcY"  target="_blank"> 
Click to play promo video </a>

## Description

VSR is a toolbar app for Microsoft Flight Simulator 2020 that allows you to check which air traffic controllers are online when flying on the VATSIM Network. You can easily change to a frequency with a single click, or place a frequency on standby ready to change when requested to by ATC. The app also send & receives messages to and from the VATSIM network.

This app is not associated or endorsed by the VATSIM Network

### Features


<img src="images/vs0.png"  width="75%" height="75%"></img>
<img src="images/vs1.png"  width="75%" height="75%"></img>
<img src="images/vs2.png"  width="75%" height="75%"></img>
<img src="images/vs3.png"  width="75%" height="75%"></img>
<img src="images/vs4.png"  width="75%" height="75%"></img>
<img src="images/vs5.png"  width="75%" height="75%"></img>
<img src="images/vs6.png"  width="75%" height="75%"></img>
<img src="images/vs7.png"  width="75%" height="75%"></img>
<img src="images/vs8.png"  width="75%" height="75%"></img>
<img src="images/vs9.png"  width="75%" height="75%"></img>
<img src="images/vs10.png"  width="75%" height="75%"></img>

## Getting Started

VSR consists of three components:

* A server that runs in the background, orchestrating data sources and messages.
* A toolbar app that installs in your community folder and runs in MSFS.
* A dynamic link library (DLL) that enables messaging between VATSIM and VSR.

An optional sound file can be installed under vPilot which makes it easier to hear incoming messages. <a href="https://youtu.be/JVm2Azv1CiQ" target="_blank">(preview)</a>

### Installation 


The install process can either be run through the installer programme, or manually. The installer will:

* Install latest release of the server
* Install latest release of the VSR Toolbar app
* Install latest release of the VSR/vPilot messaging DLL (and check it is installed correctly)
* Install new vPilot inbound message sounds 
* Enable configuration of the server with simBrief, VATSIM and CHECKWX data
* Create an optional desktop icon for the server 

<a href="https://www.youtube.com/watch?v=dQLiLrA36kM&list=PLPLro718J3Ka5t9TzFSH_9cL2-bKV70zh" target="_blank"> Installer Video </a>

### Dependencies
* Microsoft Flight Simulator 2020
* Windows 10 and above
* [vPilot](https://vpilot.rosscarlson.dev/) to connect to VATSIM and relay messages 
* Newtonsoft.json.dll (for messaging) - installed with vPilot
* SimConnect (installed with MSFS)

  
### The VSR Zip file

Download the latest version from the <a href="https://github.com/daveblackuk/VSR/releases/tag/VSR" target="_blank">github repository</a>

Unzip the file; the directory structure should be as follows:

<img width="821" alt="image" src="https://user-images.githubusercontent.com/4178804/211212976-09aa0e50-54db-4c63-bec0-7e6e6ac29eb3.png">

You can either run the installer, or install manually.

### Automatic installer
#### Installation process

The installer will undertake a number of checks as it proceeds:

* Check the MSFS community folder, it will vary based upon whether MSFS was installed:
    * Via MS Store  
    * Via Steam
    * Via a physical disk
    * Manually 
* Check the versions of the downloaded components
* Check whether you wish to continue or install manually
* Ask you where you wish to install the toolbar app component
  
   The default location is the detected community folder; however you may
   wish to install it elsewhere, for instance if you are using an add-on linker.
   If you answer n then you will need to select a folder manually.

* Ask you where you wish to install the server component. 

   By default this is under the toolbar folder; hwoever you may wish to install it elsewhere. If you answer n then you will need to select a folder manually.

* Check whether an existing configuration exists in the selected server location
* Copy the toolbar app to the selected folder.
* Copy the VSR server to the selected folder.
* Ask you whether you want the new VSR message sound for vPilot installed <a href="https://youtu.be/JVm2Azv1CiQ" target="_blank">(preview)</a>
  
   If you answer yes, then the installer will backup two existing files into a backup directory under vPilot/sounds and copy over the new files.

* Ask you if you wish to create a desktop shortcut to the VSR Server.
* Start vPilot and wait for an incoming message to ensure the DLL is working correctly.
  
* If there are issues, please read the DLL section (below)

#### Virus warnings
Some AV solutions have issues with the installer; ![image](https://user-images.githubusercontent.com/4178804/209872578-79477307-869d-4743-8cb9-7182a85ac571.png)

If this occurs, run the installer as administrator and allow the execution 

### Manual installation
#### Directories
#### The VSR vPilot DLL

The server integrates with vPilot using a plug -in DLL - this needs to be copied to the vPilot\plugins\ folder, if vPilot has been installed without changes then this can be found under  

C:\Users\[your username]\AppData\Local\vPilot\Plugins. 

Stop and start vPilot, then reconnect to the network. 

If the DLL is correctly installed then the vPilot started message will appear in the message panel in the app; the further message will appear once vPilot is connected to the VATSIM network.

<img width="695" alt="image" src="https://user-images.githubusercontent.com/4178804/178728005-8896a6d1-e1b6-4570-bd8c-c8124dbff899.png">

If the messages do not appear then check that correct permissions are set for for the DLL (see below under 
[known issues](#known-issues).


If messaging is not functioning, then please see the [debugging section](#how-to-debug).
  

### vPilot Sound file

C:\Users\[your username]\AppData\Local\vPilot\sounds. 

### The Metar key
#### Why do you need a key?
#### Obtaining free key
#### Configuring the key in VSR

### Your vPilot CID
#### Why do you need it?
#### Configuring the vPilot CID in VSR

### Your SimBrief ID
#### Why do you need it?
#### Where to find your SimBrief ID
#### Configuring the SimBrief ID in VSR

## Running the server
### Startup procedure
## Troubleshooting
### Known issues

* If you start a new flight after returning to the main simulator menu, then please restart the server from the config menu to ensure the correct aircraft location is shown in VSR.

* AFTER CTD restart the VSR server. This can be done from U/I using debug menu in left hand header above Airports table. Failure to restart might cause the App from updating frequencies and getting postion updates from Sim. 

* Crash to desktop issues have been reported with the Fenix A320; changing the memory allocations as per <a href="https://kb.fenixsim.com/potential-way-to-help-stop-ctds" target="_blank"> these instructions </a> may resolve this issue. 

* Controllers may appear above the Unicom frequency and on the map at 0 miles distance, this is caused by the VATSIM feed data baing out of sync and is designed to ensure that controllers are always visible irrespective of the feed. This is normally shortlived and disappears with a refresh about a few minutes when the controller is assigned the correct location. 

* If you are not receiving messages from Vatsim, then the DLL may require additional permissions to run; right click on the DLL and ensure that the unblock security check box, if shown, has been checked . Stop and start vPilot, the reconnect to the network. 

![image](https://user-images.githubusercontent.com/4178804/179221242-f3318ff9-dd48-4426-b801-16dab1d3ea4b.png)

• Some icons do not render correctly in MSFS; this is due to limitations in the MSFS internal browser. This due to the style sheets in the tabulator framework used for the tables; it is on the backlog to resolve (if possible).

### How to debug
#### Checking the Toolbar app is being loaded by MSFS

You can check in the simulator to ensure the toolbar app is installed and loaded:

![Microsoft Flight Simulator Screenshot 2022 06 09 - 05 41 42 96](https://user-images.githubusercontent.com/4178804/210109986-72bc6617-90dc-4ffd-9ddc-2222ec0a2822.png)

#### Checking that the DLL is being loaded by vPilot

#### Checking the server is running correctly
Load a browser and navigate to http://locahost:1228. If the server is functioning then the VSR screen will load.



## FAQs

## Authors

* David Black (main server and app)
* Craig Farrell (vPilot plug-in)


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





## Additional Screenshots
![Alt text](./images/screenshot1.png)

![Alt text](./images/screenshot2.png)

![Alt text](./images/screenshot3.png)
s
![Alt text](./images/screenshot4.png)


## Buy me a Coffee

<a href="https://www.buymeacoffee.com/deltabravozulu" target="_blank"><img width="100" alt="bmc-logo-yellow" src="https://user-images.githubusercontent.com/4178804/178282683-2d1195e1-7582-4ab5-aee3-9b57305e795c.png"></a>
