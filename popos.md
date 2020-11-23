# Pop_OS! 20.10 - This & That

## Graphic Shenanigans

The Pop_OS! build in AMD driver, doesn't play nicely with Steam / Proton for an RX580 - Basically nothing works

### Installing the AMD Driver from the website
*Apparently driver `amdgpu-pro-20.45-1164792-ubuntu-20.04` doesn't work with the installed 5.8.0-7630 kernel - This is only to not forget how to install it, if a working driver is released*

1. Download driver from the [AMD Website](https://www.amd.com/en/support/graphics/radeon-500-series/radeon-rx-500-series/radeon-rx-580) 
2. Change release info via: Manually edit `/etc/os-release` (e.g. `sudo nano /etc/os-release)`, change `ID=pop` to `ID=ubuntu`.
3. Extract the downloaded driver and navigate to the according directory
4. Install driver via `amdgpu-install -y --no-dkms --opencl=legacy`
5. Revert release info 

If their is an error message roll back via:

1. `amdgpu-uninstall`
2. >sudo rm /etc/modprobe.d/blacklist-amdgpu.conf
3. >sudo update-initramfs -u -k all

If there is need to roll back the rollback: 
> echo 'blacklist amdgpu' | sudo tee /etc/modprobe.d/blacklist-amdgpu.conf
> sudo update-initramfs -u -k all
