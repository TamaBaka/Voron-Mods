### Revisions to the Orbiter 2 StealthBurner Clockwork 2 Voron Mod.

These revisions assume that you are using a cable chain and not an umbilical cord to wire up your print head.

Problem 1:
The EBB36 module is heavily unbalanced when all of the wires are installed.  As such, having a single screw to hold it in place means that that becomes a pivot point and the motor portion of the PCB is pulled onto the cable chain where it drags along the chain as the print head moves back and forth on the chain.

My solution is to use the original hartk pcb mounting holes to add a support beam.

Problem 2:
When using the EBB36 module, the cable chain mounts are pushed to one side of the print head.  This has an unfortunate issue when using Voron Tap because when your print head is very close to the limit of the x axis (like 20mm), the chain reaches the point where it hoists itself into the air due to physics.  Normally this is okay as the chain is positioned further to the other side so you get the full range of motion before the print head wants to hoist itself.  

The reason why this is problematic is because Voron Tap detects when the head is lifted to trigger a z endstop.  When it hoists itself at the edge, you immediately get a triggered switch warning before the probe can happen.

No solution proposed yet.

