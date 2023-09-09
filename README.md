# Image Upload and Capture App

Welcome to the Image Upload and Capture App repository! This project aims to create a versatile web application, Android, and iOS app using the Python Flask framework. With this app, users can easily upload images to the server and also capture photos using their device's camera, all while enjoying a seamless user experience.

## Features

### Image Upload
Users can effortlessly upload images from their device's storage to the app. This feature is perfect for sharing existing photos.

**Visit:** [Image Upload Page](https://flaskimagecaptureanduploaderapp.onrender.com/)

### Camera Capture
Want to snap a new photo? No problem! The app allows users to use their device camera to capture pictures instantly, and the captured image will automatically upload to the server, providing a dynamic and interactive experience.

**Visit:** [Camera Capture Page](https://flaskimagecaptureanduploaderapp.onrender.com/capture)

### Key-based Authentication System using JWT Token
Test the authentication system by making an HTTP POST request to [Login](https://flaskimagecaptureanduploaderapp.onrender.com/login) with a JSON body like this:

```json
{
    "username": "flaskApp",
    "password": "App@123"
}
```

This will return an access token or an authentication failed message in JSON format. You can then test the generated token by making an HTTP GET request to [Protected](https://flaskimagecaptureanduploaderapp.onrender.com/protected) with the header value:

```
'Authorization': '<your access token here>'
```

This will provide you with a JSON message like 'Access granted,' 'Token has expired,' or 'Invalid token' based on the access token.

### Set Your Access Limit
With Flask Limiter, you can easily apply rate limits. If the number of server hits exceeds your set limit, users cannot access the website until the set time passes. You can easily manage traffic on your server by setting limits such as "3 requests per minute," "60 requests per hour," or "200 requests per day."

*Note: At the root, there is a Python API script named "throttle_limit_test_script.py" to test the throttle limit.*

### Cross-Platform Compatibility
This project is designed to work seamlessly across multiple platforms, including web, Android, and iOS. Users can access the app on their preferred device.

## Installation

To get started with the Image Upload and Capture App, follow these installation instructions:

1. Clone the repository to your local machine.
2. Navigate to the project directory.
3. Install the required dependencies using `pip install -r requirements.txt`.
4. Open the terminal in the project folder and run the app using `python app.py`.
5. If prompted, use the password "App@123" for SSL, and make sure debugging is set to False.
6. Connect your device to the same Wi-Fi network.
7. In your browser, navigate to the address similar to (e.g., https://192.168.24.53:5000) shown in the terminal.

## Contact

If you have any questions or suggestions, please feel free to contact us at "ritabrata720@gmail.com".
