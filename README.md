# simple-rsocket Simple RSocket project without Spring

- **`class Server `**  Create RSocket client which will start server
- **`SocketAcceptorImpl`** This call will accept the connection request and instantiate the correct Service class request and pass the request and the connection details of the client 
- **`class MathService `**  it will implement various request response model
  - fireAndForget
  - requestResponse
  - requestStream
  - requestChannel
- 

