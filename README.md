# Description

The provided Python code consists of two files: "Server Model.py" and "Client Model.py".

### Server Model.py

This script sets up a multi-threaded server using the socket module, capable of both secure and unsecure communication. It utilizes the `rsa` and `cryptography` libraries for encryption and decryption. The server listens on port 8888 and processes incoming client requests. It handles different packet types, such as session initiation, encryption setup, and information requests, and responds accordingly. The server supports sending and receiving encrypted messages using session keys.

### Client Model.py

This script acts as a client that connects to the server defined in "Server Model.py". It uses the `rsa` and `cryptography` libraries to handle encryption. The client prompts the user to choose between secure and unsecure communication. Depending on the choice, the client either sends unencrypted messages or sets up encryption using RSA and Fernet keys. It sends various packets to the server, including session initiation, encryption setup, and information requests, and processes server responses. The client can handle secure communication by encrypting messages before sending them to the server. 

To use these files, start the server by running "Server Model.py". Then, run "Client Model.py" to connect to the server and send messages. Ensure the required libraries (`rsa` and `cryptography`) are installed.
