---
title: TCPServerSocket.exceptionHandler - sok
---

[sok](../../index.html) / [Sok.Socket.TCP](../index.html) / [TCPServerSocket](index.html) / [exceptionHandler](./exception-handler.html)

# exceptionHandler

`var exceptionHandler: (exception: `[`Throwable`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-throwable/index.html)`) -> `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) [(source)](https://github.com/SeekDaSky/Sok/tree/master/common/sok-common/src/Sok/Socket/TCP/TCPServerSocket.kt#L17)

Lambda that will be called when an exception resulting in the closing of the socket is thrown,
for further information look at the "Exception model" part of the README

### Property

`exceptionHandler` - Lambda that will be called when an exception resulting in the closing of the socket is thrown,
for further information look at the "Exception model" part of the README