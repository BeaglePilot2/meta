#Week #6 -  

**Current Progress -**

* Added APMsubmarine vehicle folder with a few relevant files.
Github Commit : https://github.com/BeaglePilot2/ardupilot/commit/e22e7b1c3dbe3081f3cf13dae1ea1c14a1084a28

* Added steering mechanism implementation idea for OpenROV in *APMsubmarine/Notes.txt*.


**Issues -** 

* Steering mechanism for the APMrover2 implemented here -
https://github.com/BeaglePilot2/ardupilot/blob/master/libraries/APM_Control/AP_SteerController.cpp.
Could not find any PID values for the OpenROV to adapt the code for it.

* OpenROV does not seem to have a speed estimation algorithm based on IMU values.
Its Cockpit UI also does not mention speed, only motor power values, as defined here -
https://github.com/OpenROV/openrov-software/blob/master/src/plugins/rovpilot/index.js

