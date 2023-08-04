# Debian Autoinstall

This repository contains configuration management for personal Debian installations. 

For more documentation about how to install Debian click [here](https://www.debian.org/releases/stable/installmanual).

## How to Install

### Download and Verify ISO

1. Download the `download-and-verify-iso` script.
1. Check for new releases of Debian and adjust the debianVersion variable if necessary.
1. Run the script
`$ ./download-and-verify-iso`.
1. Check the output to verify the ISO signature and checksum.
1. Prepare an installation medium (e.g. USB flash drive).
`# cp <debian_version>.iso /dev/<device_name> && sync`. 

### Debian Install

1. Boot the live environment.
1. In the main boot menu select `Advanced options...` >> `... Automated install`.
1. Enter the URL or location of the preseed file you want to use (e.g. https://github.com/mlukina/debian-autoinstall/preseed.cfg).

### Post Install

1. Run ansible configuration.
