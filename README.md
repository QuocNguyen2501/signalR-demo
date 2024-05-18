# SignalR
- SignalR is an open-source library which simplifies adding real-time web/mobile functionalities to apps. This is the simple demo to show how to use AspNetCore SignalR. The demo includes 3 small projects: server, 2 clients (angular web, MAUI mobile).
- Real-time web functionality enables server-side code to push content to client instantly.
- Good scenarios for SignalR:
    - Apps require high frequency updates from server. Example: game, social networks, voting, auction, maps and GPS apps.
    - Dashboards and monitoring apps. Example: company dashboards, instant sales updates or travel alerts.
    - Collaborative apps. Whiteboard apps and team meeting software are examples of collaborative apps.
    - Apps that require notifications. Social networks, email, chat and many other apps use notifications.
- SignalR provides an API for creating server-to-client remote  procedure calls (RPC)
- Some features of SignalR for ASP.NET Core:
    - Handles connection management automatically.
    - Sends messages to all connected clients simultaneously.
    - Sends messages to specific clients or groups of clients.
    - Scales to handle increasing traffic.
    - SignalR Hub Protocol.
## Techniques for handling real-communications
- WebSockets
- Server-Sent Events
- Long Pooling

**Note:** SignalR automatically chooses the **best transport method** that is within the capapilities of the server and client.

## Hub
- Hubs are used by SignalR to communicate between clients and servers.
- A Hub is a high-level pipeline that allows a client and server to call methods on each other.
- SignalR provides 2 built-in hub protocols:
    - A text protocol based on JSON
    - A binary protocol based on MessagePack
    **Note:** Generally, MessagePack creates **smaller messages** compared to JSON. **Older browsers must support XHR level 2** to provide MessagePack protocol support.

## DON'T Support
 SignalR targets ES6. For browsers that don't support ES6, transpile the library to ES5.
 
 **The Signal javascript client DON'T support Internet Explorer and other older browsers**.