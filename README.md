# QR-Recognition-3D-Model-AR-Web-Viewer
This project is a mobile-responsive web application that utilizes augmented reality (AR) technology to load 3D models in glTF format (.glb) when an image or QR code is recognized. The 3D model is displayed in augmented reality (AR) on a specified point of an object.

Features
QR Code Recognition: The app scans QR codes or markers to trigger AR model loading.
AR Viewer: Displays the 3D model in augmented reality using the browser camera (no need for additional apps or devices).
Error Handling: If recognition fails or an incorrect URL is provided, an error message is shown and disappears after 2 seconds.
Mobile Responsive: The web app is designed to work on Android and iOS devices (Safari, Chrome).
Loading glTF Models: Supports loading glTF models (.glb) from a provided URL.
Project Scope
Technology Stack:
Frontend: React, HTML, CSS, JavaScript
AR Technology: AR.js, Three.js, A-Frame
QR Code Scanning: Using html5-qrcode or similar libraries
Responsive Design: CSS Media Queries for both portrait and landscape orientations
Supported Browsers: Android Web (Chrome), iOS Safari
Features and Flow
QR Code Recognition:

The web application scans the user's QR code using the camera.
If successful, it extracts the URL of a 3D model.
Model Loading in AR:

Upon successful QR code recognition, the application loads a 3D model in AR on the detected marker.
You can customize the model URL for specific scenarios.
Error Handling:

If the QR code recognition fails or contains an invalid URL, an error message (toast) is shown for 2 seconds.
Setup Instructions
Follow the steps below to run the project locally:

Prerequisites
Make sure you have Node.js and npm installed.

Installation
Clone the repository:

bash
Copy code
git clone https://github.com/your-username/qr-recognition-ar-web-viewer.git
cd qr-recognition-ar-web-viewer
Install dependencies:

bash
Copy code
npm install
Running the App
To run the app locally, use the following command:

bash
Copy code
npm start
This will start the development server and you can open the app in your browser at http://localhost:3000. The application should be accessible on mobile devices, and it will request camera access for QR code scanning.

Supported Browsers
The app is designed to work on mobile web browsers, specifically:

Chrome (Android)
Safari (iOS)
Make sure the camera permissions are granted for the app to function properly.

How to Test
Generate a QR code containing one of the following URLs:

https://jhjin-common.s3.ap-southeast-2.amazonaws.com/glbSample/sample_1.glb
https://jhjin-common.s3.ap-southeast-2.amazonaws.com/glbSample/sample_2.glb
Scan the QR code using the app, and the 3D model should appear in augmented reality.

Key Libraries Used
AR.js: A lightweight library to enable AR capabilities in web applications.
A-Frame: Web framework for building virtual and augmented reality experiences.
html5-qrcode: A library for QR code scanning within the browser.
Three.js: Used to render 3D models in the AR environment.
Project Structure
public/: Contains static files like index.html.
src/: The main source code for the app.
App.js: Main React component that handles QR recognition and AR functionality.
App.css: Styling for the app, including responsive design and toast notifications.
index.js: Entry point for the React application.
Troubleshooting
QR Code Not Detected:

Ensure that the QR code is clear and well-lit. If scanning fails, try adjusting the angle or distance.
AR Model Not Displaying:

Make sure the URL in the QR code points to a valid .glb file.
Browser Compatibility:

AR features work best in Chrome (Android) and Safari (iOS). Ensure that the mobile device has a compatible browser version.
Future Enhancements
Support for multiple types of markers or images (not just QR codes).
Integration with more 3D models or content from external sources.
Advanced error handling and notifications.
