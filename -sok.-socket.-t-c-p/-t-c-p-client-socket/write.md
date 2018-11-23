---
title: TCPClientSocket.write - sok
---

[sok](../../index.html) / [Sok.Socket.TCP](../index.html) / [TCPClientSocket](index.html) / [write](./write.html)

# write

`suspend fun write(buffer: `[`MultiplatformBuffer`](../../-sok.-buffer/-multiplatform-buffer/index.html)`): `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html) [(source)](https://github.com/SeekDaSky/Sok/tree/master/common/sok-common/src/Sok/Socket/TCP/TCPClientSocket.kt#L117)

**Platform and version requirements:** Common


`suspend actual fun write(buffer: <ERROR CLASS>): `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html) [(source)](https://github.com/SeekDaSky/Sok/tree/master/jvm/sok-jvm/src/Sok/Socket/TCP/TCPClientSocket.kt#L308)

**Platform and version requirements:** JVM, JS, Native

Perform a suspending write, the method will not return until all the data between buffer.cursor and buffer.limit are written.
The socket use an internal write queue, allowing multiple threads to concurrently write. Backpressure mechanisms
should be implemented by the developer to avoid having too much data in the queue. If the peer
closes the socket while reading, a `PeerClosedException` will be thrown. If the socket is manually closed while reading,
either `NormalCloseException` or `ForceCloseException` will be thrown

### Exceptions

`SocketClosedException` -

`BufferUnderflowException` -

`SokException` -

`PeerClosedException` -

### Parameters

`buffer` - data to write

**Return**
Success of the operation

