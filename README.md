# Information
* Project: Flight Controller Teensy 4.0
* Description: Design  PCB For Flight Controller System
* Author: Alifia Nuraini
* Date: 30 April 2026
  
# Komponen Utama
* **Microcontroller:** Teensy 4.0
* **Sensor IMU:** MPU 6050
* **Power Module:** UBEC 5V 3 A
* **Penggerak (aktuator):** 4x Servo MG90S & ESC_40A

#include <Wire.h>
#include <Servo.h>
#include <MPU6050.h>

MPU6050 (0X68);
MPU6050 (0X69);

const int pin_servo[] = {6,7,8,9};
const int pin_esc[] = {1,3,4,5};
const int pin_AD0[] = 18;

void setup();
Serial.begin ();
