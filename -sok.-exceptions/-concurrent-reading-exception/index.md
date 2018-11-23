---
title: ConcurrentReadingException - sok
---

[sok](../../index.html) / [Sok.Exceptions](../index.html) / [ConcurrentReadingException](./index.html)

# ConcurrentReadingException

`class ConcurrentReadingException : `[`SokException`](../-sok-exception/index.html) [(source)](https://github.com/SeekDaSky/Sok/tree/master/common/sok-common/src/Sok/Exceptions/Exceptions.kt#L64)

**Platform and version requirements:** Common

Exception thrown when trying to read the socket while another read call is executing

### Parameters

`message` - Message given by the exception when thrown

### Constructors

| [&lt;init&gt;](-init-.html) | `ConcurrentReadingException(message: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)` = "The socket si already being read")`<br>Exception thrown when trying to read the socket while another read call is executing |

