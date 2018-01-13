# Asus N53 PCI Driver for Linux Kernel 4.13-Ubuntu-16.04LTS
Asus N53 PCI RT5592STA Driver for Linux Kernel 4.13-Ubuntu-16.04LTS

Forked from https://github.com/kuttor and altered to compile correctly for kernel 4.13.x

### Installation
- sudo git clone  /op://github.com/elock37/Asus-N53-PCU-RT5592STA-Driver-for-Linux-Kernel-4.6-Ubuntu-16.10t/asus-n53-driver
- cd /opt/asus-n53-driver
- sudo make
- sudo make install
- sudo modprobe rt5592sta

### Troubleshooting
- I had to bring the wireless interface down and up and then restart NetworkManager. 
1. sudo ip link set 'link_name' down
2. sudo ip link set 'link_name' up
3. sudo systemctl restart NetworkManager

