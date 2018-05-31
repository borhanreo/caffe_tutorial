# Caffemodel Tutorial
## Installation
    sudo mkdir Development
### Open terminal
### CPU INSTALL
	sudo apt install caffe-cpu
### Test python3 install (open terminal )
    python3
    impotr caffe
    print (caffe.__version__)
### If install successfully then no error    
### now git clone from git hub 
    cd Development
    sudo git clone https://github.com/BVLC/caffe.git
    cp Makefile.config.example Makefile.config
    sudo nano Makefile.config
### Change Line no 8 
    #CPU_ONLY := 1
    CPU_ONLY := 1
### Under the "Ubuntu Software" tab click "Source code" open terminal
        software-properties-gtk
- Tick the Source code
- Download from dropdown **Customer Service / Bangladesh server**     
### Install some dependency for cpu only
    sudo apt build-dep caffe-cpu
    sudo apt-get install libhdf5-serial-dev
### Change again Make.config file in line 95 and 96
#### line 95
        INCLUDE_DIRS := $(PYTHON_INCLUDE) /usr/local/include /usr/include/hdf5/serial/
#### line 96
            LIBRARY_DIRS := $(PYTHON_LIB) /usr/local/lib /usr/lib /usr/lib/x86_64-linux-gnu/hdf5/serial/
            
            
            
            