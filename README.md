# Temperature_Based_Fan_Speed_Control
  # 🔹 Components Required
  Electronic Components:
  Arduino Uno – Microcontroller for processing temperature data
  
  DHT11 or DHT22 Sensor – Measures temperature and humidity
  
  DC Motor (Fan) – Represents the fan whose speed will be controlled
  
  L298N Motor Driver Module – Controls the speed and direction of the DC motor
  
  # Power Supply:
  5V (for Arduino & DHT11)
  
  12V (for L298N & DC Motor, if required)
  
  Jumper Wires & Breadboard – For circuit connections
  
  # Circuit Connections:
  1. Connecting the DHT11/DHT22 Sensor to Arduino:

        VCC of DHT11 → 5V on Arduino
     
        Data of DHT11 → Digital Pin 2 on Arduino

        GND of DHT11 → GND on Arduino
     
        A 10kΩ pull-up resistor is recommended between VCC and Data for stability.

  3. Connecting the L298N Motor Driver to Arduino:
     
        IN1 of L298N → Digital Pin 3 on Arduino
     
        IN2 of L298N → Digital Pin 4 on Arduino
     
        ENA (Enable A) of L298N → PWM Pin 5 on Arduino
     
        GND of L298N → GND on Arduino
     
        12V Power Input of L298N → 12V Power Source

  6. Connecting the DC Motor (Fan) to L298N:
     
        Motor Positive Terminal → OUT1 on L298N
     
        Motor Negative Terminal → OUT2 on L298N

  9. Powering the System:
      
        The Arduino can be powered via USB or an external 5V supply.
      
        The L298N motor driver needs a 12V power supply to drive the fan.

# 🔹 How it works
  The DHT11 sensor reads the ambient temperature.
  
  The Arduino processes the temperature data and generates a PWM signal for motor speed control.
  
  The L298N motor driver regulates the voltage to the DC motor based on the PWM input.
  
  The fan speed increases with rising temperature and decreases when the temperature drops.
  
  Would you like the Arduino code for this circuit? 🚀
