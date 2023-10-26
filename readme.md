# Socket Server Documentation

This repository contains a Python script for a simple socket server that listens for incoming connections, receives messages from clients, logs them to a specified file, and responds with random quotes if the received message contains the word "network." Below is a detailed documentation of the code.

## Table of Contents

- [Socket Server Documentation](#socket-server-documentation)
  - [Table of Contents](#table-of-contents)
  - [Introduction](#introduction)
  - [Prerequisites](#prerequisites)
  - [Usage](#usage)
  - [Functionality](#functionality)
  - [License](#license)

## Introduction

This Python script creates a basic socket server that listens for incoming connections, processes messages, and logs them to a file. It also provides a random quote if the received message contains the word "network." The script uses command-line arguments to specify the port number for the server and the log file.

## Prerequisites

Before using this script, ensure you have the following:

- Python 3.x installed on your system.
- A text file named `quotes.txt` containing quotes for responses. The quotes should be separated by line breaks.
- Command-line access to run the script.

## Usage

To use the socket server script, follow these steps:

1. Clone or download this repository to your local machine.

2. Ensure you have Python 3.x installed.

3. Create a text file named `quotes.txt` in the same directory as the script. Add quotes, each on a separate line, to this file.

4. Open a terminal or command prompt and navigate to the directory containing the script.

5. Run the script with the following command:

   ```
   python server.py -p [port] -l [log_file]
   ```
- Replace [port] with the desired port number (e.g., 8080).
- Replace [log_file] with the name of the log file (e.g., server_log.txt).

## Functionality

The script has the following functionality:

- It creates a socket server and listens for incoming connections on the specified port.
- It logs received messages from clients to a specified log file.
- If a received message contains the word "network," the server responds with a random quote from the quotes.txt file.
- The quotes are read from the quotes.txt file, and the server sends one randomly selected quote as a response.
- The server can handle up to two concurrent connections.

## License
This code is provided under the MIT License. You are free to use and modify the code as needed. Please refer to the license file for more details.
