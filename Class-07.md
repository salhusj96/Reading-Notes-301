# **What is NGINX?**
## *Why is this topic important?*
- NGINX is a great Linux tool for webserving, and even though it's not necessarily a direct domain of Cybersecurity, it is still an essential tool for Networking.
### **Backstory**
- Written by Igor Sysoev to solve the C10K problem
  - handling large numbers (*the 10K*) of concurrent connections (*the C*)
- Revolutionized how servers operate in high-performance contexts
- Became the fastest webserver available
### **NGINX as a Web Server**
- consistently beats Apache and other servers in benchmarks measuring web server performance
- supports HTML, WebSocket, HTTP/2, gRPC, and streaming of multiple video formats
### **NGINX Beyond Web Serving**
- commonly used as a reverse proxy and load balancer to manage incoming traffic and distribute it to slower upstream servers
- frequently placed between clients and a second web server
  - serves as an SSL/TLS terminator or web accelerator
- efficiently handles tasks that may slow down the web server
- makes effective use of underlying hardware
  - Dynamic sites, built using anything from Node.js to PHP, commonly deploy NGINX as a content cache and reverse proxy to reduce load on application servers
### **What Can NGINX and NGINX Plus Do for You?**
- used by high-traffic websites such as DropBox, Netflix, etc.
- multi-function; can use the same tool as your load balancer, reverse proxy, content cache, and web server
---
## **Things I want to know more about**
- NGINX seems like it could be the perfect solution for a home PLEX server, I'd like to know more about its smaller organizational/home use-cases.