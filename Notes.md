**Notes on OpenROV code -**

* Neutrally Buoyant ROV, ie neither floats nor sinks.
  Motors spin in reverse direction with double power to compensate for thrust.

* Navigation -
  
  Forward - Port Motor CCW, Starboard Motor CW (viewed from rear)

  Reverse - Port Motor CW, Starboard Motor CCW (viewed from rear)

  Left - Both Port and Starboard Motors CW (viewed from rear)

  Right - Both Port and Starboard Motors CCW (viewed from rear)

  Ascend - Vertical Motor CW (viewed from top)

  Descend - Vertical Motor CCW (viewed from top)

* Steering mechanism for the APMrover2 implemented here -
https://github.com/BeaglePilot2/ardupilot/blob/master/libraries/APM_Control/AP_SteerController.cpp.
Could not find any PID values for the OpenROV to adapt the code for it.

* OpenROV does not seem to have a speed estimation algorithm based on IMU values.
Its Cockpit UI also does not mention speed, only motor power values, as defined here -
https://github.com/OpenROV/openrov-software/blob/master/src/plugins/rovpilot/index.js
