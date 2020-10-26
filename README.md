# Firebase-Server
Many times we need to manage servers, write APIs, data-store management, etc. This project can be used to display the temperature and humidity values from DHT11 sensor, by using Firebase server.Firebase is a Backend as a Service(Baas).It is a most preferred backend for Iot based applications. It is a platform, not just a database. Firebase is Google’s mobile application development platform that helps you build, improve, and grow your app. Firebase is a technology that allows you to create web applications without server-side programming, making development faster and easier. It supports Web, iOS, OS X and Android clients. 
Apps that use Firebase can use and control data without thinking about how data is stored and synchronized across different instances of the application in real-time.
The ESP8266 (Node MCU) is an open source Iot platform are becoming more popular with Makers due to a low cost and a powerful, programmable microcontroller SOC-board.
DHT series digital temperature and humidity sensors and we have a project that may literally be deployed anywhere to broadcast sensor data.This project demonstrates the programming of the ESP8266 (-12E) module with the Arduino IDE and interfacing with a DHT temperature/humidity sensor.  Using other sensors and their corresponding libraries, other electronics may be interfaced with the ESP8266 and monitored via wifi. It display the temperature and humidity values from the DHT11 sensor.  Node MCU will read the temperature and humidity data from the DHT11 sensor and display it on the Firebase Real-time database. 

Here the Firebase Cloud Function issues the timestamp when a value is pushed to the Firebase Real-time Database.  Firebase Cloud Functions(or “Cloud Functions for Firebase”) are part of Google Cloud Platform and are functions executed in a Node Environment on Google servers. A Firebase Cloud Function can be: called from an app involving Firebase (directly or via a HTTP request),automatically triggered upon an event on Firebase products:
Writing cloud functions- before write this functions, first we create/host an web-app, after that we deploy functions.
Firebase Hosting is a secure, global web hosting CDN (Content Delivery Network). It’s really good at quickly delivering static content (HTML,CSS, JS, images) using servers that are close to your users. And you can get it set up quickly, with or without your custom domain, along with a provisioned SSL certificate that costs you nothing.  Firebase Hosting has one important point of integration with the rest of Firebase, and that’s through Cloud Functions. Firebase Hosting lets you proxy the request and response to and from Cloud Functions when writing HTTP type functions. And, even better, it’ll cache the responses from your functions, if you configure them properly.
The aim of our project is to make a Wi-Fi module which can sense the temperature and humidity values and display the values  to the frontend html images, using servers and store into the firebase Real time database. So this whole process is operated automatically by its sensors.

## Project initialization
1. ![Slide5](https://user-images.githubusercontent.com/68738766/90042173-f12c7480-dce7-11ea-8cf9-cfa732920456.JPG)
2. ![Slide6](https://user-images.githubusercontent.com/68738766/90042178-f4276500-dce7-11ea-9fb1-596abb3b731c.JPG)
3. ![Slide8](https://user-images.githubusercontent.com/68738766/90042195-fdb0cd00-dce7-11ea-82f6-25e5052dc248.JPG)
4. ![Slide9](https://user-images.githubusercontent.com/68738766/90042201-00132700-dce8-11ea-956f-c9cb9320bb00.JPG)
5. ![Slide10](https://user-images.githubusercontent.com/68738766/90042208-030e1780-dce8-11ea-8a27-9b7fe54a819b.JPG)
## Commands to access firebase console
1. Once you install the node.js as well as npm, you can write on cmd prompt-” npm install-g firebase-tools”
2. To initialize the firebase project, type- “firebase login” & “firebase init”
3. Once you initialize, now deploy your firebase project- “firebase deploy --only hosting”& “firebase deploy  -- only functions”
4. Once we deploy the hosting & functions, your website or(web-page)is automatically triggered to the cloud functions and firebase Real- time database.
5. push this object to our Firebase Real time Database using the function:
6. String push(constString &path, constJsonVariant&value)
7. We have to create this function with .js  file extension and deploy the functions using cmd- “firebase deploy - - only functions
8. ![index](https://user-images.githubusercontent.com/68738766/90042280-191bd800-dce8-11ea-9bc2-11ab5e74ff5c.png)
## Hosting Web app  
![newplot](https://user-images.githubusercontent.com/68738766/90042494-626c2780-dce8-11ea-8a0c-610864e31236.png)
### Link https://nodemcu-nielit125.firebaseapp.com/
