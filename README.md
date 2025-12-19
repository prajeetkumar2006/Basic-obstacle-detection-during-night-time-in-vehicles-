# Basic-obstacle-detection-during-night-time-in-vehicles-
# Introduction
  Obstacle detection at night in vehicles enhances road safety by using sensors like infrared, LiDAR, ultrasonic, or cameras to detect objects in low-light conditions. These systems help prevent collisions by      
  alerting drivers or enabling autonomous braking.

# Components requried
  1. Ultrasonic Sensor X 1
  2. LCD X 1
  3. Gear Motors X 2
  4. Motor Driver (L298) X 1
  5. 12V Battery X 1
  6. LDR X 1
  7. Arduino X 1

 #Working
  The ultrasonic Sensor is used to find if any obstacle is detected from a long range as well as measures the distance between the source and the obstacle and the distance is sent to LCD for the user to see. 
  A LDR(Light Detection Ranging) is used to detect if it is day or night.
  
  # During Day Time
  The driver is alerted only through the LCD by displaying the distance and some special messages 
    
  # During Night Time
   Arduino does the same task as the day time but here when the obstacle is too close (for this project it is 10cm) brakes are applied using to stop the vehicle. 
    
# Appling Brakes
  We can't connect motors directly in the GPIO of an arduino and set either of the motors pins to HIGH and LOW, if we, it damages the microcontroller because GPIO pin of an arduino can supply only 40mA
  but a DC motor need 500mA to power up. As we connect motors to GPIO motors draws more current than the limit of the GPIO pins leads to the damage so, to solve this motor drivers are used.

  
  
    
   
    
  
  
