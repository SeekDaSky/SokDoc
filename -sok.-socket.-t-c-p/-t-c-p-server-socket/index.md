---
title: TCPServerSocket - sok
---

[sok](../../index.html) / [Sok.Socket.TCP](../index.html) / [TCPServerSocket](./index.html)

# TCPServerSocket

`expect class TCPServerSocket` [(source)](https://github.com/SeekDaSky/Sok/tree/master/common/sok-common/src/Sok/Socket/TCP/TCPServerSocket.kt#L12)

Class representing a listening socket. You can use it to perform accept() operation only.

### Properties

| [exceptionHandler](exception-handler.html) | `var exceptionHandler: (exception: `[`Throwable`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-throwable/index.html)`) -> `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)<br>Lambda that will be called when an exception resulting in the closing of the socket is thrown, for further information look at the "Exception model" part of the README |
| [isClosed](is-closed.html) | `var isClosed: `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)<br>keep track of the socket state |

### Functions

| [accept](accept.html) | `suspend fun accept(): `[`TCPClientSocket`](../-t-c-p-client-socket/index.html)<br>Accept a client socket. The method will suspend until there is a client to accept |
| [close](close.html) | `fun close(): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)<br>close the server socket |

