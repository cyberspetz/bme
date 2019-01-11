# BME sensor instruction

# formatting the SD card on rasperry
sudo dd bs=1m if=~/Downloads/raspbian-wheezy.img of=/dev/rdisk2

# the default raspberry password
raspberry

hostname: raspberrypi.local

# SSH access
ssh pi@raspberrypi.local

user: pi
pass: ...

# Running a remote server, all the scripts are in "/scripts" folder 

# added following line to bashrc
sudo python3 /home/pi/bme/scripts/bme280_sensor.py [dbname] [access_code] &
