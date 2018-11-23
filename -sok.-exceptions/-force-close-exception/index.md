---
title: ForceCloseException - sok
---

[sok](../../index.html) / [Sok.Exceptions](../index.html) / [ForceCloseException](./index.html)

# ForceCloseException

`class ForceCloseException : `[`CloseException`](../-close-exception/index.html) [(source)](https://github.com/SeekDaSky/Sok/tree/master/common/sok-common/src/Sok/Exceptions/Exceptions.kt#L34)

**Platform and version requirements:** Common

Exception passed to the socket exception handler whent the socket is forcefully closed by a call to the `forceClose` method

### Parameters

`message` - Message given by the exception when thrown

### Constructors

| [&lt;init&gt;](-init-.html) | `ForceCloseException(message: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)` = "The socket was forcefully closed")`<br>Exception passed to the socket exception handler whent the socket is forcefully closed by a call to the `forceClose` method |

