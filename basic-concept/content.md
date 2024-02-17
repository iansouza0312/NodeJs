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
