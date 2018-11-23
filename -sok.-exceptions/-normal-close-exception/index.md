---
title: NormalCloseException - sok
---

[sok](../../index.html) / [Sok.Exceptions](../index.html) / [NormalCloseException](./index.html)

# NormalCloseException

`class NormalCloseException : `[`CloseException`](../-close-exception/index.html) [(source)](https://github.com/SeekDaSky/Sok/tree/master/common/sok-common/src/Sok/Exceptions/Exceptions.kt#L27)

**Platform and version requirements:** Common

Exception passed to the socket exception handler when the socket is gracefully closed by a call to the `close` method

### Parameters

`message` - Message given by the exception when thrown

### Constructors

| [&lt;init&gt;](-init-.html) | `NormalCloseException(message: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)` = "The socket was gracefully closed")`<br>Exception passed to the socket exception handler when the socket is gracefully closed by a call to the `close` method |

