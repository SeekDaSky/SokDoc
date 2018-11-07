---
title: BufferPool - sok
---

[sok](../../index.html) / [Sok.Buffer](../index.html) / [BufferPool](./index.html)

# BufferPool

`class BufferPool` [(source)](https://github.com/SeekDaSky/Sok/tree/master/common/sok-common/src/Sok/Buffer/BufferPool.kt#L21)

**Platform and version requirements:** Common

In order to avoid garbage collection pressure it is a common practice to pre-allocate objects that are known to be long-living
for a later use, Kotlin channels give us a great way to implement a quite straightforward object pool. The pool will allocate
all the buffers lazily when needed, this means that the pool will never suspend until reaching the maximum size.

This class is of course thread safe

We need to use a factory lambda to let the developer use a DirectByteBuffer pool on the JVM instead of a HeapByteBuffer one

### Constructors

| [&lt;init&gt;](-init-.html) | `BufferPool(maximumNumberOfBuffer: `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)`, bufferSize: `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)`, bufferBuilder: (bufferSize: `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)`) -> `[`MultiplatformBuffer`](../-multiplatform-buffer/index.html)` = { allocMultiplatformBuffer(bufferSize) })`<br>Creates an empty pool that will grow to the given maximum number of buffer if needed |

### Properties

| [bufferBuilder](buffer-builder.html) | `val bufferBuilder: (bufferSize: `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)`) -> `[`MultiplatformBuffer`](../-multiplatform-buffer/index.html)<br>lambda called when the pool need to allocate a buffer |
| [bufferSize](buffer-size.html) | `val bufferSize: `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)<br>parameter passed to the factory lambda, used to determine the size of the buffer to allocate |
| [maximumNumberOfBuffer](maximum-number-of-buffer.html) | `val maximumNumberOfBuffer: `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)<br>maximum number of buffer that the pool will allocate |

### Functions

| [freeBuffer](free-buffer.html) | `suspend fun freeBuffer(obj: `[`MultiplatformBuffer`](../-multiplatform-buffer/index.html)`): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)<br>Free the object in order to let another coroutine have it. If you forget to call this method the pool will empty itself and starve, blocking all coroutines calling requestBuffer() |
| [requestBuffer](request-buffer.html) | `suspend fun requestBuffer(): `[`MultiplatformBuffer`](../-multiplatform-buffer/index.html)<br>Fetch a buffer from the pool. If the pool as not reached its maximum size and that the channel si empty we can allocate the buffer instead of suspending. |

