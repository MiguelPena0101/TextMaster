
# TextMaster

## Table of Contents
- [Description](#description)
- [Installation](#installation)
- [Usage](#usage)
- [Features](#features)
- [Technologies Used](#technologies-used)

## Description
**TextMaster** is a Progressive Web Application (PWA) designed to provide a powerful text editor that can be used both online and offline. Whether you are creating notes or writing code snippets, TextMaster allows you to store your content seamlessly in IndexedDB and access it even without an internet connection. It also provides the functionality to install the application locally on your device for quick and easy access.

## Installation
To install and run TextMaster locally, follow these steps:

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/textmaster.git
   cd textmaster
   ```

2. **Install Dependencies**: Run the following command from the root directory to install the server-side and client-side dependencies:
   ```bash
   npm install
   cd client
   npm install
   ```

3. **Build the Client**: Build the project using Webpack to create the bundled output.
   ```bash
   npm run build
   ```

4. **Start the Server**: Go back to the root directory and start the server:
   ```bash
   cd ..
   npm run start
   ```

## Usage
1. Open your web browser and go to `http://localhost:3000` (or the specified port).
2. You will be presented with a text editor interface powered by CodeMirror.
3. Type your content in the editor.
4. The content is automatically saved to IndexedDB when you click away from the editor or lose focus.
5. The next time you open the app, your saved content will be retrieved from IndexedDB.
6. Use the **Install** button to install TextMaster as a local app on your desktop or mobile device.

## Features
- **Offline Access**: TextMaster works seamlessly even without an internet connection, allowing you to retrieve and save content using IndexedDB.
- **PWA Capabilities**: The app can be installed on your desktop or mobile device for a native-like experience.
- **Code Syntax Highlighting**: Utilizes CodeMirror for syntax highlighting and an enhanced text editing experience.
- **Auto-Save**: Automatically saves your content to IndexedDB.
- **Responsive Design**: Works on all devices, whether it be a desktop, tablet, or mobile phone.

## Technologies Used
- **Node.js**: Server-side runtime environment.
- **Express.js**: Web framework for building the server and handling routes.
- **Webpack**: Module bundler for packaging JavaScript, CSS, and other assets.
- **Babel**: JavaScript compiler for next-gen syntax support.
- **IndexedDB**: Database to handle offline storage and retrieval of content.
- **Workbox**: Service worker library for managing offline capabilities.
- **CodeMirror**: In-browser code editor with support for multiple languages and syntax highlighting.

