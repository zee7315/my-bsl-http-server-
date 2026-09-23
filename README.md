# BSL HTTP Server

A Low-Level HTTP Web Server Using Bonezegei Scripting Language and BSL Socket Library

---

## 1. Project Overview

This project implements a low-level HTTP web server from scratch using **Bonezegei Scripting Language (BSL)** and the **BSL Socket Library**.

The purpose of this project is to demonstrate the basic operation of an HTTP server using socket programming. Instead of using a high-level web framework, the server directly creates and manages a TCP socket, listens for incoming client connections, reads HTTP requests, identifies the requested URL path, generates an appropriate HTTP response, and sends the response back to the client.

The server runs locally on **port 8080** and supports three types of responses:

- `GET /` — returns the home page with an HTTP `200 OK` response.
- `GET /about` — returns the about page with an HTTP `200 OK` response.
- Any other requested path — returns a custom `404 Not Found` response.

The implementation demonstrates how a browser communicates with a basic HTTP server through TCP sockets.

---

## 2. Project Objectives

The main objectives of this project are:

1. To build a basic HTTP web server using Bonezegei Scripting Language.
2. To use the BSL Socket Library for TCP socket communication.
3. To understand how a server listens for incoming client connections.
4. To receive and process HTTP requests.
5. To identify the requested URL path from an HTTP request.
6. To implement basic HTTP routing.
7. To generate HTTP response headers and HTML response bodies.
8. To return appropriate HTTP status codes.
9. To demonstrate successful communication between a web browser and a low-level socket-based server.
10. To document the implementation and testing results.

---

## 3. Technologies Used

| Technology | Purpose |
|---|---|
| Bonezegei Scripting Language (BSL) | Programming language used to implement the server |
| BSL Socket Library | Provides socket functions for TCP communication |
| HTTP/1.1 | Application protocol used for browser-server communication |
| TCP | Transport protocol used by the socket connection |
| Visual Studio Code | Development environment |
| Windows Terminal / PowerShell | Used to run the BSL server |

---

## 4. Project Structure

The project follows the required structure and also contains the `lib` directory generated when the BSL Socket Library was installed.

```text
my-bsl-http-server/
│
├── .gitattributes
├── LICENSE
├── README.md
│
├── lib/
│   └── socket.bzg
│
├── src/
│   └── http.bzg
│
└── documentation/
    ├── home.png
    ├── about.png
    ├── 404.png
    └── terminal.png