# LVM-shpora
# Посмотреть logical volume:
sudo lvdisplay /dev/ubuntu-vg/ubuntu-lv 
# Посмотреть volume group:
sudo vgdisplay /dev/ubuntu-vg 
# Посмотреть сколько места занимает ФС:
df -Th /
# Расширить logical volume на все свободное место которое есть в VG:
sudo lvextend -l+100%FREE /dev/ubuntu-vg/ubuntu-lv 
# Расширить ФС:
sudo resize2fs /dev/ubuntu-vg/ubuntu-lv 
