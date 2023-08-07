# Debian Autoinstall

This repository contains my configuration management for personal Debian installations. 

For more documentation on how to install Debian click [here](https://www.debian.org/releases/stable/installmanual).

## Installation Steps

### Download and Verify ISO

1. Download the `download-and-verify-iso` script. This script will download and verify the latest Debian stable ISO.
1. Run the script
`$ ./download-and-verify-iso`.
1. Check the output to verify the ISO signature and checksum.
1. Prepare an installation medium (e.g. USB flash drive).
`# cp <debian_version>.iso /dev/<device_name> && sync`. 

### Debian Install

1. Boot the live environment.
1. In the main boot menu select `Advanced options...` >> `... Automated install`.
1. Enter the URL or location of the preseed file you want to use (e.g. https://github.com/mlukina/debian-autoinstall/workstation-preseed.cfg).

### Post Install

1. Run ansible configuration.
