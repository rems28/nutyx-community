# nutyx-community
Community collection for nutyx distribution.
To enable the collection, please add to your /etc/cards.conf the following lines

```
## For community
# Comment following line
#if you don't want to install community
dir /var/lib/pkg/depot/community
dir /var/lib/pkg/depot/community-extra
```
```
Instructions for Kernel-414 and Nvidia-340
sudo -i

vi /boot/grub/grub.cfg or 

nano /boot/grub/grub.cfg if nano is installed

Create a new menuentry with the new kernel 4.14.
Replace the /boot/kernel-lts by /boot/kernel-414 in the linux line at the end of the menuentry

Save the file

Install kernel-414, kernel-414-nvidia-340, nvidia 340 packages

Make sure that kernel file is kernel-4.14.*-YaoLinuX-414 in /boot and be sure that is a file and not a symbolic link.
Make sure the kernel-414 is created in /boot and is a symbolic link to kernel-4.14.*-YaoLinuX-414 in /boot
 ```
