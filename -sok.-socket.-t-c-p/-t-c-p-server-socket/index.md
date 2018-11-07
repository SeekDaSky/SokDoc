---
title: TCPServerSocket - sok
---

[sok](../../index.html) / [Sok.Socket.TCP](../index.html) / [TCPServerSocket](./index.html)

# TCPServerSocket

`expect class TCPServerSocket` [(source)](https://github.com/SeekDaSky/Sok/tree/master/common/sok-common/src/Sok/Socket/TCP/TCPServerSocket.kt#L8)

Class representing a listening socket. You can use it to perform accept() operation only.

### Constructors

| [&lt;init&gt;](-init-.html) | `TCPServerSocket(address: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`, port: `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)`)`<br>Start a listening socket on the given address (or alias) and port |

### Properties

| [isClosed](is-closed.html) | `var isClosed: `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)<br>keep track of the socket state |

### Functions

| [accept](accept.html) | `suspend fun accept(): `[`TCPClientSocket`](../-t-c-p-client-socket/index.html)<br>Accept a client socket. The method will suspend until there is a client to accept |
| [bindCloseHandler](bind-close-handler.html) | `fun bindCloseHandler(handler: () -> `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)`): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)<br>handler called when the socket close (expectedly or not) |
| [close](close.html) | `fun close(): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)<br>close the server socket |

