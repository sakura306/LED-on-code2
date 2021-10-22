# LED-on-code2
import RPi.GPIO as GPIO
import time

LedGpio=18
waitTime=1

GPIO.setwarnings(False)
GPIO.setmode(GPIO.BCM)
GPIO.setup(LedGpio,GPIO.OUT)

GPIO.output(LedGpio,True)
time.sleep(waitTime)
GPIO.output(LedGpio,False)

GPIO.cleanup()

