

'''
wifis:
  wlan0:
    dhcp4: true
    optional: true
    access-points:
      ChinaNet-QmqN:
        password: "sava"
#      myworkwifi:
'''

sudo nano /etc/netplan/50-cloud-init.yaml

$ sudo netplan apply

$ sudo netplan --debug apply

ip a
