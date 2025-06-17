Simple Multithreaded HTTP Server in Java
This project implements a lightweight, multithreaded HTTP server from scratch using core Java libraries only – without relying on external frameworks.

It was developed as part of an academic Software Engineering course (פת"מ 1) and received a perfect score (100/100).

Features
✅ Full implementation of a modular HTTP server from scratch

📡 Supports basic HTTP methods: GET, POST, and DELETE

🧩 Custom routing mechanism with longest prefix matching

🧵 Multithreaded client handling using a thread pool

📦 Request parsing with support for URI parameters and request body

🔌 Easily extendable via the Servlet interface

Structure
MyHTTPServer.java: The core server class implementing HTTPServer

RequestParser.java: Parses raw HTTP requests into structured RequestInfo objects

Servlet.java: Interface for handling HTTP requests

MainTrain.java: Test suite for parsing and server execution

Example Usage
java
Copy
Edit
MyHTTPServer server = new MyHTTPServer(8080, 4);
server.addServlet("GET", "/api/echo", new EchoServlet());
server.start();
✅ Developed by: Roni Ayalon
🎓 Course: Advanced Software Development (פת"מ 1)
🏆 Final Grade: 100/100
Passed all functional and automated tests, including parameter parsing and content accuracy.

---

*Built by: Abigail Jacob*
