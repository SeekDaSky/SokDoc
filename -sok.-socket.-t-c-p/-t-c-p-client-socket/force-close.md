---
title: TCPClientSocket.forceClose - sok
---

[sok](../../index.html) / [Sok.Socket.TCP](../index.html) / [TCPClientSocket](index.html) / [forceClose](./force-close.html)

# forceClose

`fun forceClose(): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) [(source)](https://github.com/SeekDaSky/Sok/tree/master/common/sok-common/src/Sok/Socket/TCP/TCPClientSocket.kt#L40)

forcefully closes the channel without checking the writing request queue. Once the socket is closed a `ForceCloseException`
will be passed to the exception handler and to any ongoing read method call

