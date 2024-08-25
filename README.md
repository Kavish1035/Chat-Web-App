Firebase Chat Application
This is a simple web-based chat application built using Firebase as the backend. The application allows users to send and
receive messages in real-time, with different colors for messages sent by the sender and the receiver.

Features
  Real-time Messaging: Messages are instantly sent and received using Firebase Realtime Database.
  Message Colors: Messages sent by the sender and receiver are displayed in different colors for better visual distinction.
  Username Persistence: Usernames are stored in the browser's local storage, ensuring a personalized experience.
  Responsive Design: The chat window is designed to be responsive and user-friendly.
Technologies Used
  HTML for the structure of the web pages.
  CSS for styling the chat interface.
  JavaScript for dynamic content and interactions.
  Firebase for real-time database functionality.
Getting Started
  Follow these steps to set up and run the project on your local machine:

Prerequisites
  A modern web browser (e.g., Chrome, Firefox, Safari).
  Firebase project setup with Realtime Database enabled.
  Installation

Clone the Repository:

  bash
  Copy code
  git clone (https://github.com/Kavish1035/Chat-Web-App)
  cd firebase-chat-app
Set Up Firebase:
  Go to the Firebase Console.
  Create a new project.
  Enable Realtime Database in your Firebase project.
  Get your Firebase configuration details (API key, Auth domain, Database URL, etc.).

Update Firebase Configuration:

  Replace the firebaseConfig object in the code with your own Firebase project configuration:
  javascript
Copy code
  const firebaseConfig = {
      apiKey: "YOUR_API_KEY",
      authDomain: "YOUR_AUTH_DOMAIN",
      databaseURL: "YOUR_DATABASE_URL",
      projectId: "YOUR_PROJECT_ID",
      storageBucket: "YOUR_STORAGE_BUCKET",
      messagingSenderId: "YOUR_MESSAGING_SENDER_ID",
      appId: "YOUR_APP_ID",
  };
Open index.html in Your Browser:

Simply open the index.html file in your browser to start the chat application.
Usage
When the page loads, you will be prompted to enter your username.
Type your messages in the input field and click the "Send" button or press "Enter" to send the message.
Messages sent by you will appear on the right side of the chat window, with a specific background color.
Messages received from others will appear on the left side of the chat window, with a different background color.
Code Overview
index.html
HTML Structure: Defines the chat window, input field, and send button.
CSS: Provides styling for the chat window, message bubbles, scrollbar, and button hover effects.
app.js
Firebase Initialization: Connects to Firebase and initializes the Realtime Database.
Real-time Messaging: Listens for new messages in the database and updates the chat window in real-time.
Message Sending: Sends a new message to the database with the user's username and a timestamp.
Color Management: Distinguishes messages sent by the current user and others with different background colors.
Customization
Message Colors: You can customize the colors used for messages sent by the sender and receiver by modifying the openChat and sendMessage functions in the JavaScript code.
User Interface: Modify the CSS to change the appearance of the chat window, buttons, and other elements to fit your design preferences.
Contributing
Contributions are welcome! If you have suggestions or improvements, feel free to create a pull request or open an issue.

License
This project is licensed under the MIT License. See the LICENSE file for more information.

Acknowledgements
Special thanks to Firebase for providing a powerful real-time database solution.
