# Jason Holden's customizations for the ADV360-PRO-ZMK

## Review of the ADV360-PRO-ZMK

This keyboard is awesome, full stop.  But it can be even better.
As a full-time programmer, I find the default layout for locations of
control/alt/command keys hard to reach without awkward wrist movements.
You can find my customizations, ready to flash, in [releases](https://github.com/jasonkholden/Adv360-Pro-ZMK/tree/feature/jholden-mac/releases) 

## To build Firmware in GitHub Actions

### Setup

1. Fork this repo.
2. Enable GitHub Actions on your fork.

### Build firmware

1. Push a commit to trigger the build.
2. Download the artifact.

## Local building in a container

### Setup

#### Software

Either Podman or Docker is required, Podman is preferred if both are present.\
Make is also required

#### Windows specific
If compiling on Windows use WSL2 and Docker [Docker Setup Guide](https://docs.docker.com/desktop/windows/wsl/).\
Install make using `sudo apt-get install make`.\
The repository can be cloned directly into the WSL2 instance or accessed through the C: mount point WSL provides by default (`/mnt/c/path-to-repo`).

### Build firmware

1. Execute `make`.
2. Check the `firmware` directory for the latest firmware build.

### Cleanup

The built docker container and compiled firmware files can be deleted with `make clean`.

## Flashing firmware

Follow the programming instruction on page 8 of the [Quick Start Guide](https://kinesis-ergo.com/wp-content/uploads/Advantage360-Professional-QSG-v8-25-22.pdf) to flash the firmware.

## Other support

Further support resources can be found on Kinesis.com
https://kinesis-ergo.com/support/kb360pro/#firmware-updates
https://kinesis-ergo.com/support/kb360pro/#manuals
