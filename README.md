# VSR VATSIM Radio


MSFS 2020 toolbar app for VATSIM



<a href="https://www.youtube.com/watch?v=TaDjbuafZbg" target="_blank"> <img width="800" alt="image" src="https://user-images.githubusercontent.com/4178804/178738153-935324aa-7ce9-4857-81c4-af3385934324.png"> </a>

<a href="https://www.youtube.com/watch?v=TaDjbuafZbg" target="_blank"> 
Click to play promo video </a>


## Description

VATSIM Radio (VSR) is a toolbar app for Microsoft Flight Simulator 2020 that allows you to check which ATC controllers are online when flying on the VATSIM Network. You can easily change to a frequency with a single click, or place a frequency on standby ready to change when requested to by ATC. The app also receives messages from the VATSIM network.

This app is not associated or endorsed by the VATSIM Network

## Getting Started


<a href="https://github.com/daveblackuk/VSR/releases"> Download </a> the zip file containing the latest version and unzip the entire folder "vs-radio-toolbar" into your community folder. The server directory needs create, write and delete rights to the directory to create it’s working files.

<img width="370" alt="image" src="https://user-images.githubusercontent.com/4178804/178781921-e038b421-50f8-448e-87d2-95d75f829353.png">

Once you are happy that everything is installed, then launch MSFS and click on the VSR.EXE file in the server directory.

Server will wait for MSFS to start.  

<img width="960" alt="image" src="https://user-images.githubusercontent.com/4178804/178726943-1c6d54e2-d484-4883-9827-3fe21f5015f4.png">

Once the flight is started click on the headset icon in the toolbar, 

<img width="899" alt="image" src="https://user-images.githubusercontent.com/4178804/178727280-07c9c089-f153-44d6-b3ee-b3ed8c04844f.png">


The app should load and get updated with your current position.

<img width="686" alt="image" src="https://user-images.githubusercontent.com/4178804/178278004-fd93cd76-da0e-47d7-b99b-b69de9fbb771.png">


To test the app, click on the Unicom frequency 122.800 and your Comm1 radio should change to this frequency.  

## vPilot integration - Important requirement for messages from Vatsim network

The server integrates with vPilot using a plug-in DLL - this needs to be copied to the vPilot\plugins\ folder, if vPilot has been installed without changes then this can be found under  

C:\Users\[your username]\AppData\Local\vPilot\Plugins. 

There is a batch file (install_message.bat) in the server directory that will automatically copy the DLL to the correct directory. 

Stop and start vPilot, the reconnect to the network. 

If the DLL is correctly installed then the vPilot started message will appear in the message panel in the app; the further message will appear once vPilot is connected to the VATSIM network.

<img width="695" alt="image" src="https://user-images.githubusercontent.com/4178804/178728005-8896a6d1-e1b6-4570-bd8c-c8124dbff899.png">

If the messages do not appear then check that correct permissions are set for for the DLL (see below under Known issues)

## Config.ini

The server directory contains a config.ini file; for most configurations this should be unchanged, however if you wish to add live TAF/METAR information then add a key obtained from https://www.checkwxapi.com/ 

* The refresh time is set to 10 minutes, setting to 0 will disable automatic refreshes and require a manual refresh.
* The maximum distance for stations is set at 1500nm; this can be changed dynamically in the App.
* The default radio is set at Comm1 active, this can be changed in this file

<img width="977" alt="image" src="https://user-images.githubusercontent.com/4178804/178731182-4aebb291-9904-4ac7-ab64-05e1f9f27c14.png">



### Dependencies

* Microsoft Flight Simulator 2020
* Windows 10 and above
* [vPilot](https://vpilot.rosscarlson.dev/) to connect to VATSIM and relay messages 
* Newtonsoft.json.dll (for messaging) - installed with vPilot
* SimConnect

### Installing

* Download latest zip
* Unzip and copy vs-radio-toolbar directory to either community or chosen folder
* run batch install_message.bat in the vs-radio-toolbar\server directory to copy the DLL under vPilot installation


### Executing program

* Run the VSR.EXE in the vs-radio-toolbar\server directory to start the app
* Start MSFS 2020, start a flight, click on VSR headset icon in the toolbat to launch the app
* A splash screen will load, if the server is correctly installed and running it will be displayed


## Known issues

* AFTER CTD restart the VSR server. This can be done from U/I using debug menu in left hand header above Airports table. Failure to restart might cause the App from updating frequencies and getting postion updates from Sim. 

* Crash to desktop issues have been reported with the Fenix A320; changing the memory allocations as per <a href="https://kb.fenixsim.com/potential-way-to-help-stop-ctds" target="_blank"> these instructions </a> may resolve this issue. 

* Controllers may appear above the Unicom frequency and on the map at 0 miles distance, this is caused by the VATSIM feed data baing out of sync and is designed to ensure that controllers are always visible irrespective of the feed. This is normally shortlived and disappears with a refresh about a few minutes when the controller is assigned the correct location. 

* If you are not receiving messages from Vatsim, then the DLL may require additional permissions to run; right click on the DLL and ensure that the unblock security check box, if shown, has been checked . Stop and start vPilot, the reconnect to the network. 

![image](https://user-images.githubusercontent.com/4178804/179221242-f3318ff9-dd48-4426-b801-16dab1d3ea4b.png)

• Some icons do not render correctly in MSFS; this is due to limitations in the MSFS internal browser. This due to the style sheets in the tabulator framework used for the tables; it is on the backlog to resolve (if possible).

• Window sizing is an issue with SU9 and currently (9th Aug) SU10, this also causes issues with scrollbars - The app uses a fixed size but the enclosing window size is not persistant, known ASOBO fault. 


## Authors

* David Black (main server and app)
* Craig Farrell (vPilot plug-in)


### Buy me a Coffee

<a href="https://www.buymeacoffee.com/deltabravozulu" target="_blank"><img width="100" alt="bmc-logo-yellow" src="https://user-images.githubusercontent.com/4178804/178282683-2d1195e1-7582-4ab5-aee3-9b57305e795c.png"></a>


## Change Log

<a href="https://docs.google.com/spreadsheets/d/1pHLaK52r3LXt4Q7lJwkGNhDcoo6tHtJIGlU1LCS9lZw/edit#gid=0" target="_blank" >Change log </a>  including beta releases

## Version History

* 1.0
    * Initial Release 15th July, 2022

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



## Help screens

![Slide1](https://user-images.githubusercontent.com/4178804/178279125-5ce48542-b3b9-4db2-8ae3-9abb3ebda818.jpeg)
![Slide2](https://user-images.githubusercontent.com/4178804/178279144-250af7f3-1f23-4f78-ad72-3355ea2c4134.jpeg)
![Slide3](https://user-images.githubusercontent.com/4178804/178279149-ee352555-fa55-43c4-b268-f44a7ced10fb.jpeg)
![Slide4](https://user-images.githubusercontent.com/4178804/178279153-9d269d7d-8711-46b0-9352-9873c0081fb9.jpeg)
