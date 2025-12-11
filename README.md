# EAP-Automation
Tesla EAP Auto Lane-change ESP

Needed items: <br />
ESP32-WROOM-32 DevKit ($6.50) <br />
MCP2515 + TJA1050 CAN Module ($3.90) <br />
OBD-II 16-pin Breakout Cable ($9.90) <br />
100Ω 1/4W Resistor ($0.60) <br />
Micro-USB Cable (1m) ($3.00) <br />

Wiring Diagram: <br />
OBD-II (under passenger dash) → ESP32 <br />
┌─────────────────────────────────────┐ <br />
│ OBD Pin 6  (CAN-H) ──────► MCP2515 CANH   │ <br />
│ OBD Pin 14 (CAN-L) ──────► MCP2515 CANL   │ <br />
│ OBD Pin 16 (+12V) ──► 5V Buck → ESP32 VIN │ <br />
│ OBD Pin 4/5 (GND) ───────► ESP32 GND      │ <br />
└─────────────────────────────────────┘ <br />

5. Final Test (Highway) <br />
a) Enable EAP → Navigate → Highway <br />
b) Wait for lane change suggestion (screen shows arrow) <br />
c) Blinker auto-flashes → lane change starts <br />
d) No touch needed <br />
