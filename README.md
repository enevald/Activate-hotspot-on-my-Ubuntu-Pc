# Activate-hotspot-on-my-Ubuntu-Pc

sudo nmcli device set ap0 managed no
sudo ip link set ap0 down
sudo iw dev ap0 set type __ap
sudo ip link set ap0 up
sudo nmcli device set ap0 managed yes
sudo nmcli connection up uuid df1509a0-d925-41e5-922d-5adccbacb4e8 ifname ap0
