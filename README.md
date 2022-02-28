# ESP32-MCW-Metrobus-Simple-CAN-Lighting-Controller
CAN Lighting Controller for Classic MCW Metrobus (to replace original damaged wiring)

# Why is this needed?
In order to rewire my classic bus, I need to replace the wiring loom following rodent damage. It makes sense to upgrade the electrical system to operate with modern LED lamps, provide lamp failure detection, and provide engine sensor details to the drivers cab.

# Proposed Layout
- Front & Rear Lighting Control Unit, these will be a duplicate of the same module with different settings, and provide fused switched outputs for external vehicle lighting.
- Engine Control Unit, this isn't particularly complex, but will control engine start-stop, and allow connection of oil pressure, temperature sensors, fire warnings, etc. This will incorporate all the original sensor functions, as well as coolant level, and safety interlocks (will not start if engine door open etc).
- Dashboard Cluster, will provide a digital dashboard appropriate to the vehicle and able to show warnings, speeds, values.
- Driver Input Controller, this will take inputs for start stop / ignition, and all control switches, provide security for anti-theft etc.

The system will be run with a can-bus and wake-up signal, power and ground only, allowing simple connection and addition of modules in required. It will have the ability to add further modules to expland for instance, lighting outputs for running lights, work lights, etc. It will allow another lighting controller for trailer lighting control, trailer lighting control could also be provided over a ESPNOW connection to ensure stability even if there 
