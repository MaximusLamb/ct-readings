# HTTP
* The Hyper Text Transfer Protocol (HTTP) is a stateless request-response application layer protocol. 
*  HTTP is used to build distributed, collaborative, hypermedia information systems. HTTP is the foundation for the world wide web. Applications built using HTTP subscribe to the client-server computing model.
# Requests
* A HTTP/1.1 request is formatted in text and transferred using TCP. 
### GET
### HEAD
### POST
### PUT
### DELETE
### CONNECT
### OPTIONS
### TRACE
### PATCH
* Safe methods should only be used for information retrieval and should not change the server state. Idempotent methods means if two identical requests are made they should get an identical response. Cacheable means the client should be able to cache the response.
# RESPONSES
* A HTTP/1.1 response is also formatted in text and transferred using TCP. The first line of the response contains the HTTP VERSION, STATUS CODE, and STATUS MESSAGE. The following lines are the request headers and are formatted exactly the same way as the request headers. The header section of the request is terminated with an empty line. An optional body follows the header section.