### What are the relevant arguments to those methods, and the values of any relevant fields of the class?

- **`HttpExchange exchange`:** This object contains all the details of a single HTTP request-response transaction. It includes the request URI, which has the path `/add-message` and the query parameters `s` (the message) and `user` (the username), for processing chat messages.

### How do the values of any relevant fields of the class change from this specific request? If no values got changed, explain why.

- **Field:** `String chatHistory`

  - **Before First Request:** Initially, `chatHistory` starts as an empty string `""` which when we open the link the page shows the very
      first screenshot.

  - **After First Request** (`/add-message?s=Hello&user=eemami`):
    - `chatHistory` is updated to `"eemami: Hello\n"`.
  - **After Multiple Requests:** Each additional request further appends a message to `chatHistory` in the format `<user>: <message>\n`. Below is the example I used to execute the ChatServer.java

    ```
    eemami: Hello
    eemami: Hello
    eemami: Hello
    eemami: Hello
    Constantin: Hey Dude, What up?
    eemami: Are you Constantin, What up?
    eemami: Are you Constantin?
    Constantin: Yeah I am the former Emperor of Rome CONSTANTIN!
    eemami: You liar! You're a student in cse15L!
    Constantin: So what?!
    ```

    This shows the chat history being sequentially updated with each new message, formatted as `<user>: <message>` followed by a newline character.

### Explanation:

- Upon receiving a chat message through the `/add-message` endpoint, the server's `handle` method is invoked with the `HttpExchange` object.
- This method extracts the `user` and `s` (message) values from the query parameters of the request URI.
- These values are then used to append the new message to the `chatHistory` field in the specified format.
- The `chatHistory`, now containing the updated conversation, is included in the server's response, allowing users to view the ongoing chat history.
