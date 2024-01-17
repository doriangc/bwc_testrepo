# Software Subsystem

## Main Requirements

Battery State Estimation algorithms must be developed by the teams (SOC, SOP, SOH, SOF, RUL (optional), SOCE (optional)).
- State of Charge
How much charge remains in the battery.
- State of Power
How much power can be released or absorbed by the battery inside some time interval.
- State of Function
- State of Health
How much usable energy the battery can store considering degradation.
- Remaining Useful Life
Estimated number of operating hours before battery is unuseable.
- State of Certified Energy

Additionally:
- Communication Protocols
    - Negotiate Charge over J1772
- We must support fast charging
- BPS will validate their code through xIL testing to ensure signals are measured correctly and effectively, and that controls strategies are functional and valid. 
    - xIL is basically simulated testing.
- Must keep track of temperature.
- Software must be able to electrically connect and disconnect the battery array from the HV bus/battery to vehicle power interface.
- Interfacing with the vehicle
    "Teams may not connect any team-added sensors or actuators directly to a Stock Vehicle's CAN bus other than via their HVBS connectors. However, teams can install a secondary monitoring system (e.g. ETK) to monitor their cell and pack behavior on a team-added network."

Main Components:
1. Cell Management
    - State Estimation Algorithms
    - Fault detection
2. Charging (+ bus disconnect)
    - Fault Detection
3. In-Car Communication System
    - Probably CAN bus
4. Thermal Management
    - Fault detection
5. Secondary monitoring system
    - Communicate with equipment.
    - Application Software


BMS will be designed by the Electrical Hardware Team
For now, we will use simulations + .
