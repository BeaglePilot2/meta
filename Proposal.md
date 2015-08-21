BeaglePilot 2.0 - Google Summer of Code 2015 Proposal
===

## About the project -

The aim of the project is to create an open hardware underwater vehicle based on BeagleBone Black. The project will involve using the OpenROV code base and the APM, to provide autopilot capabilities. ROS will be used as a bridge (mavros) to interface with the APM. The project will enable hobbyists to get access to a low cost, easy to use and open hardware underwater vehicle platform with autopilot capabilities which they can modify according to their needs and requirements. Also, APM is used in multicopters, planes and ground rovers. Adding an underwater vehicle, eg APM:Submarine will improve its already impressive portfolio further. The programming languages used for the project wil be C/C++, nodejs. Other open source technologies that will be used are ROS, APM planner etc.

## Impact on community -

Rohith Madhavan, Student : After successful completion of the project, it will be possible for the community to use the advanced autopilot capabilities which the APM has to offer for underwater vehicles too, such as submarines and ROVs. This will make autonomous navigation easier and is great for the exploration of water bodies. Combining the open source technologies of APM, ROS, OpenROV and BeagleBoard into a single project benefits each of the aforementioned and hence the impact on the community is manifold. The project will also add to the portfolio of APM vehicles and therefore can be used as a base for several other projects.

Victor Mayoral Vilches, Mentor : The project will enable growth in both size and interest in the field of drones in communities such as DIYDrones, which currently has 65,000+ users. Having a strong software architecture for underwater vehicles is a must in order to further improve the field, especially for autonomous navigation. The addition of the capabilities of the APM such as a well-defined logging system, groung control stations, autonomous mission planning, drivers for various sensors, ROS integration etc. to the vehicle will definitely improve functionality and make it easier to control underwater vehicles.

## Timeline -

**During the community bonding period (27th April to 25th May) -**

Will start working on the OpenROV code and determine the features to be ported after discussion with the mentors. Will brush up nodejs since it will be of great importance during the course of the project for porting the OpenROV code.

**Pre-mid-term evaluation - (25th May to 26th June) -**

* Week 1: Start the porting of relevant OpenROV features to APM.

* Week 2: The support for the various sensors shall be implemented.

* Week 3: Testing and debugging of the above.

* Week 4: Will finish porting OpenROV code to C/C++. The same shall be submitted for mid-term evaluation review.

**Post-mid-term evaluation - (3rd July to 17th August) -**

* Week 6: APM interfaced via a ROS bridge (mavros).

* Week 7: Creating necessary libraries for the APM submarine.

* Week 8: Testing the autopilot on the underwater vehicle.

* Week 9: Integrating the code with the main ardupilot repository.

* Week 10: Final housekeeping, wrap-up and documentation.
