---
title: createTCPClientSocket - sok
---

[sok](../index.html) / [Sok.Socket.TCP](index.html) / [createTCPClientSocket](./create-t-c-p-client-socket.html)

# createTCPClientSocket

`suspend expect fun createTCPClientSocket(address: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`, port: `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)`): `[`TCPClientSocket`](-t-c-p-client-socket/index.html) [(source)](https://github.com/SeekDaSky/Sok/tree/master/common/sok-common/src/Sok/Socket/TCP/TCPClientSocket.kt#L95)

Create a client socket with the given address and port. This function will throw a `ConnectionRefusedException` if the socket
failed to connect.

### Parameters

`address` - IP or domain to connect to

`port` - port to connect to

**Return**
connected socket

