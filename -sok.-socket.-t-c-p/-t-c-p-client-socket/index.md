---
title: TCPClientSocket - sok
---

[sok](../../index.html) / [Sok.Socket.TCP](../index.html) / [TCPClientSocket](./index.html)

# TCPClientSocket

`expect class TCPClientSocket` [(source)](https://github.com/SeekDaSky/Sok/tree/master/common/sok-common/src/Sok/Socket/TCP/TCPClientSocket.kt#L13)

Class representing a client socket. You can use it to perform any I/O operation. Keep in mind that this class keep an internal
queue for write operations thus storing data until written so you should have some kind of backpressure mechanism to prevent
the accumulation of too many data.

### Constructors

| [&lt;init&gt;](-init-.html) | `TCPClientSocket(channel: `[`SocketChannel`](http://docs.oracle.com/javase/6/docs/api/java/nio/channels/SocketChannel.html)`, selectorPool: `[`SelectorPool`](../../-sok.-selector/-selector-pool/index.html)`)`<br>Helper contrutor that simply get the less busy selector from the pool then use the "standard" constructor`TCPClientSocket(channel: `[`SocketChannel`](http://docs.oracle.com/javase/6/docs/api/java/nio/channels/SocketChannel.html)`, selector: `[`Selector`](../../-sok.-selector/-selector/index.html)`)`<br>Wrap a NIO channel with a Sok client socket class`TCPClientSocket(socket: dynamic)`<br>Wrap a Node.js socket with Sok Client socket class`TCPClientSocket(socket: `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)`, selector: `[`Selector`](../../-sok.-selector/-selector/index.html)`)`<br>Construtor used by the Server socket to build the client socket |

### Properties

| [isClosed](is-closed.html) | `var isClosed: `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)<br>Keep track of the socket status |

### Functions

| [bindCloseHandler](bind-close-handler.html) | `fun bindCloseHandler(handler: () -> `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)`): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)<br>handler called when the socket close (expectantly or not) |
| [bulkRead](bulk-read.html) | `suspend fun bulkRead(buffer: `[`MultiplatformBuffer`](../../-sok.-buffer/-multiplatform-buffer/index.html)`, operation: (buffer: `[`MultiplatformBuffer`](../../-sok.-buffer/-multiplatform-buffer/index.html)`, read: `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)`) -> `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)`): `[`Long`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-long/index.html)<br>`suspend actual fun bulkRead(buffer: <ERROR CLASS>, operation: (<ERROR CLASS>, read: `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)`) -> `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)`): `[`Long`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-long/index.html)<br>Used to do efficient read-intensive loops, it will basically execute the operation each time there is data to be read and avoid registrations/allocation between each iteration. The passed lambda must return true to continue the loop or false to exit. The call will suspend as long as the loop is running. |
| [close](close.html) | `suspend fun close(): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)<br>gracefully stops the socket. The method suspends as it waits for all the writing requests in the channel to be executed before effectively closing the channel |
| [forceClose](force-close.html) | `fun forceClose(): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)<br>forcefully closes the channel without checking the writing request queue |
| [read](read.html) | `suspend fun read(buffer: `[`MultiplatformBuffer`](../../-sok.-buffer/-multiplatform-buffer/index.html)`): `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)<br>`suspend actual fun read(buffer: <ERROR CLASS>): `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)<br>Perform a suspending read, the method will read n bytes ( 0 &lt; n &lt;= buffer.remaining() ) and update the cursor`suspend fun read(buffer: `[`MultiplatformBuffer`](../../-sok.-buffer/-multiplatform-buffer/index.html)`, minToRead: `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)`): `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)<br>`suspend actual fun read(buffer: <ERROR CLASS>, minToRead: `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)`): `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)<br>Perform a suspending read, the method will read n bytes ( minToRead &lt; n &lt;= buffer.remaining() ) and update the cursor |
| [write](write.html) | `suspend fun write(buffer: `[`MultiplatformBuffer`](../../-sok.-buffer/-multiplatform-buffer/index.html)`): `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)<br>`suspend actual fun write(buffer: <ERROR CLASS>): `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)<br>Perform a suspending write, the method will not return until all the data between buffer.cursor and buffer.limit are written. The socket use an internal write queue, allowing multiple threads to concurrently write. Backpressure mechanisms should be implemented by the developer to avoid having too much data in the queue. |

