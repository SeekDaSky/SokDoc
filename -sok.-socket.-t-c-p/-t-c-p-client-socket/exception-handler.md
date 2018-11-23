---
title: TCPClientSocket.exceptionHandler - sok
---

[sok](../../index.html) / [Sok.Socket.TCP](../index.html) / [TCPClientSocket](index.html) / [exceptionHandler](./exception-handler.html)

# exceptionHandler

`var exceptionHandler: (exception: `[`Throwable`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-throwable/index.html)`) -> `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) [(source)](https://github.com/SeekDaSky/Sok/tree/master/common/sok-common/src/Sok/Socket/TCP/TCPClientSocket.kt#L27)

Lambda that will be called when an exception resulting in the closing of the socket is thrown. This
happen when calling the `close` or `forceClose` method, if the peer close the socket or if something wrong happen internally.
Exception that does not affect the socket state will not be received by this handler (exception in the `bulkRead` operation
lambda for example)

### Property

`exceptionHandler` - Lambda that will be called when an exception resulting in the closing of the socket is thrown. This
happen when calling the `close` or `forceClose` method, if the peer close the socket or if something wrong happen internally.
Exception that does not affect the socket state will not be received by this handler (exception in the `bulkRead` operation
lambda for example)