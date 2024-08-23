# TCP Proxy

## Overview
This is a simple TCP echo server written in Go. The server listens for incoming TCP connections on a specified port, receives data from the client, and sends the same data back to the client. This is commonly referred to as an "echo" server because it echoes back the input it receives.

## Features
* Listens for incoming TCP connections on port 20080.
* Handles multiple clients concurrently using Goroutines.
* Echoes received data back to the client.
* Gracefully handles client disconnections and unexpected errors.
## Usage
To use this TCP echo server, you need to have Go installed on your system.
### 1) Clone the repository
(if applicable) or create a new file with the provided code.
### 2) Build the application:
```bash
go build -o echoServer
```

### 3) Run the application:
```bash
./echoServer
```
The server will start listening on 0.0.0.0:20080.

### 4) Connect to the server:
You can use tools like telnet or nc (Netcat) to connect to the server and test its functionality:
```bash
telnet localhost 20080
```
Or:
```bash
nc localhost 20080
```
Type any text, and the server will echo it back to you.

## Disclaimer

## Contribution
Feel free to open an issue or submit a pull request if you have any suggestions or improvements.

