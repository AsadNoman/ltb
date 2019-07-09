# ltb
Simple linux kernel build and toybox build in 10MB

tested only on qemu (qemu-system-x86_64)

---

1. install qemu on your linux system.
*. for ubuntu/debian
```
sudo apt-get install qemu
```
*. for arch based
```
sudo pacman -S qemu
```
2. clone this repo.
```
git clone https://github.com/AsadNoman/ltb.git
```
3. go to tlb directory
```
cd ltb
```
4. run
```
qemu-system-x86_64 -kernel boot/bzImage -initrd troot.cpio.gz -append "panic=10  rdinit=/bin/sh"
```
and boom.
