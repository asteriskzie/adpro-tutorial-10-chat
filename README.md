1. The screenshot: 
    ![alt text](img/image-2.1.png)
    The server is the leftmost. Run it using:
    ```
    cargo run --bin server
    ```
    And run the client using:
    ```
    cargo run --bin client
    ```
    When I typed something in the client, the server received it and broadcasted it to all clients. The clients received the message and printed it out. The server also printed out the message it received and from which client. 

2. Firstly I changed the port of client.rs as instructed. When I try running the server and client again, the server runs just fine but the cilent says "Connection refused". Turns out I also need to modify the port in server.rs (specifically, the listener port). After that, the client can connect to the server as before. 