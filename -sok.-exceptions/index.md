---
title: Sok.Exceptions - sok
---

[sok](../index.html) / [Sok.Exceptions](./index.html)

## Package Sok.Exceptions

**Platform and version requirements:** Common

Contains all the exception classes

### Exceptions

| [AddressInUseException](-address-in-use-exception/index.html)<br>(Common) | `class AddressInUseException : `[`SokException`](-sok-exception/index.html)<br>Exception thrown when trying to bind a socket to an address/port already bound |
| [BufferDestroyedException](-buffer-destroyed-exception/index.html)<br>(Common) | `class BufferDestroyedException : `[`SokException`](-sok-exception/index.html)<br>Exception thrown when trying to modify the buffer after the destroy() method was called |
| [BufferOverflowException](-buffer-overflow-exception/index.html)<br>(Common) | `class BufferOverflowException : `[`SokException`](-sok-exception/index.html)<br>Exception thrown when trying to put a value too large for the remaining space in the buffer |
| [BufferUnderflowException](-buffer-underflow-exception/index.html)<br>(Common) | `class BufferUnderflowException : `[`SokException`](-sok-exception/index.html)<br>Exception thrown when trying to read a value too large for the remaining space in the buffer |
| [CloseException](-close-exception/index.html)<br>(Common) | `open class CloseException : `[`SokException`](-sok-exception/index.html)<br>Parent class of the exceptions thrown when gracefully closing a socket |
| [ConcurrentReadingException](-concurrent-reading-exception/index.html)<br>(Common) | `class ConcurrentReadingException : `[`SokException`](-sok-exception/index.html)<br>Exception thrown when trying to read the socket while another read call is executing |
| [ConnectionRefusedException](-connection-refused-exception/index.html)<br>(Common) | `class ConnectionRefusedException : `[`SokException`](-sok-exception/index.html)<br>Exception thrown when a client tries to connect and fails |
| [ForceCloseException](-force-close-exception/index.html)<br>(Common) | `class ForceCloseException : `[`CloseException`](-close-exception/index.html)<br>Exception passed to the socket exception handler whent the socket is forcefully closed by a call to the `forceClose` method |
| [NormalCloseException](-normal-close-exception/index.html)<br>(Common) | `class NormalCloseException : `[`CloseException`](-close-exception/index.html)<br>Exception passed to the socket exception handler when the socket is gracefully closed by a call to the `close` method |
| [OptionNotSupportedException](-option-not-supported-exception/index.html)<br>(Common) | `class OptionNotSupportedException : `[`SokException`](-sok-exception/index.html)<br>Exception thrown when trying to get/set a socket option not supported on the platform |
| [PeerClosedException](-peer-closed-exception/index.html)<br>(Common) | `class PeerClosedException : `[`CloseException`](-close-exception/index.html)<br>Exception thrown when trying to perform an I/O on a closed socket |
| [SocketClosedException](-socket-closed-exception/index.html)<br>(Common) | `class SocketClosedException : `[`SokException`](-sok-exception/index.html)<br>Exception thrown when trying to perform an I/O on a closed socket |
| [SokException](-sok-exception/index.html)<br>(Common) | `open class SokException : `[`Exception`](http://docs.oracle.com/javase/6/docs/api/java/lang/Exception.html)<br>Parent class of any exception thrown by Sok |

### Functions

| [handleException](handle-exception.html)<br>(Common) | `fun <ERROR CLASS>.handleException(exception: `[`Throwable`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-throwable/index.html)`): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)<br>Extension function used to throw an exception in a particular `CoroutineExceptionHandler` without having to pass an `EmptyCoroutineContext` |

