iface eth0 inet manual
allow-hotplug wlan0
iface wlan0 inet static
    address 192.168.1.50
    netmask 255.255.255.0
    gateway 192.168.1.1
    wpa-ssid "pukpik"
    wpa-psk "ecc807807"
    #wpa-conf /etc/wpa_supplicant/wpa_supplicant.conf
    
    
