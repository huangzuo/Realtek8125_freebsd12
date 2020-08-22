# Realtek8125_freebsd12
#Realtek 8125 for Driver FreeBSD 12.1
1. Copy if_re.ko to /boot/kernel/ 
2. In /boot/kernel  
chown root:wheel if_re.ko  
chmod 0555 if_re.ko
3. Add the following line to /boot/loader.conf  
if_re_load="YES"
4. It is a good idea to test before reboot:  
kldload /boot/kernel/if_re.ko
5. reboot

