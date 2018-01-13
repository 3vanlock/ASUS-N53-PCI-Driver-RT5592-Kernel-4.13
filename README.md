# Asus N53 PCI Driver for Linux Kernel 4.13 on Ubuntu-16.04LTS
Asus N53 PCI RT5592STA Driver for Linux Kernel 4.13 on Ubuntu-16.04LTS

Forked from https://github.com/kuttor/Asus-N53-PCU-RT5592STA-Driver-for-Linux-Kernel-4.6-Ubuntu-16.10 and altered to compile correctly for kernel 4.13.x

### Installation
    sudo git clone https://github.com/elock37/ASUS-N53-PCI-Driver-RT5592-Kernel-4.13 /opt/asus-n53-driver 
    cd /opt/asus-n53-driver
    sudo make
    sudo make install
    sudo modprobe rt5592sta

### Cycle network interface and restart NetworkManager 
    sudo ip link set 'link_name' down
    sudo ip link set 'link_name' up
    sudo systemctl restart NetworkManager

