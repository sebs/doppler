# Setup 

## Ardunio 

Please find the instructions in our repository with the dadamachines board support packages for **Arduino**.
[https://github.com/dadamachines/arduino-board-index](https://github.com/dadamachines/arduino-board-index)

## FPGA

Install **Docker** as binary: 
- [download here](https://www.docker.com/products/docker-desktop).

If you are on **macOS** using **homebrew** you can do this easily by running:  
```
brew cask install docker
```  

Open the **Docker** Application. And give it the privileges it's asking for.

[Download Firmware zip](https://github.com/dadamachines/doppler-FPGA-firmware/archive/master.zip) or git clone the [**doppler-FPGA-firmware**](https://github.com/dadamachines/doppler-FPGA-firmware):  

```
  git clone https://github.com/dadamachines/doppler-FPGA-firmware
```

Go into the directory you just cloned or extracted from the zip.    

```
cd doppler-FPGA-firmware/
```

Build the **icestorm** toolchain with **Docker**:  

This will take a while...  (you only need todo that once or when updating the toolchain)

```
docker build -t icestorm  icestorm/
```

Set the Mountpoint for **Docker**  

```
export MOUNTPOINT=`pwd`  
docker run -it -v $MOUNTPOINT:/PRJ icestorm bash
```

Now we are in the container and can build our bitstream. 