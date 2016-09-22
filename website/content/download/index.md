---
date: 2016-03-09T00:11:02+01:00
title: Download
weight: 10
---

NOTE: Only the Tango Top data is online thus far, we are still looking for large enough disk space to host the entire set. Should happen any day.

## Preparing for Download

The installation instructions and scripts have been tested on Ubuntu 14.04. Porting the scripts to any unix-like operating system should be straight forward. The Windows OS is not supported, but we provide raw download links so you can piece the data together yourself.

The full data set, without the frames extracted, has a size of about 25GB. If frames are extracted for all cameras and all sequences, the total size balloons to more than 100GB, so having some head room is definitely a good idea. For most purposes, 50GB should be more than enough spacce.

## Running the Installer

The install scripts are in the "master" branch of the
github repository, and can be run like this (you may need to install
`git` if it's not on your machine yet, using `sudo apt-get install git`):

```
git clone https://github.com/daniilidis-group/penncosyvio.git
cd penncosyvio/tools
./download.bash 
================ PENNCOSYVIO INSTALLER ======================
------------ select sensor to download:
1) GoPro C1		  4) Tango Bottom	    7) Intrinsic Calibration
2) GoPro C2		  5) Tango Top		    8) Extrinsic Calibration
3) GoPro C3		  6) VI Sensor		    9) Quit
enter your choice: 
```

Pick the sensors that you are interested in and download the
data. Once you quit out of the installer tool, change into the parent
directory and have a look. This is how it looks if you downloaded only
the `Tango Top` data:

```
cd ..
ls
README.md  tango_top  tools
```

