---
title: TCPServerSocket.bindCloseHandler - sok
---

[sok](../../index.html) / [Sok.Socket.TCP](../index.html) / [TCPServerSocket](index.html) / [bindCloseHandler](./bind-close-handler.html)

# bindCloseHandler

`fun bindCloseHandler(handler: () -> `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)`): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) [(source)](https://github.com/SeekDaSky/Sok/tree/master/common/sok-common/src/Sok/Socket/TCP/TCPServerSocket.kt#L34)

handler called when the socket close (expectedly or not)

### Parameters

`handler` - lambda called when the socket is closed