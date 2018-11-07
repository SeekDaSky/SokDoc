---
title: BufferPool.freeBuffer - sok
---

[sok](../../index.html) / [Sok.Buffer](../index.html) / [BufferPool](index.html) / [freeBuffer](./free-buffer.html)

# freeBuffer

`suspend fun freeBuffer(obj: `[`MultiplatformBuffer`](../-multiplatform-buffer/index.html)`): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) [(source)](https://github.com/SeekDaSky/Sok/tree/master/common/sok-common/src/Sok/Buffer/BufferPool.kt#L50)

**Platform and version requirements:** Common

Free the object in order to let another coroutine have it. If you forget to call this method the pool will empty
itself and starve, blocking all coroutines calling requestBuffer()

### Parameters

`obj` - Buffer to free