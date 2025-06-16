# Simple HTTP Server – Java Project

This project implements a simplified HTTP server in Java as part of an academic software engineering course.  
It includes a generic server structure with support for parsing HTTP requests, routing based on HTTP method and URI, and dynamic servlet handling.

## 🧩 Main Components

- *RequestParser* – Parses raw HTTP requests into structured data including:
  - Method (GET, POST, etc.)
  - URI segments
  - Query parameters
  - Request body content
- *HTTPServer / MyHTTPServer* – A multithreaded HTTP server supporting servlet registration/removal and background execution.
- *Servlet* – Defines how each handler responds to client requests based on the parsed request info.

## ✅ Example Request Handling

The server correctly parses requests such as:

GET /api/resource?id=123&name=test HTTP/1.1
Host: example.com
Content-Length: 5

filename="hello_world.txt"

hello world!

markdown
Copy
Edit

Extracted results:

- *Parameters*:  
  - id=123  
  - name=test  
  - filename=hello_world.txt

- *Content (body)*:  
  hello

## 🏆 Grade

*100/100*  
Passed all functional and automated tests, including parameter parsing and content accuracy.

---

*Built by: Abigail Jacob*
