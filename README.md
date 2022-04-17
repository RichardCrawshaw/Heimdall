# Heimdall
A diagnostics application for CBUS^(r)^, written in .NET 6. It is intended to be cross-platform, but 
will initially target Windows, as that is what I have most experience with.

## The Name
Heimdall is the Norse God who keeps watch for invaders and the onset of Ragnarök. The act of watching
seemed the closest to monitoring while keeping to the theme of Norse Mythology with gods and godesses 
for applications and places for libraries.

## Initial CBUS^(r)^ Diagnostics
It is still early days for formal diagnostics for CBUS^(r)^. There is (hopefully) an initial spec in the 
process of being written, but beyond that there is no explicit support.

However, it is possible using the CBUS^(r)^ communication specification it should be possible with 
existing modules to implement a basic ping test. Version 6c states that each module should respond to a 
QNN (Query Node Number) message with a PNN (Query Node Number Response) message. So if a QNN is sent on
a regular basis, every minute or so, it will be possible to determine which modules are present, and 
deduce which modules are no longer communicating.

In its initial form Heimdall will implement this regular ping and report any changes in modules that
respond.

## Future Development
It is intended that Heimdall will develop as CBUS^(r)^ Diagnostics develops. Furthermore it is hoped that 
by creating a CBUS^(r)^ Diagnostics application it will help cement the use of diagnostics in future 
CBUS^(r)^ modules and encourage the update of existing firmware and or the generation of new firmware for 
current modules to incorporate diagnostics.

## Colaboration
All projects benefit from multiple perspectives and additional viewpoints; as such I welcom colaborators
to Heimdall. I would particularly welcome colaborators who can bring Linux and Mac OS experience.
