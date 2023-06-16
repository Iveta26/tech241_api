# Intro to API

### What is an API?
API is used to communicate with other programs, it can translate the programs well.

[Diagram showcassing data transfer process in API communication](C:\Users\iveta_6esu9b1\PycharmProjects\tech241\pythonAndAPIs\Screenshot_5.png)

<br />

### What is a rest API?
REST (representational state transfer architectural) API is an API that conforms to the design principles of the REST, or representational state transfer architectural style. 

1. **Representational data flow**. All API requests for the same resource should look the same, no matter where the request comes from. The REST API should ensure that the same piece of data, such as the name or email address of a user, belongs to only one uniform resource identifier (URI). Resources shouldn’t be too large but should contain every piece of information that the client might need.

2. **URIs and naming**. In REST API design, client and server applications must be completely independent of each other. The only information the client application should know is the URI of the requested resource; it can't interact with the server application in any other ways. Similarly, a server application shouldn't modify the client application other than passing it to the requested data via HTTP.

3. **Statelessness**. REST APIs are stateless, meaning that each request needs to include all the information necessary for processing it. In other words, REST APIs do not require any server-side sessions. Server applications aren’t allowed to store any data related to a client request.

4. **Cacheability**. When possible, resources should be cacheable on the client or server side. Server responses also need to contain information about whether caching is allowed for the delivered resource. The goal is to improve performance on the client side, while increasing scalability on the server side.

<br />

### What is HTTP (Hyper Text Transfer Protocol)
HTTP is application protocol for distributed, collaborative, hypermedia information systems that allows users to communicate data on the World Wide Web. HTTPS is encrypted and secure.

<br />

### HTTP request structure

[Diagram showcassing HTTP request structure](C:\Users\iveta_6esu9b1\PycharmProjects\tech241\pythonAndAPIs\Screenshot_1.png)

Request consists of a **verb** (GET, POST, PUT, PATCH, DELETE), **URL** of the data and the **version**. **Header** consists of key value pairs, **body** (content) is optional.

<br />

### HTTP response structure
[Diagram showcassing HTTP response structure](C:\Users\iveta_6esu9b1\PycharmProjects\tech241\pythonAndAPIs\Screenshot_2.png)
Response consists of **response code** (e.g. 404, 200), **HTTP version**, **header** and **body** 

<br />

### 5 HTTP verbs
 - **GET** - get the data from server
 - **POST** - send the data to server
 - **PUT** - update existing resource
 - **PATCH** - similar to **PUT** as it also modifies an existing resource. The difference is that for the **PUT** method, the request body contains the complete new version, whereas for the **PATCH** method, the request body only needs to contain the specific changes to the resource, specifically a set of instructions describing how that resource should be changed, and the API service will create a new version according to that instruction.
 - **DELETE** - delete a resource specified by its URI.
