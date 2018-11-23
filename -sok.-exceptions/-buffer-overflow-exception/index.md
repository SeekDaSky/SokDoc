---
title: BufferOverflowException - sok
---

[sok](../../index.html) / [Sok.Exceptions](../index.html) / [BufferOverflowException](./index.html)

# BufferOverflowException

`class BufferOverflowException : `[`SokException`](../-sok-exception/index.html) [(source)](https://github.com/SeekDaSky/Sok/tree/master/common/sok-common/src/Sok/Exceptions/Exceptions.kt#L87)

**Platform and version requirements:** Common

Exception thrown when trying to put a value too large for the remaining space in the buffer

### Parameters

`message` - Message given by the exception when thrown

### Constructors

| [&lt;init&gt;](-init-.html) | `BufferOverflowException(message: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)` = "There is not enough remaining space in the buffer to perform the write operation")`<br>Exception thrown when trying to put a value too large for the remaining space in the buffer |

