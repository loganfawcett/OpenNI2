# OpenNI

http://structure.io/openni

This is a modified version of OpenNI2 created specifically to be installed on the Jetson TX2. The process is laid out nicely by JetsonHacks, who also helped make this fork. 

## Contributing ##

Pull requests that do not apply cleanly on top of the [`develop` branch head](http://github.com/occipital/OpenNI2/tree/develop) will be rejected.

Other than that, sensible and meaningful contributions are very welcome!

## Building Prerequisites

### Linux

- GCC 4.x

	- Download and install from: http://gcc.gnu.org/releases.html

    - Or use `apt`:
    	
	    	sudo apt-get install g++

- Python 2.6+/3.x

    - Download and install from: http://www.python.org/download/

    - Or use `apt`:

	    	sudo apt-get install python

- LibUSB 1.0.x

    - Download and install from: http://sourceforge.net/projects/libusb/files/libusb-1.0/

    - Or use `apt`:

	    	sudo apt-get install libusb-1.0-0-dev

- LibUDEV

		sudo apt-get install libudev-dev

- JDK 8.0

    - Use `apt`:
    
	    	sudo apt-get install openjdk-8-jdk

- FreeGLUT3

    - Download and install from: http://freeglut.sourceforge.net/index.php#download

    - Or use `apt`:

	    	sudo apt-get install freeglut3-dev

- Doxygen

    - Download and install from: http://www.stack.nl/~dimitri/doxygen/download.html#latestsrc

    - Or use `apt`:
    
    		sudo apt-get install doxygen

- GraphViz

    - Download and install from: http://www.graphviz.org/Download_linux_ubuntu.php

    - Or use `apt`:
    
    		sudo apt-get install graphviz

## Building

### Building on Windows:

  Open the solution `OpenNI.sln`

### Building on Linux:

  Run:

	make

### Creating OpenNI2 packages

  - Go into the directory `Packaging`
  - Run:

		ReleaseVersion.py [x86|x64|arm|android]

  - The installer will be placed in the `Final` directory
