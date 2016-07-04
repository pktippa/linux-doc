1. Upgrade kernel on Centos 7

   rpm --import https://www.elrepo.org/RPM-GPG-KEY-elrepo.org
   rpm -Uvh http://www.elrepo.org/elrepo-release-7.0-2.el7.elrepo.noarch.rpm
   yum --enablerepo=elrepo-kernel install kernel-ml
   
2. Selecting kernel from multiple version

   Centos 7
   grep '^menuentry' /boot/grub2/grub.cfg
   
   /etc/default/grub
   GRUB_DEFAULT=2
   
   grub2-mkconfig -o /boot/grub2/grub.cfg
   
   reboot