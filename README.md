make clean
make
sudo mv /lib/modules/$(uname -r)/kernel/drivers/bluetooth/btusb.ko /lib/modules/$(uname -r)/kernel/drivers/bluetooth/btusb.ko.bak
sudo cp btusb.ko /lib/modules/$(uname -r)/kernel/drivers/bluetooth/
sudo depmod -a
