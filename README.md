### Real-Time Chat Application in Java

This project implements a simple Real-Time Chat Application in Java using sockets. It consists of two main components: the server-side (`ChatServer`) and the client-side (`ChatClient`).

### How it works:

- **Server-side (`ChatServer`)**:
    - Listens for incoming connections from clients on port `5000`.
    - Creates a new `ClientHandler` thread for each connected client.
    - Receives messages from clients and broadcasts them to all connected clients.
- **Client-side (`ChatClient`)**:
    - Connects to the server on localhost port `5000`.
    - Starts a receiver thread to listen for messages from other clients.
    - Reads user input from the console and sends it to the server to be broadcasted.

### Features:

- Multiple clients can connect to the server simultaneously.
- Messages sent by any client are broadcasted to all connected clients in real-time.
- Basic error handling for network communication.

### Usage:

1. Compile the Java files (`ChatServer.java` and `ChatClient.java`).
2. Run the `ChatServer` class to start the server.
3. Run the `ChatClient` class to start a client.
4. Enter messages in the client's console to send them to the server and receive messages from other clients.

### Notes:

- This is a basic implementation and lacks advanced features like user authentication, private messaging, or GUI.
- Additional error handling, threading, and security measures may be required for a production-ready chat application.
