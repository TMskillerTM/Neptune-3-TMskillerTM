Upload them to your config and include them in your printer.cfg. 
Either rename or delete already existing macros with the same name.
The only things you should need to adjust are:

- Bed_screw positions depending on your exact printer model
- bed_mesh_min and bed_mesh_max depending on your exact printer model

the steps are well documented in the official Klipper documentation.

# Functions:
- accessibility.cfg:
  - useful commands for a userfriendly experience.
 
- main_macro.cfg
  - important macros for printer calibration/operation of the printer
  - Example: bed leveling macro, PID macros
 
- testing.cfg
  - macros for testing (currently only for speed testing)
 
- pause_resume_cancel.cfg
  - as the name indicates, macros for pause, resume and canceling the print
  - if you're using it with TheFeralEngineer's printer.cfg you would need to change/delete the already existing ones or just not use this configfile

- clean_nozzle.cfg
  - a macro for nozzle cleaning using a brush that is mounted to the bed
  - parameters like the position of the brush need to be defined first (see diagramm at the top of the file)
