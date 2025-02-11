---
hide:
  - navigation

---
# Troubleshooting
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

Start debugging in Vpilot by typing .debug into vPilot, connect to the VATSIM network and the should contain the following:

![Alt text](images/vpilot-log.png)

Once connected with a flight started, send a message to the network (no receipient). vPilot will show the message in its interface.

![Alt text](images/vpilot-send-message.png)

The vPilot debug log will contain:

![Alt text](images/vpilot-log2.png)



#### Checking the server is running correctly

Load a browser and navigate to http://locahost:1228. If the server is functioning then the VSR screen will load.

