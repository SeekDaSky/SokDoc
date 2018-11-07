---
title: Sok.Socket.TCP - sok
---

[sok](../index.html) / [Sok.Socket.TCP](./index.html)

## Package Sok.Socket.TCP

### Types

| [TCPClientSocket](-t-c-p-client-socket/index.html) | `expect class TCPClientSocket`<br>Class representing a client socket. You can use it to perform any I/O operation. Keep in mind that this class keep an internal queue for write operations thus storing data until written so you should have some kind of backpressure mechanism to prevent the accumulation of too many data. |
| [TCPServerSocket](-t-c-p-server-socket/index.html) | `expect class TCPServerSocket`<br>Class representing a listening socket. You can use it to perform accept() operation only. |

### Functions

| [createTCPClientSocket](create-t-c-p-client-socket.html) | `suspend expect fun createTCPClientSocket(address: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`, port: `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)`): `[`TCPClientSocket`](-t-c-p-client-socket/index.html)<br>Create a client socket with the given address and port. This function will throw a `ConnectionRefusedException` if the socket failed to connect. |

