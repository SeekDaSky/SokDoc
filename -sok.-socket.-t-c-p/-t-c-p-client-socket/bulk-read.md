---
title: TCPClientSocket.bulkRead - sok
---

[sok](../../index.html) / [Sok.Socket.TCP](../index.html) / [TCPClientSocket](index.html) / [bulkRead](./bulk-read.html)

# bulkRead

`suspend fun bulkRead(buffer: `[`MultiplatformBuffer`](../../-sok.-buffer/-multiplatform-buffer/index.html)`, operation: (buffer: `[`MultiplatformBuffer`](../../-sok.-buffer/-multiplatform-buffer/index.html)`, read: `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)`) -> `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)`): `[`Long`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-long/index.html) [(source)](https://github.com/SeekDaSky/Sok/tree/master/common/sok-common/src/Sok/Socket/TCP/TCPClientSocket.kt#L67)

**Platform and version requirements:** Common


`suspend actual fun bulkRead(buffer: <ERROR CLASS>, operation: (<ERROR CLASS>, read: `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)`) -> `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)`): `[`Long`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-long/index.html) [(source)](https://github.com/SeekDaSky/Sok/tree/master/jvm/sok-jvm/src/Sok/Socket/TCP/TCPClientSocket.kt#L172)

**Platform and version requirements:** JVM, JS, Native

Used to do efficient read-intensive loops, it will basically execute the operation each time there is data to be read
and avoid registrations/allocation between each iteration. The passed lambda must return true to continue the loop or
false to exit. The call will suspend as long as the loop is running.

THE OPERATION MUST NOT BE COMPUTATION INTENSIVE OR BLOCKING as the internal selector will call it synchronously and wait
for it to return before processing any other event. The buffer cursor will be reset between each iteration so you should
not use it between two iterations and must avoid leaking it to exterior coroutines/threads. each iteration will read
n bytes ( 0 &lt; n &lt;= buffer.limit ) and set the cursor to 0, the read parameter of the operation is the amount of data read.

If an exception is thrown in the operation lambda, the exception will not close the socket and will not be received by the
exception handler, it will instead be thrown directly by the method

### Exceptions

`PeerClosedException` -

`SocketClosedException` -

`BufferOverflowException` -

`ConcurrentReadingException` -

### Parameters

`buffer` - buffer used to store the data read. the cursor will be reset after each iteration. The limit of the buffer remains
untouched so the developer can chose the amout of data to read.

`operation` - lambda called after each read event. The first argument will be the buffer and the second the amount of data read

**Return**
Total number of byte read

