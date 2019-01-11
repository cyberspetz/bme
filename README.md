# The code here is for BME280 sensor and runs and I'ma running it on 2 nodes: 
1. Raspberry pi using python setup (wired through lan)
2. NodeMCU wifi and Adafruit library on address 0x76 (wireless)

# Here are libraries to written with help of coralysis articles https://corlysis.com/docs/tutorials/external_posts/



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
