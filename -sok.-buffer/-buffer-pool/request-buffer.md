---
title: BufferPool.requestBuffer - sok
---

[sok](../../index.html) / [Sok.Buffer](../index.html) / [BufferPool](index.html) / [requestBuffer](./request-buffer.html)

# requestBuffer

`suspend fun requestBuffer(): `[`MultiplatformBuffer`](../-multiplatform-buffer/index.html) [(source)](https://github.com/SeekDaSky/Sok/tree/master/common/sok-common/src/Sok/Buffer/BufferPool.kt#L35)

**Platform and version requirements:** Common

Fetch a buffer from the pool. If the pool as not reached its maximum size and that the channel si empty we can allocate
the buffer instead of suspending.

**Return**
the requested buffer

