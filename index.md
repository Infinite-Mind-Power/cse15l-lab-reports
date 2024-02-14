![scrnshot](thirdscrn.png)


This page provides a simple explanation of how messages are added to a chat using ChatServer.java.
Every time a message is added, like "Hello" from "eemami" or "Constantin"  "be the Emperor of Rome", the server performs a series of steps to update the chat history.

 ### Which methods in your code are called?
 
When interacting with the chat server, specifically when adding messages through the `/add-message` endpoint, the following method is involved:

### `handle(HttpExchange exchange)`

This method is the core of our `ChatHandler` class, designed to respond to HTTP requests. Here's a brief overview of its role in processing chat messages:

- **Purpose:** Handles incoming HTTP requests to the server, parsing the request URI to act accordingly based on the specified path and query parameters.
  
- **Process:**
  1. **Parse Request:** Extracts the request URI and query parameters (`s` for the message and `user` for the username).
  2. **Update Chat History:** Appends the new message to the `chatHistory` string in the format `<user>: <message>\n`.
  3. **Respond:** Sends back the updated chat history to the requester, showing the entire conversation so far.

Every time a user adds a message to the chat, this method is called to process the request and update the server's state accordingly.
