# dt-jupyter

Run Jupyter Lab on the Duckiebot with access to docker & duckietown-shell.  Develop and deploy directly on the device via a web-browser.  Currently a prototype with the goal of allowing students to develop strictly on a duckiebot.  While some functionality may be limited, this container would allow entry into the duckietown platform targeting high school students.

Clone and build the image on from any computer(tested on x86 and raspi):

**dts devel build -H duckie_name.local**

Launch using this command:

**docker -H duckie_name.local run -it --rm --network="host" -v /data:/data -v /var/run/avahi-daemon/socket:/var/run/avahi-daemon/socket -v /var/run/docker.sock:/var/run/docker.sock duckietown/dt-jupyter:latest-arm64v8**


Using Jupyter Lab a terminal is available.  A repository can be cloned and deployed via the terminal.

