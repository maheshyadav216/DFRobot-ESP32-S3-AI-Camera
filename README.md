# ANPR-using-DFRobot-ESP32S3-AI-Camera-Module
ANPR-using-DFRobot-ESP32S3-AI-Camera-Module  
  
<img src="/Images/mah216-hack-thumb.png" height="400">
  
In this project, the ESP32-S3 AI camera captures an image of a vehicle and converts it into a Base64-encoded string, which is then embedded into a JSON payload along with a natural language prompt requesting number plate extraction. This payload is sent via an HTTP POST request to Google's Gemini API (generateContent endpoint). The Gemini API processes the image and returns a JSON-formatted response, where the extracted number plate (or a relevant message) is found within a nested text field. The ESP32 then parses this JSON response using ArduinoJson, extracts the plain-text number plate, and—if valid—logs it or sends it to Firebase for storage and further monitoring.  
<br>
<br>

## DFRobot's ESP32-S3 AI Camera Module  
<img src="/Images/DF-Esp32S3.jpg" height="200">
  
The **ESP32-S3 AI Camera** is a cutting-edge intelligent camera module built around the high-performance ESP32-S3 chip, designed for efficient video processing, edge AI, and voice interaction. Featuring a wide-angle infrared camera, onboard microphone, and speaker, it is ideally suited for applications such as electronic peepholes, baby monitors, and license plate recognition.  
  
  
## Documentation

Refer the [Project Blog on Hackster](https://www.hackster.io/maheshyadav216/ai-powered-anpr-using-dfrobot-s-esp32-s3-ai-cam-gemini-api-74d458) for more information.  

**Hardware**
- [ESP32-S3 AI Camera Module](https://www.dfrobot.com/product-2899.html)  
  
**Software**
- Arduino  
    [Wiki Page for Info](https://wiki.dfrobot.com/SKU_DFR1154_ESP32_S3_AI_CAM)  
    [ESP32-S3 AI Camera Module Demo](https://dfimg.dfrobot.com/enshop/20250331/dfr1154-en.mp4)  
  
------------------------------------------------------------------------------------------------------

📕 **YouTube Video Links**  

▶️  [DIY Project] AI Powered ANPR System 🔗  https://youtu.be/jt6_WuvNuSQ   
  
-------------------------------------------------------------------------------------------------------
📒 **Important Links**  
 
🌐 DFRobot - 🔗 https://www.dfrobot.com  
📒 ESP32-S3 AI Camera Module 🔗 https://docs.m5stack.com/en/core/AtomS3  
🔑 Get Gemini API Key 🔗 https://aistudio.google.com/app/apikey  
⚙️ Firebase Database Console 🔗 https://console.firebase.google.com/  

🛒 Hardware Purchase Links -
[ESP32-S3 AI Camera Module]  🔗 https://www.dfrobot.com/product-2899.html
   
------------------------------------------------------------------------------------------------------

📜 Source Code, Circuit Diagrams and Documentation : 

🌐 GitHub Repository - 🔗 https://github.com/maheshyadav216/ANPR-using-DFRobot-ESP32S3-AI-Camera-Module    
  
🌐 Hackster Blog - 🔗 https://www.hackster.io/maheshyadav216/ai-powered-anpr-using-dfrobot-s-esp32-s3-ai-cam-gemini-api-74d458  
  
------------------------------------------------------------------------------------------  

Shield: [![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa]

This work is licensed under a
[Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License][cc-by-nc-sa].

[![CC BY-NC-SA 4.0][cc-by-nc-sa-image]][cc-by-nc-sa]

[cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-sa/4.0/
[cc-by-nc-sa-image]: https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png
[cc-by-nc-sa-shield]: https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg
