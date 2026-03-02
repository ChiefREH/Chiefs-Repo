# BASIC NODE-RED SETUP

## Editor layout
- Zoom In/Zoom Out in bottom right-hand corner (- o +)

## Palette
- Installing Palette Nodes:
    - contrib-themes (for dark mode)
    - contrib-cip-ethernet-ip (for PLCs)
    - contrib-pccc (for AB PLCs)
    -ui-led (for Dashboards) 
    - dashboard (for Dashboard UI) deprecated, use anyway!
    - nodes for RaspberryPi GPIO
    - node-ui-table (for SCADA)
    - node-crypto-js (for AES encryption)

## Color theme
- I prefer dark mode (monokai theme)

## First Workflow
- Hover over output points to see information

### Inject
- Timestamp can be clicked in debug window to show different formats
- Inject can repeat based on time interval
- See Delay to rate limit multiple injections
- Can send multiple variables: payload, topic, rate, etc.
	
### Debug
- Displays msg.payload by default (right sidebar window)
- Can see everything injected by changing Output properties to “complete msg object”

### Switch
- “If-Then-Else” statements
- Rules and Conditions in the drop-down
- Can stop after the first match
- Each rule creates its own output on the node  (“ → 1”)
	
### Change
- Can Set, Change, Delete and Move a value in the payload
	
### Filter
- Exceptions Rule
- “Blocks unless value changes”
- Several other options to create more conditions
	
### Delay
- Is a “sleep” node that delays passing the payload through the flow
- Can “rate limit” the number of messages per time interval
	
### Trigger
- When activated, can send True/False, then after an interval, sends any msg.payload variable
	
### HTTP Request
- Grabs meta data from a webpage
- GET Method: https://httpbin.org/get
- Properties: ← Return “a parsed JSON object”

### Split & Join
- Breaks an output into individual objects (or join individuals back together)
	
### Link In / Link Out
- Connects nodes that are in separate areas or other flows
- Think of it as invisible wires that pass signals between flows
- Similar to the wiring done in AB Studio 5000 Function Block Diagrams
	
### Exec	
- For Linux, gives access to terminal commands
- Outputs (put a debug on each one)
    - stdout – standard output
    - stderr – standard error
    - return code – outputs a copy of the return code (rc) 			
- Example Linux Commands
    - whoami, uname -a, hostnamectl, pwd, uptime, free -h, df -h, ifconfig, netstat

### Export Workflow
- Save your work to the hard drive
