---
title: "Welcome to my blog - HttpClient
---

I'm glad you are here. I plan to talk about ...

HttpClient is designed for re-use. You should use a single instance of it throughout the lifetime of your application, or at least as few as possible when request signatures will vary (explained later). The main reason for this is that each instance of HttpClient will open a new socket connection and on high traffic sites, you can exhaust the available pool and receive a System.Net.Sockets.SocketException.
