---
title: BufferDestroyedException - sok
---

[sok](../../index.html) / [Sok.Exceptions](../index.html) / [BufferDestroyedException](./index.html)

# BufferDestroyedException

`class BufferDestroyedException : `[`SokException`](../-sok-exception/index.html) [(source)](https://github.com/SeekDaSky/Sok/tree/master/common/sok-common/src/Sok/Exceptions/Exceptions.kt#L101)

**Platform and version requirements:** Common

Exception thrown when trying to modify the buffer after the destroy() method was called

### Parameters

`message` - Message given by the exception when thrown

### Constructors

| [&lt;init&gt;](-init-.html) | `BufferDestroyedException(message: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)` = "The buffer is destroyed an no operation should be done with it")`<br>Exception thrown when trying to modify the buffer after the destroy() method was called |

