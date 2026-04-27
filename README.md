# nvsleep
simple script to make nvidia GPUs sleep on linux

## Install

### Requirements: 
- Nvidia GPU
- nvidia.NVreg_DynamicPowerManagement=0x02 set in either grub or udev rules
- DE/WM not running on the dGPU
- nvidia or nvidia-open drivers (not nova or nouveau)

Download the [latest release](https://github.com/C0C0B01/nvsleep/releases/latest)

Then prefereably move the file elsewhere then /Downloads and use any method of running it (WM config, bash config, runit, ect)

## Why is this a thing?
some nvidia GPUs dont support D3cold, meaning they just sit there sucking power even when not in use, this script forces it into D3cold until used again
