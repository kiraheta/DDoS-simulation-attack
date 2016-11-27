# Overview
A DDoS simulation attack for educational purposes

# Environment Setup
##Kali Linux

1. Download [Kali Linux](https://www.kali.org/downloads/)

   Or from terminal: `curl -L http://cdimage.kali.org/kali-2016.2/kali-linux-2016.2-amd64.iso>kali-linux-2016.2-amd64.iso`
2. Install on [VMware Fusion](http://www.vmware.com/products/fusion/fusion-evaluation.html) or [VirtualBox](http://www.oracle.com/technetwork/server-storage/virtualbox/downloads/index.html)

##Loic (Low Orbit Ion Cannon) 
An open source network stress tool, written in C#. Based on [Praetox's LOIC project](https://sourceforge.net/projects/loic/)

[SOURCE](https://github.com/NewEraCracker/LOIC)

### Disclaimer
This tool is released for educational purposes only, with the intent of helping server owners develop a "Hacker Defense" attitude. This tool comes without any warranty at all.

You may not use this software for any illegal or unethical purpose; including activities which would give rise to criminal or civil liability.

Under no event shall the Licensor be responsible for the activities, or any misdeeds, conducted by the Licensee.

### Running LOIC on LINUX / MACOSX and WINDOWS

   Follow instructions to run [LOIC](https://github.com/NewEraCracker/LOIC)
   
### Running LOIC on Kali

Since set-up can be tedious, follow the instructions below for running LOIC on Kali:

1. Download & extract Windows binaries: https://github.com/NewEraCracker/LOIC/releases

2. Install Mono -- More [info](http://www.mono-project.com/docs/getting-started/install/linux/)

     `sudo apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF`

     `echo "deb http://download.mono-project.com/repo/debian wheezy main" | sudo tee /etc/apt/sources.list.d/mono-xamarin.list`
     
     `sudo apt-get update`
     
     `sudo apt-get upgrade`
     
3. Install Packages -- More [info](http://www.mono-project.com/docs/getting-started/install/linux/#usage)

     `sudo apt-get install mono-devel`
     
     `sudo apt-get install mono-complete`
     
     `sudo apt-get install referenceassemblies-pcl`
     
     `sudo apt-get install ca-certificates-mono`
     
     `sudo apt-get install mono-xsp4`

4. Open terminal and type *mono /path_to_loic/debug/LOIC.exe*

5. LOIC will now run

## Raspbian Linux 

1. Download [Raspbian Linux](https://downloads.raspberrypi.org/raspbian_latest) 

2. Install [Raspberry Pi OS image on an SD card](https://www.raspberrypi.org/documentation/installation/installing-images/README.md)

3. Insert SD card in RPi & boot up

## Running a Local Server

1. Install NGINX

      `sudo apt-get install nginx`
      
2. NGINX usually starts after installation. Double check it's running

      `sudo netstat -an | grep LISTEN | grep :80`

## Add Target Website

1. Download "Wildlife Photography"

2. Add files to /var/www in NGINX in RPi
