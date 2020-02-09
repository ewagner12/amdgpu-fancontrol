# amdgpu-fancontrol

Simple bash script to control AMD Radeon graphics cards fan pwm. Adjust temp/pwm values and hysteresis/interval in the script as desired. Other adjustments, such as the correct hwmon path might be required as well.

This script was initially meant as an example. Please don't just run it naively and keep in mind that I'm not responsible for failures.

To enable on startup, from download directory:
```
sudo mv amdgpu-fancontrol /usr/bin/
sudo mv amdgpu-fancontrol.service /etc/systemd/system/
systemctl enable amdgpu-fancontrol
```

## Packages

- Arch Linux (on AUR): https://aur.archlinux.org/packages/amdgpu-fancontrol-git/
