# Instructions -

**Compiling the code -**

To compile the vehicle code on a linux distro -

    git clone https://github.com/BeaglePilot2/ardupilot.git

    cd ardupilot/APMsubmarine/

    make linux

*Video tutorial : https://www.youtube.com/watch?v=HnvBVJOQr-I*

Alternatively, you can also cross-compile the vehicle code for the Erle-Brain -

    git clone https://github.com/BeaglePilot2/ardupilot.git

    sudo apt-get install gcc-arm-linux-gnueabihf g++-arm-linux-gnueabihf

    cd ardupilot/APMsubmarine/

    make pxf

*Video tutorial : https://www.youtube.com/watch?v=9GgWxrrJR9s*

**Setting up the Erle Brain -**

Download the Snappy Ubuntu Core image for the Erle Brain [here](https://mega.co.nz/#!bNFiFCzY!r06g96-mYsllv7CKcDPIJppPiLWwaElqTCxkNkgyIA8). More details - http://erlerobotics.com/blog/updating-the-software/

Flash the image onto a microSD card and insert it into the Erle Brain.

Connect the Erle Brain to your computer using a mini USB cable and let it power on.

Assign a static IP to the relevant interface -

    sudo ifconfig <interface> 192.168.7.1

Copy the APMsubmarine.elf to the Erle Brain -

    scp /path/to/APMsubmarine.elf ubuntu@192.168.7.2:/home/ubuntu

(The password for the user `ubuntu` is `ubuntu`)

**Running the code -**

SSH into the Erle Brain -

    ssh ubuntu@192.168.7.2

(The password for the user `ubuntu` is `ubuntu`)

Stop the existing ArduCopter service running on the image -

    systemctl stop copter.service

Run the APMsubmarine executable -

    sudo ./APMsubmarine.elf -A udp:127.0.0.1:6001

Open APM Planner and setup the connection to use IP address 192.168.7.1 and UDP port 6000.

Connect to the Erle Brain to test the onboard sensors.

*Video tutorial : https://www.youtube.com/watch?v=z42JYAiYx4w*
