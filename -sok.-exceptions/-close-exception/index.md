---
title: CloseException - sok
---

[sok](../../index.html) / [Sok.Exceptions](../index.html) / [CloseException](./index.html)

# CloseException

`open class CloseException : `[`SokException`](../-sok-exception/index.html) [(source)](https://github.com/SeekDaSky/Sok/tree/master/common/sok-common/src/Sok/Exceptions/Exceptions.kt#L20)

**Platform and version requirements:** Common

Parent class of the exceptions thrown when gracefully closing a socket

### Parameters

`message` - Message given by the exception when thrown

### Constructors

| [&lt;init&gt;](-init-.html) | `CloseException(message: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)` = "The socket was closed")`<br>Parent class of the exceptions thrown when gracefully closing a socket |

### Inheritors

| [ForceCloseException](../-force-close-exception/index.html)<br>(Common) | `class ForceCloseException : `[`CloseException`](./index.html)<br>Exception passed to the socket exception handler whent the socket is forcefully closed by a call to the `forceClose` method |
| [NormalCloseException](../-normal-close-exception/index.html)<br>(Common) | `class NormalCloseException : `[`CloseException`](./index.html)<br>Exception passed to the socket exception handler when the socket is gracefully closed by a call to the `close` method |
| [PeerClosedException](../-peer-closed-exception/index.html)<br>(Common) | `class PeerClosedException : `[`CloseException`](./index.html)<br>Exception thrown when trying to perform an I/O on a closed socket |

