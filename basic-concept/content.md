## NodeJs - Understanding basic concepts

### The essential knowledge

Important steps to create a webserver

- How does the web work ? (Refresher)
- Creating a NodeJs server
- Using Node cores modules
- Working with Requests and Responses
- Async code
- Event Loop

These are crucial things who you've got know to build a good node application.

Other important point is undertand how node uses asynchronous code and acept callled the event loop to stay reactive.

### How the web works ?

_User / Client (Browser) -> http://my-page(Domain Lookup)_

The user enter in some URL, what happens behind the scene is actualy that browser reaches out to some domain name servers.

This domain is not really the adress of your server. It's basically and encoded human readable version of that adress (IP).

- User/Client send a request to server
- Server (at 10.211.212.2)
- Server send a response

That request and response follow some rules who are defined by some protocol.

#### HTTP / HTTPS

- **H**yper **T**ext **T**ransfer **P**rotocol : A protocol for transferring data wich is understood by browser and server

- **H**yper **T**ext **T**ransfer **P**rotocol **S**ecure : HTTP + Data Encryption (during transmission of data)

### Core modules of node server

- http
  - Launch a server
  - Send requests
- https
  - Launch a SSL server
- fs
- path
- os

### NodeJs prigram lifecycle

- Start Script (node app.js)
- Parse code, register variables and functions
- Event Loop (keeps on running as long as there are event listeners registered)
- proccess.exit

_obs Want to quit your running Node.js server?_

_You can always do that by pressing CTRL + C in the terminal/ command prompt window where you started your server (i.e. where you ran node app.js)._

### Undertanding requests

A Hypertext Transfer Protocol (HTTP) request is a fundamental communication mechanism in the World Wide Web that enables the exchange of information between a client and a server. When a user interacts with a web browser, such as entering a URL or clicking a link, the browser generates an HTTP request to the specified server. This request is essentially a message sent by the client to request a specific resource, such as a web page, image, or file. The HTTP request includes important details, such as the type of request (e.g., GET for retrieving information, POST for submitting data), the target resource's location, and any additional parameters or headers. Upon receiving the HTTP request, the server processes the request, retrieves the requested resource, and sends back an HTTP response containing the desired information. HTTP requests form the backbone of communication on the internet, facilitating the seamless transfer of data and content between clients and servers.

### Sending responses

An HTTP response is the server's reply to an HTTP request made by a client, typically a web browser. After receiving a request, the server processes the information and sends back an HTTP response containing the requested data or indicating an error. The response includes a status code that conveys the outcome of the request, such as success (status code 200), redirection (status code 300s), client error (status code 400s), or server error (status code 500s). Additionally, the response may include headers, a message body, and other metadata. The headers provide crucial information about the response, such as the content type, server type, date of the response, and any specific instructions for the client. The message body contains the actual content requested, whether it be HTML for a web page, an image, or other types of data. Together, HTTP responses play a pivotal role in enabling seamless communication between clients and servers on the internet.

HTTP headers are key-value pairs included in both HTTP requests and responses, serving as additional metadata that conveys essential information about the message being exchanged. Headers provide details such as content type, content length, server information, and caching instructions. They play a crucial role in facilitating effective communication between clients and servers by conveying instructions on how the data should be processed, interpreted, or displayed. For example, the "Content-Type" header specifies the media type of the resource, ensuring the client knows how to handle the received data. Headers enhance the functionality and efficiency of the HTTP protocol by enabling customization and control over the communication process between web clients and servers.
