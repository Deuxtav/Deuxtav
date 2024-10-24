Chat Application README

Overview

This chat application consists of a server and client built in Java, allowing multiple users to connect and communicate in real-time. The server manages client connections, while clients can send and receive messages.

Features

- Multi-client Support : The server can handle multiple clients simultaneously.
- User Identification : Each client must provide a unique alias upon connecting.
- Broadcast Messaging : Messages sent by any client are broadcasted to all connected clients.
- Graceful Exit : Clients can exit the chat using the "exit" command.

Components

Server

- Class : ChatServer
- Port :12345 (modifiable in the code)
- Functionality :
  - Accepts new client connections.
  - Manages communication between clients.
  - Handles user identification and broadcasting messages.

Client

- Class :ChatClient
- Connection: Connects to the server at localhost:12345.
- Functionality:
  - Prompts the user for a name and sends it to the server.
  - Listens for messages from the server and displays them.
  - Allows the user to send messages to the server.

Getting Started

Prerequisites

- Java Development Kit (JDK) installed on your machine.
- Basic understanding of Java programming.

Running the Application

1. Compile the Code:
   Navigate to the directory containing the server and client packages and compile the code:
     javac server/ChatServer.java client/ChatClient.java
   
2. Start the Server:
   Open a terminal window and run the server:
     java server.ChatServer
   
3. Start the Client:
   Open one or more terminal windows (or instances) to run the client:
     java client.ChatClient
   
4. Connecting:
   - The client will prompt for a name. Enter your alias and press Enter.
   - You can start sending messages. To exit, type "exit".

Code Structure

- ChatServer.java :Contains the server logic, including handling client connections and broadcasting messages.
- ChatClient.java :Contains the client logic, handling user input and communication with the server.

Error Handling

- The server and client include basic error handling for socket operations and user input validation.
- Ensure that the server is running before starting any clients to avoid connection errors.

Customization

- You can change the networkPort variable in ChatServer.java to use a different port.
- Modify the messaging logic to add additional features, such as private messaging or message history.

License

This application is open source. Feel free to modify and distribute as needed.
