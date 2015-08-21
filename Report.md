Report -
========

The aim of *BeaglePilot 2 : Making Underwater Drones*, my Google Summer of Code 2015 project, was to create an open hardware underwater vehicle based on BeagleBone Black. An introductory video outlining the same can be viewed [here](https://www.youtube.com/watch?v=GvIZOCGMYiA).

![BeaglePilot2](https://github.com/BeaglePilot2/meta/blob/master/images/beaglepilot2.jpg)

The code from the project can be found at https://github.com/BeaglePilot2/ardupilot, with [APMsubmarine](https://github.com/BeaglePilot2/ardupilot/tree/master/APMsubmarine) being the relevant vehicle folder. Instructions for compiling and running the vehicle code on Erle Brain, along with tutorial videos, are located [here](https://github.com/BeaglePilot2/meta/blob/master/Instructions.md).

Although the base structure of the APMsubmarine vehicle code is in place and compiles successfully, there is still quite a bit of work to be done before the code is ready to be implemented on an underwater vehicle. The complexity of the project turned out to be more than what was initially expected and hence not all that was mentioned in the [proposal](https://github.com/BeaglePilot2/meta/blob/master/Proposal.md) could be achieved within the GSoC time frame. I would like to continue working on this project in the future to add more functionality.

The project was a great learning experience for me. Getting to work with amazing people on a project that was of interest to me, but at the same time something that was new and challenging, made for an enriching summer.

I would like to take this opportunity to thank my mentors Víctor, Iñigo and Alejandro for their guidance throughout the course of the program. Their prompt feedback and help enabled me to progress even when the going seemed tough.

I would also like to thank Jason, Vladimir and the rest of the BeagleBoard.org community for their support, and Google for providing this wonderful platform for students.

Rohith Madhavan

---

## Summary -

| Goal | Status |
|------|--------|
| APMsubmarine vehicle code | Base structure in place, still a WIP |
| Compiling a generic build using `make linux` | Successful |
| Cross compiling for Erle Brain using `make pxf` | Successful |
| Erle Brain IMU on Primary Flight Display | Working |
| Interfacing Erle Brain via ROS | Left aside |
| Testing code on underwater vehicle | Not done, unable to test |
| Integrating code with Upstream | Not done, vehicle code not complete |
