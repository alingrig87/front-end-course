
# 02_Request_Life_Cycle - Detailed Answers

1. **What is the Request Life Cycle? Describe its purpose in web applications.**  
   The **Request Life Cycle** refers to the sequence of steps that a request follows from initiation to the server’s response, essential for web applications to manage interactions between client and server. It ensures that each request is systematically handled, processed, and responded to, providing a structured flow for data exchange.

2. **Explain the first step in the Request Life Cycle: Client Request Initiation.**  
   The cycle begins when the client (e.g., browser or app) triggers a request. This initiation can occur by entering a URL, clicking a link, or submitting a form, and signals to the client system to gather information and begin establishing a connection with the intended server.

3. **What is DNS resolution, and why is it necessary?**  
   **DNS resolution** is the process of translating a domain name (e.g., www.example.com) into its corresponding IP address, which is required for the client to connect to the correct server. If the IP is not cached locally, the client queries DNS servers in a hierarchical structure until it obtains the IP address, allowing it to locate the server on the internet.

4. **How does a client establish a connection to a server?**  
   Once the IP address is known, the client initiates a **TCP connection** with the server, typically over **port 80 for HTTP** or **port 443 for HTTPS**. This connection is established via a handshake, allowing both client and server to agree on communication protocols and enabling secure, reliable data transfer.

5. **What is included in the HTTP request sent to the server?**  
   The HTTP request includes:
   - **Request Line**: Specifies the HTTP method (GET, POST), resource path, and HTTP version.
   - **Headers**: Metadata about the request, such as content type and authentication.
   - **Optional Body**: Data sent with the request, relevant for methods like POST or PUT (e.g., form data or JSON payload).

6. **How does the server process a request? What factors affect this process?**  
   The server receives and interprets the request, identifying the endpoint and verifying permissions. Factors affecting processing include request complexity, server load, required database access, and the need to execute application logic. The server then prepares the appropriate data or action as specified by the request.

7. **When is database access needed in the Request Life Cycle? Describe the server's role in accessing data.**  
   Database access is needed when the requested resource or data is not readily available. The server interacts with the database, executing queries to retrieve or update data. This data is often processed or formatted before being returned in the response.

8. **Explain the steps involved in generating and sending a response from the server.**  
   The server composes an HTTP response, including:
   - **Status Line**: HTTP version, status code, and reason phrase (e.g., 200 OK).
   - **Headers**: Provide metadata (e.g., content type, content length).
   - **Body**: Contains the requested data or a message, structured based on client expectations (e.g., JSON or HTML).

9. **What happens on the client side after receiving a response?**  
   The client interprets the response. In browsers, HTML content is rendered, while JSON may trigger dynamic actions or updates on the interface. The client may also display error messages based on status codes if the response indicates an error.

10. **Describe the significance of closing the connection in the Request Life Cycle.**  
   Closing the connection frees up resources on both the client and server, making the system more scalable. In HTTP/1.1, persistent connections may remain open briefly to allow multiple requests without reconnecting, improving efficiency in multi-request scenarios.
