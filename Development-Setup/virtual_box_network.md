Virtual Box Network Setup



1. Click Virtual Box > Preferences > Network > Host-only Networks
2. Add one host-only network:
  ipv4: 192.168.56.1
  ipv4 network mask: 255.255.255.0
  ipv6: blank
  ipv6 network mask length: 0
  disable DHCP server.
3. Select the virtual machine, then open the settings.
  Choose Network: 
  Enable Network Adapter 1, attached to Host-only Adapter and select vboxnet1 (the one we just created in step 2)
  Enable Network Adapter 2, attached to NAT
  save settings
4. start virtual machine.
  Open file `/etc/network/interfaces`
  Change it to:
  ```
  # This file describes the network interfaces available on your system
  # and how to activate them. For more information, see interfaces(5).

  # The loopback network interface
  auto lo
  iface lo inet loopback

  # The primary network: local virtualbox network
  auto eth0
  iface eth0 inet static
  address 192.168.56.10
  network 192.168.56.0
  netmask 255.255.255.0

  # The secondary network interface (NAT)
  auto eth1
  iface eth1 inet dhcp
  ```

5. Reboot VM and from your laptop you can ping 192.168.56.10
Repeat above step: 3 ~ 5 for other VMs.
You will have a group of VM setting on that virtual network.
They communicate to each other through virtual network and talk to internet through NAT.
Better for performance and easier to setup.

