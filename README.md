# SimpleTCPFileTransfer

🖥️ Client-Server File Transfer Program
This project involved developing a custom client-server application built to demonstrate foundational network programming concepts, including socket communication, concurrency, and file transfer protocols.

🔧 Key Features & Functionality:

Server Initialization:
The server is programmed to start in a listening state on the default TCP port 7005, awaiting incoming client connections.
Designed to run persistently, handling multiple connection attempts without requiring manual resets or intervention.

Client Connectivity:
A client program can connect to the server using either the server’s IP address or domain name, with flexibility to specify the port (defaulting to 7005 if none is provided).
Upon connection, the client can send supported command requests which are interpreted and executed by the server.

Command Support:
GET Command: Allows the client to request a specific file from the server. Upon receiving this command, the server locates the file, reads it, and streams the data back to the client securely over the established socket connection.
SEND Command: Enables the client to send/upload a file to the server. The server receives the incoming data and writes it to disk in the appropriate location.

Connection Management:
The server is designed to accept any client without authentication or IP restrictions, making it ideal for testing or educational environments.
Robust error handling is implemented to manage scenarios such as unavailable files, incomplete transfers, or malformed requests.

Language & Tools Used:
Developed in Python, utilizing standard socket libraries.
Console-based I/O and clear logging to help monitor connection events and data flow.


🎯 Purpose & Impact:
This project showcases a practical implementation of socket programming, reinforcing concepts such as persistent connections, request-response cycles, and basic protocol design. It also demonstrates your ability to handle both client-side and server-side logic, and effectively manage file operations across a network.
