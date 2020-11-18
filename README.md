# APS-what-if

I translated the original java code of "determineSMB-basal" into python and can run it on a PC or Android.
This offers a safe method to play with settings and check their impact before actually adapting them in APS itself.
- On Windows, his allows me to untertake a time travel back to any time slot and see how insulin delivery 
  would have differed with different APS settings. 
- On the AAPS Android phone this will shadow the active loop and list, for the last hour, how insulin delivery 
  would have differed with different APS settings.

The historical logfiles contain enough information to rerun the APS loop, but with modified settings like
- changed target
- changed ISF
- SMB on/off
- ...

The main result in tabular and graphical output is the change in insulin required and the related SMB and TBR. 
Related data like SGV, target, Autosens ratio etc. are also shown.

A special output is the flowchart which helps to understand the logic flow through the loop. This is the 
track which statements in "determineSMB-basal" were executed and which not together with the reasoning 
of those decisions as listed in the original java code.
