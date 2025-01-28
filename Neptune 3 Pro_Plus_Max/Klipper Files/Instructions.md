## These config files are designed to be used with TheFeralEngineer's configs
Upload them to your config and include them in your printer.cfg. 
Either rename or delete already existing macros with the same name.
The only things you should need to adjust are:

- screws_tilt_adjust positions depending on your exact printer model
  
- delete or rename the existing pause and resume macros in TheFeralEngineer's configs

the steps are well documented in the official Klipper documentation.
  
- Add the following to the machine start g-code:
  
    START_PRINT EXTRUDER=[nozzle_temperature_initial_layer] BED=[bed_temperature_initial_layer_single]
  
    The variables in brackets may need to be changed depending on the slicer being used. The ones that are being used are for Orca Slicer.
    Here are some for the most common slicers:

    Prusa Slicer: START_PRINT EXTRUDER=[first_layer_temperature] BED=[first_layer_bed_temperature]
    
    
## Functions:
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

### Mods
- clean_nozzle.cfg
  - a macro for nozzle cleaning using a brush that is mounted to the bed
  - parameters like the position of the brush need to be defined first (see diagramm at the top of the file)
