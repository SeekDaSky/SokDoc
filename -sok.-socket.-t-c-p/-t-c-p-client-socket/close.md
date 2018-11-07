---
title: TCPClientSocket.close - sok
---

[sok](../../index.html) / [Sok.Socket.TCP](../index.html) / [TCPClientSocket](index.html) / [close](./close.html)

# close

`suspend fun close(): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) [(source)](https://github.com/SeekDaSky/Sok/tree/master/common/sok-common/src/Sok/Socket/TCP/TCPClientSocket.kt#L29)

gracefully stops the socket. The method suspends as it waits for all the writing requests in the channel to be
executed before effectively closing the channel

