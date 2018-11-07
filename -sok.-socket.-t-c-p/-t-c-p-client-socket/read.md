---
title: TCPClientSocket.read - sok
---

[sok](../../index.html) / [Sok.Socket.TCP](../index.html) / [TCPClientSocket](index.html) / [read](./read.html)

# read

`suspend fun read(buffer: `[`MultiplatformBuffer`](../../-sok.-buffer/-multiplatform-buffer/index.html)`): `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html) [(source)](https://github.com/SeekDaSky/Sok/tree/master/common/sok-common/src/Sok/Socket/TCP/TCPClientSocket.kt#L62)

**Platform and version requirements:** Common


`suspend actual fun read(buffer: <ERROR CLASS>): `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html) [(source)](https://github.com/SeekDaSky/Sok/tree/master/jvm/sok-jvm/src/Sok/Socket/TCP/TCPClientSocket.kt#L197)

**Platform and version requirements:** JVM, JS, Native

Perform a suspending read, the method will read n bytes ( 0 &lt; n &lt;= buffer.remaining() ) and update the cursor

### Parameters

`buffer` - buffer used to store the data read

**Return**
Number of byte read

`suspend fun read(buffer: `[`MultiplatformBuffer`](../../-sok.-buffer/-multiplatform-buffer/index.html)`, minToRead: `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)`): `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html) [(source)](https://github.com/SeekDaSky/Sok/tree/master/common/sok-common/src/Sok/Socket/TCP/TCPClientSocket.kt#L71)

**Platform and version requirements:** Common


`suspend actual fun read(buffer: <ERROR CLASS>, minToRead: `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)`): `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html) [(source)](https://github.com/SeekDaSky/Sok/tree/master/jvm/sok-jvm/src/Sok/Socket/TCP/TCPClientSocket.kt#L232)

**Platform and version requirements:** JVM, JS, Native

Perform a suspending read, the method will read n bytes ( minToRead &lt; n &lt;= buffer.remaining() ) and update the cursor

### Parameters

`buffer` - buffer used to store the data read

**Return**
Number of byte read

