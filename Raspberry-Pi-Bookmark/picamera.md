https://www.raspberrypi.org/learning/getting-started-with-picamera/worksheet/

from picamera import PiCamera
from time import sleep

camera = PiCamera()

camera.start_preview()
sleep(10)
camera.stop_preview()

camera.rotation = 180
camera.start_preview()
sleep(10)
camera.stop_preview()

camera.start_preview()
sleep(5)
camera.capture('/home/pi/Desktop/image.jpg')
camera.stop_preview()

--------------------------------------------

สั่งถ่ายภาพ

raspistill -v -o test.jpg
raspivid -o filename.h264 -t 20000

sudo apt-get install python3-picamera

convert h264 to mp4
sudo apt-get install gpac
MP4Box -add filename.h264 filename.mp4
