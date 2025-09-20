📚 Study Focus App

The Study Focus App helps students stay productive by using motion detection to discourage distractions.
It leverages the Arduino Nano 33 BLE Sense with Edge Impulse machine learning to monitor phone activity.

    ✅ Tracks focused study time while the phone is still.
    
    🚨 Triggers an alarm and pauses the timer when the phone is lifted.
    
    🔗 Uses Bluetooth Low Energy (BLE) for communication between Arduino and the smartphone app.
  
  
  

🔨 Project Overview

  How It Works

    Data Collection
    
    Gyroscope + accelerometer data captured from the Arduino Nano 33 BLE Sense.
    
    Edge Impulse used to label:
  
      📚 Still → Phone resting on table.
      
      📱 Moved → Phone lifted or rotated.

  Model Training
  
    ML model trained in Edge Impulse.
  
    Deployed back to Arduino as a C++ inference library.
    
  BLE Communication

    Arduino sends state (Still or Moved) to the smartphone app via BLE.
  
  App Logic
  
    Timer runs when state = Still.
    
    Alarm triggers + timer pauses when state = Moved.
    
    Study sessions logged for later review.
  


📦 Tech Stack

  Hardware: Arduino Nano 33 BLE Sense (built-in 9-axis IMU).
  
  Machine Learning: Edge Impulse SDK for motion classification.
  
  Connectivity: ArduinoBLE library for BLE communication.
  
  Smartphone App:
  
    Android 
    
    Cross-platform option: Flutter with BLE plugins.


📱 App Features

    Focus Timer – Tracks productive study time.
    
    Instant Alarm – Rings when the phone is picked up.
    
    Data Logging – Records total study hours + distractions.
  

🛠 Future Improvements

    Add screen lock detection.
    
    Implement cloud sync for study stats.
    
    AI-based distraction prediction.
    
    Gamification .  
