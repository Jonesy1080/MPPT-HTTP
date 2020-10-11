# MPPT-HTTP
A web interface for viewing EPEver and SolarEpic MPPT charge controllers via Raspberry Pi.

This Project Contains:
mppt.html - The Web server file
mppt.js - The JavaScript file for interfacing the HTML to the WebSocket server
install.sh - The installation script.

The installation script:
1. Tested working on the newest Raspberry Pi OS Lite
2. Downloads and installs all prerequisites:
  a. XRUSB driver
  b. nginx
  c. libmodbus
3. Configures NGINX web server
4. Starts WebSocket server automatically on boot

Known Problems:
1. WebSocket client/server not immediate. Using websocketd, this has not been a problem with other programs
2. MBPOLL is off-by-one, in other words, to add registers, you will need to offset the desired register by 1

Other Notes:
A left-menu on the html is commented out, so you can add other features later
The web design is a modified template from w3.
