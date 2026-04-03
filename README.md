# Chat Application

A simple Java-based chat application consisting of a client and server that communicate over sockets.

## Description

This project implements a basic client-server chat system using Java sockets. The server listens on port 2222, and the client connects to it. Both sides can send and receive messages in real-time using separate threads for reading and writing. The chat can be terminated by typing "exit".

## Features

- Real-time messaging between client and server
- Multi-threaded for concurrent reading and writing
- Simple text-based interface
- Terminates chat when "exit" is sent

## Prerequisites

- Java Development Kit (JDK) 8 or higher
- A terminal or command prompt to run the applications

## Installation

1. Clone the repository:
   ```
   git clone <repository-url>
   cd chat-application
   ```

2. Ensure JDK is installed and `java` and `javac` are in your PATH.

## Usage

1. **Start the Server:**
   - Open a terminal in the project directory.
   - Compile the server: `javac Server.java`
   - Run the server: `java Server`

2. **Start the Client:**
   - Open another terminal in the project directory.
   - Compile the client: `javac Client.java`
   - Run the client: `java Client`

3. **Chatting:**
   - Type messages in either terminal to send them.
   - Messages will appear prefixed with "Client:" or "Server:".
   - Type "exit" to terminate the chat.

## How It Works

- The server creates a ServerSocket on port 2222 and waits for a client connection.
- The client connects to localhost:2222.
- Both use BufferedReader for input and PrintWriter for output.
- Separate threads handle reading incoming messages and writing outgoing messages.
- The connection closes when "exit" is sent.

## Contributing
<img width="1920" height="1080" alt="Screenshot (97)" src="https://github.com/user-attachments/assets/1ed25bae-ceca-480b-9d6b-50ce22f9204d" />
<img width="1920" height="1080" alt="Screenshot (97)" src="https://github.com/user-attachments/assets/025a8610-8b89-4e21-b621-1d09941e0915" />

1. Fork the repository.
2. Create a feature branch: `git checkout -b feature-name`
3. Commit changes: `git commit -am 'Add feature'`
4. Push to the branch: `git push origin feature-name`
5. Submit a pull request.

## License

This project is licensed under the MIT License - see the LICENSE file for details.
