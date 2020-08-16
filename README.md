# General
Virtualización con KVM

En la carpeta resources se encuentran:
* La presentación utilizada en el live
*  El cheat sheet de KVM

[Vídeo del live](https://www.youtube.com/watch?v=1ZH9ok_Sbh0 "Virtualización con KVM")

# Comandos utilizados en el live

## Crear una máquina virtual
```sh
sudo virt-install --connect=qemu:///system --name=debianTest --ram=512 --vcpus=2 --check-cpu --os-variant debian10 --hvm --vnc --accelerate --disk=/home/proyectosbeta/debianPrueba.img,size=8,sparse=true --cdrom=/var/lib/libvirt/images/ISOs/debian-10.4.0-amd64-netinst.iso
```

## Listar todas las máquinas virtuales
```sh
sudo virsh list --all
```

# Herramientas útiles:
```sh
  osinfo-query os | grep debian
```
