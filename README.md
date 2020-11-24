# Node-Red short wsjtx logger
Node-Red - Compact Logger for own tx/rx 

Problem: Sometimes QSO's are not logged because you didn't copy that final 73. That leads to the other station submitting a logged QSO to either LoTW or QRZ, and it not showing in your logs. Then you have to go in manually and try to find your QSO in your rather large 'ALL.TXT' log file. For some people, that can be a HUGE file and certainly time consuming.

Solution: This is a very simple (really, it's super simple) Node-Red flow that will watch your 'ALL.TXT' log and will log any time you transmit to or receive from another station. It does not log when you call 'CQ' or when you initially try calling someone with your grid square included in the packet.

Result: A very tidy, clean, log with just your TX/RX entries. This file is a fraction of the size of your 'ALL.TXT' file and will make finding that contact and verifying it a piece of cake!


Easily modifyable, simple to install!


Requirements:
- Node-Red  (https://nodered.org/) - probably already installed on your Raspberry Pi ( Howto: https://nodered.org/docs/getting-started/raspberrypi )

- Node-Red Tail   (https://flows.nodered.org/node/node-red-node-tail) Installed using Menu/Manage Pallet/Install, then search for 'node-red-node-tail' version 0.1.1 or higher

- Copy entire contents of short_logger.txt file into clipboard.

- Import script using Menu/Inport/Clipboard and paste from clipboard.

- Change the settings by double clicking 'Config' in the flow. Callsign and Grid Square have to be ALL upper case.

- Output filename will be "Filtered_Output_(Callsign)_(UTC Month)_(UTC Year).txt'

- Deploy (Done!)

-------------------------------------------------------------------------------------------------------------------------
* Obviously this script will ONLY run while Node-Red is running. Set Node-Red as system startup to enable always running.
* See https://nodered.org/docs/getting-started/raspberrypi   - Autostart On Boot
-------------------------------------------------------------------------------------------------------------------------
![Done](https://raw.githubusercontent.com/va24531/NR_short_wsjtx_logger/main/short_logger.jpg?raw=true)
