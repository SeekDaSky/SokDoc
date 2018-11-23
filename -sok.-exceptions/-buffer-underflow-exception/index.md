---
title: BufferUnderflowException - sok
---

[sok](../../index.html) / [Sok.Exceptions](../index.html) / [BufferUnderflowException](./index.html)

# BufferUnderflowException

`class BufferUnderflowException : `[`SokException`](../-sok-exception/index.html) [(source)](https://github.com/SeekDaSky/Sok/tree/master/common/sok-common/src/Sok/Exceptions/Exceptions.kt#L94)

**Platform and version requirements:** Common

Exception thrown when trying to read a value too large for the remaining space in the buffer

### Parameters

`message` - Message given by the exception when thrown

### Constructors

| [&lt;init&gt;](-init-.html) | `BufferUnderflowException(message: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)` = "There is not enough remaining data in the buffer to perform the read operation")`<br>Exception thrown when trying to read a value too large for the remaining space in the buffer |

