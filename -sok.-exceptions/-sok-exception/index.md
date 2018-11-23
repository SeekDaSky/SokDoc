---
title: SokException - sok
---

[sok](../../index.html) / [Sok.Exceptions](../index.html) / [SokException](./index.html)

# SokException

`open class SokException : `[`Exception`](http://docs.oracle.com/javase/6/docs/api/java/lang/Exception.html) [(source)](https://github.com/SeekDaSky/Sok/tree/master/common/sok-common/src/Sok/Exceptions/Exceptions.kt#L11)

**Platform and version requirements:** Common

Parent class of any exception thrown by Sok

### Parameters

`message` - Message given by the exception when thrown

### Constructors

| [&lt;init&gt;](-init-.html) | `SokException(message: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)` = "Something unexpected happened")`<br>Parent class of any exception thrown by Sok |

### Inheritors

| [AddressInUseException](../-address-in-use-exception/index.html)<br>(Common) | `class AddressInUseException : `[`SokException`](./index.html)<br>Exception thrown when trying to bind a socket to an address/port already bound |
| [BufferDestroyedException](../-buffer-destroyed-exception/index.html)<br>(Common) | `class BufferDestroyedException : `[`SokException`](./index.html)<br>Exception thrown when trying to modify the buffer after the destroy() method was called |
| [BufferOverflowException](../-buffer-overflow-exception/index.html)<br>(Common) | `class BufferOverflowException : `[`SokException`](./index.html)<br>Exception thrown when trying to put a value too large for the remaining space in the buffer |
| [BufferUnderflowException](../-buffer-underflow-exception/index.html)<br>(Common) | `class BufferUnderflowException : `[`SokException`](./index.html)<br>Exception thrown when trying to read a value too large for the remaining space in the buffer |
| [CloseException](../-close-exception/index.html)<br>(Common) | `open class CloseException : `[`SokException`](./index.html)<br>Parent class of the exceptions thrown when gracefully closing a socket |
| [ConcurrentReadingException](../-concurrent-reading-exception/index.html)<br>(Common) | `class ConcurrentReadingException : `[`SokException`](./index.html)<br>Exception thrown when trying to read the socket while another read call is executing |
| [ConnectionRefusedException](../-connection-refused-exception/index.html)<br>(Common) | `class ConnectionRefusedException : `[`SokException`](./index.html)<br>Exception thrown when a client tries to connect and fails |
| [OptionNotSupportedException](../-option-not-supported-exception/index.html)<br>(Common) | `class OptionNotSupportedException : `[`SokException`](./index.html)<br>Exception thrown when trying to get/set a socket option not supported on the platform |
| [SocketClosedException](../-socket-closed-exception/index.html)<br>(Common) | `class SocketClosedException : `[`SokException`](./index.html)<br>Exception thrown when trying to perform an I/O on a closed socket |

