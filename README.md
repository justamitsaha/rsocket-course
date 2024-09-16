# simple-rsocket Simple RSocket project without Spring

- **`class Server `**  Create RSocket client which will start server
- **`SocketAcceptorImpl`** This call will accept the connection request and instantiate the correct Service class request and pass the request and the connection details of the client.  Un comment the propre service method to route the request to proper service class
- **`Basic Request response Model`** implemented in    **`class MathService `**  it To be tested with **`Lec01RSocketTest`**
  - fireAndForget
  - requestResponse
  - requestStream
  - requestChannel
- Call back to Client
- **`Callback from`** from BatchJobService will call the service **`CallbackService`** defined in test (client) triggered via  **` Lec02CallbackTest `**.
- **`Backpressure`** will be handled automatically by **`FastProducerService`**  for slow client **`Lec03BackpressureTest`**.
- **`Persistent connection`** will be  demonstrated by  **`Lec04PersistentConnectionTest`** uses  to connect with **`FastProducerService`** even when connection is reset
- **`Connection set up payload`** will be passed by **`Lec05ConnectionSetupTest`** based on that **`FreeService`** is called

