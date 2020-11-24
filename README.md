# Node-Red short wsjtx logger
Node-Red - Compact Logger for own tx/rx 

Tired of manually searching in your 'ALL.TXT' log to see if you worked a station in WSJT-X or JTDX? This is a very simple (really, it's super simple) Node-Red flow that will watch your 'ALL.TXT' log and will log any time you transmit to or receive from another station. It does not log when you call 'CQ' or when you initially try calling someone with your grid square included in the packet.

Easily modifyable, simple to install!

Requirements:
- Node-Red  (https://nodered.org/) - probably already installed on your Raspberry Pi

- Node-Red Tail   (https://flows.nodered.org/node/node-red-node-tail) Installed using Menu/Manage Pallet/Install, then search for 'node-red-node-tail' version 0.1.1 or higher

- Copy entire contents of .txt file into clipboard.

- Import script using Menu/Inport/Clipboard and paste from clipboard.

- Change the settings by double clicking 'Config' in the flow.

- Deploy (Done!)

