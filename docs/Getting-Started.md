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

Manual installation is not recommended, however if you wish to copy the files yourself then the following is important:

#### Directories

Copy the vs-radio-toolbar folder to either a custom folder or the community folder for your installation:

Microsoft Store:

` %AppData%\Local\Packages\Microsoft.FlightSimulator_8wekyb3d8bbwe\LocalCache\Packages\Community ` 

Steam:

` %AppData%\Roaming\Microsoft Flight Simulator\Packages\Community` 

Retail disk:

` %AppData%\Local\MSFSPackages\Community` 

Copy the server executable VSR.EXE to a directory of your choice


#### The VSR vPilot DLL

The server integrates with vPilot using a plug -in DLL - this needs to be copied to the vPilot\plugins\ folder, if vPilot has been installed without changes then this can be found under  

` %AppData%\Local\vPilot\Plugins. ` 

Stop and start vPilot, then reconnect to the network. 

If the DLL is correctly installed then the vPilot started message will appear in the message panel in the app; the further message will appear once vPilot is connected to the VATSIM network.

<img width="695" alt="image" src="https://user-images.githubusercontent.com/4178804/178728005-8896a6d1-e1b6-4570-bd8c-c8124dbff899.png">

If the messages do not appear then check that correct permissions are set for for the DLL (see below under 
[known issues](#known-issues).


If messaging is not functioning, then please see the [debugging section](#how-to-debug).
  

#### vPilot Sound files 

Copy the sound files to the following directory:

`  %AppData%\Local\vPilot\sounds ` 



### Your VATSIM User ID 

Your vPilot CID, or user ID, is used when you login to VATSIM using vPilot or via the web, it is typically a six digit number.

#### Why do you need it?

VSR uses your CID for two functions:

* Removes your "ghost" aircraft from the map, otherwise you get followed by a green aircraft. 
* Retrieves your flight plan, so you can load the departure, arrival and alternat airports.

#### Configuring the vPilot CID in VSR
The VATSIM CID is entered in the configuration screen
Tools->Edit config->Your VATSIM ID.

![Alt text](images/config-vatsim-cid.png)

### Your SimBrief ID

This tutorial covers all the aspects of SimBrief integration

 <a href="https://www.youtube.com/watch?v=q0iAoEC4zIU" target="_blank">SimBrief VSR Tutorial</a>

![Alt text](images/SB2.png)

#### Why do you need it?

VSR uses SimBrief information to:

 * Import your latest flight plan
 * Filter the airport table with your depature and arrival airports
 * Plot your route on the map
 * Add the airports to the weather menu 
 * Add quick links for the airports for other information

#### Where to find your SimBrief ID

This is found on SimBrief under Account settings->SimBrief data

Note this is your Pilot ID not your username

![Alt text](images/sb-1.png)

#### Configuring the SimBrief ID in VSR

The SimBrief ID is entered in the configuration screen
Tools->Edit config->Your SimBrief ID.


