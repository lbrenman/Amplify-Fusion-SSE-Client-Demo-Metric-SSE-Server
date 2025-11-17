# Amplify Fusion SSE Client Demo

This is a demo project of the Amplify Fusion SSE Client artifact which can connect to an SSE Server.

In this demo it connects to a [Mock Metric server](https://github.com/lbrenman/nodejs-express-sse-mock-metrics-server-codespace) which can run in [GitHub CodeSpace](https://github.com/features/codespaces).

A video of the demo can be viewed [here](https://youtu.be/r4Sdjiox30E).

The demo filters the SSE server events and sends them to an client connected to an event-stream API exposed in Fusion.

![Imgur](https://imgur.com/Tx7GJyd.png)
![Imgur](https://imgur.com/N80sUxL.png)

The server is sending multiple event types:

![Imgur](https://imgur.com/8stWeSi.png)

and the Fusion Demo implementation is filtering for notification events only

![Imgur](https://imgur.com/UBcZeck.png)

You can import the project export zip file and edit the SSE Client Connection with the base URL of your SSE Metric Server.

![Imgur](https://imgur.com/8M5WLmy.png)

Then you can enable the API and connect to it to see notification events.

```bash
curl --location 'https://axway-appc-se-design.sandbox.fusion.services.axway.com:4443/MetricServerSSE/sse-metrics-from-server'
```

![Imgur](https://imgur.com/UBcZeck.png)