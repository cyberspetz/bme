# bme

# formatting the SD card
sudo dd bs=1m if=~/Downloads/2015-02-16-raspbian-wheezy.img of=/dev/rdisk2

the default raspberry pass: raspberry

hostname: raspberrypi.local

# SSH access
ssh pi@raspberrypi.local

user: pi
pass: ...

# Running a remote server
# folder
cd scripts 

# added following line to bashrc
sudo python3 /home/pi/bme/scripts/bme280_sensor.py [dbname] [access_code] &
