# SMART-IOT-SYSTEM-FOR-LEAFY-VEGETABLE-STORAGE_iot
# Smart IoT System for Leafy Vegetable Storage

## 📌 Project Overview
This project presents an IoT-based smart storage monitoring system designed to maintain optimal environmental conditions for leafy vegetables. The system continuously monitors temperature, humidity, and motion inside a storage area and sends real-time data to a cloud platform for visualization and decision-making.

## 🎯 Objectives
- Monitor temperature and humidity inside the vegetable storage area  
- Detect motion during non-working hours  
- Send real-time sensor data to a cloud platform  
- Visualize data using an online dashboard  
- Trigger automatic alerts under abnormal conditions  

## 🛠️ System Architecture
Environmental sensors are connected to an ESP32 microcontroller. Sensor readings are transmitted via WiFi to the ThingSpeak cloud platform using HTTP requests. Threshold-based decision logic is applied to activate alerts such as LED and buzzer when abnormal conditions are detected.

## ⚙️ Hardware Components
- ESP32 Microcontroller  
- DHT11 Temperature & Humidity Sensor  
- PIR Motion Sensor  
- LED  
- Buzzer  

## 💻 Software & Tools
- Arduino IDE  
- ThingSpeak Cloud Platform  
- Wokwi Simulator  
- Programming Language: Arduino (C/C++)  

## ☁️ Cloud & Data Pipeline
Sensor data is uploaded to ThingSpeak for real-time visualization and analysis.
- Field 1: Temperature (°C)  
- Field 2: Humidity (%)  
- Field 3: Motion Status (0 / 1)  

## 📊 Analytics & Decision Logic
The system applies threshold-based analytics:
- If temperature > 30°C → Alert activated  
- If humidity > 80% → Alert activated  
- If motion is detected between 12:00 AM and 6:00 AM → Alert activated  

## ✅ Results
- Real-time sensor data successfully uploaded to the cloud  
- Live visualization achieved using ThingSpeak dashboards  
- Alert system responded correctly to abnormal conditions  
- System performed reliably during testing  

## 🔐 Security & Privacy
- Cloud communication secured using a private API key  
- No personal or sensitive data is collected  
- Only environmental and motion data is transmitted  

## 🚀 Future Enhancements
- Mobile notifications  
- Machine learning-based spoilage prediction  
- Additional sensors such as gas or air quality sensors  

## 📚 References
Relevant IoT, cloud computing, and smart agriculture literature and online documentation.
