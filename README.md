# Chatboot Application

## Overview
The **Chatboot Application** is a browser-based chatbot that utilizes IndexedDB for managing user interactions. The application simulates multiple user sessions across different tabs, with each tab acting as an independent user.

---

## Key Features

- **IndexedDB for Data Storage:**
  - Stores chat messages locally in the user's browser.
  - Ensures message persistence even when tabs are closed and reopened.

- **Session Management:**
  - Treats each browser tab as a unique user session.
  - Allows independent conversations in each tab.

- **Real-time Chat Interface:**
  - Provides a responsive and interactive interface for user engagement.
  - Supports dynamic message handling and real-time responses.

- **Offline Support:**
  - Conversations are stored locally, enabling the chatbot to function without a server connection.

---

## How It Works

### Example Workflow:

1. **New Tab as New User:**
   - When a user opens a new tab, a new IndexedDB session is initialized.
   - The chatbot treats the tab as a separate user session with its own message history.

2. **Message Handling:**
   - Users type queries in the chat interface.
   - The messages are stored in IndexedDB for the current session.

3. **Response Generation:**
   - The chatbot processes user queries and generates appropriate responses.
   - Responses are displayed in the interface and saved in IndexedDB.

4. **Session Continuity:**
   - If a tab is closed and reopened, the chat history is retrieved from IndexedDB to maintain continuity.

---

## Technical Overview

- **Frontend:** Built with modern web technologies, such as React or vanilla JavaScript.
- **IndexedDB Integration:** Manages chat data storage and retrieval for each user session.
- **State Management:** Leverages browser APIs for dynamic session handling.
- **Styling:** Designed with responsive CSS for optimal usability across devices.

---

## Installation and Setup

To run this project locally, follow these steps:

### Clone the repository:

```bash
git clone https://github.com/mjsol12/Chatboot.git
cd Chatboot
```

### Install dependencies:

Using Yarn:

```bash
yarn install
```

Or using npm:

```bash
npm install
```

### Start the development server:

Using Yarn:

```bash
yarn start
```

Or using npm:

```bash
npm start
```

The application will be accessible at `http://localhost:3000`.

---

## Contributing

Contributions are welcome! If you'd like to contribute, please fork the repository and create a pull request with your changes.

---

## License

This project is licensed under the **MIT License**.
