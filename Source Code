import RPi.GPIO as GPIO
import time

# Configure GPIO
GPIO.setmode(GPIO.BCM)
GPIO.setwarnings(False)

# Ultrasonic sensor pins
TRIG = 23
ECHO = 24

# Water level sensor pin
LEVEL_SENSOR_PIN = 25

GPIO.setup(TRIG, GPIO.OUT)
GPIO.setup(ECHO, GPIO.IN)
GPIO.setup(LEVEL_SENSOR_PIN, GPIO.IN)

def measure_distance():
    # Send a pulse
    GPIO.output(TRIG, GPIO.LOW)
    time.sleep(0.5)
    GPIO.output(TRIG, GPIO.HIGH)
    time.sleep(0.00001)
    GPIO.output(TRIG, GPIO.LOW)

    # Measure the time of the pulse
    while GPIO.input(ECHO) == GPIO.LOW:
        pulse_start = time.time()
    while GPIO.input(ECHO) == GPIO.HIGH:
        pulse_end = time.time()

    pulse_duration = pulse_end - pulse_start
    distance = pulse_duration * 34300 / 2  # Speed of sound in cm/s

    return distance

def water_level_status():
    # Read the status of the water level sensor
    return GPIO.input(LEVEL_SENSOR_PIN)

try:
    while True:
        dist = measure_distance()
        level_status = water_level_status()

        print(f"Distance: {dist:.2f} cm")
        if level_status == GPIO.HIGH:
            print("Water level detected")
        else:
            print("Water level not detected")

        time.sleep(1)

except KeyboardInterrupt:
    print("Program interrupted")

finally:
    GPIO.cleanup()
