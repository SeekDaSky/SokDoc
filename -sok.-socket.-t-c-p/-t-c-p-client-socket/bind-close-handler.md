---
title: TCPClientSocket.bindCloseHandler - sok
---

[sok](../../index.html) / [Sok.Socket.TCP](../index.html) / [TCPClientSocket](index.html) / [bindCloseHandler](./bind-close-handler.html)

# bindCloseHandler

`fun bindCloseHandler(handler: () -> `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)`): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) [(source)](https://github.com/SeekDaSky/Sok/tree/master/common/sok-common/src/Sok/Socket/TCP/TCPClientSocket.kt#L25)

handler called when the socket close (expectantly or not)

### Parameters

`handler` - lambda called when the socket is closed