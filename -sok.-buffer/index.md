---
title: Sok.Buffer - sok
---

[sok](../index.html) / [Sok.Buffer](./index.html)

## Package Sok.Buffer

As Sok is buffer based, you need to use buffers to perform I/O operations. The primitive for that is the `MultiplatformBuffer` class. This package also contains a basic implementation of a buffer pool for object recycling.

### Types

| [BufferPool](-buffer-pool/index.html)<br>(Common) | `class BufferPool`<br>In order to avoid garbage collection pressure it is a common practice to pre-allocate objects that are known to be long-living for a later use, Kotlin channels give us a great way to implement a quite straightforward object pool. The pool will allocate all the buffers lazily when needed, this means that the pool will never suspend until reaching the maximum size. |
| [JSMultiplatformBuffer](-j-s-multiplatform-buffer/index.html)<br>(JS) | `class JSMultiplatformBuffer`<br>JS implementation of the `MultiplatformBuffer` class |
| [JVMMultiplatformBuffer](-j-v-m-multiplatform-buffer/index.html)<br>(JVM) | `class JVMMultiplatformBuffer`<br>JVM implementation of the `MultiplatformBuffer` class |
| [MultiplatformBuffer](-multiplatform-buffer/index.html)<br>(Common) | `abstract class MultiplatformBuffer`<br>A `MultiplatformBuffer` is the primitive type of Sok, you will use it to receive, send and manipulate data |
| [NativeMultiplatformBuffer](-native-multiplatform-buffer/index.html)<br>(Native) | `class NativeMultiplatformBuffer`<br>Native implementation of the `MultiplatformBuffer` class |

### Functions

| [allocDirectMultiplatformBuffer](alloc-direct-multiplatform-buffer.html)<br>(JVM) | `fun allocDirectMultiplatformBuffer(size: `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)`): <ERROR CLASS>`<br>Allocate a new MultiplatformBuffer. The buffer is not zeroed, be careful. |
| [allocMultiplatformBuffer](alloc-multiplatform-buffer.html) | `expect fun allocMultiplatformBuffer(size: `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)`): `[`MultiplatformBuffer`](-multiplatform-buffer/index.html)<br>Allocate a new MultiplatformBuffer. The buffer is not zeroed, be careful. |
| [wrapMultiplatformBuffer](wrap-multiplatform-buffer.html) | `expect fun wrapMultiplatformBuffer(array: `[`ByteArray`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-byte-array/index.html)`): `[`MultiplatformBuffer`](-multiplatform-buffer/index.html)<br>Wrap the array with a MultiplatformBuffer. The data will not be copied and the array will be linked to the MultiplatformBuffer class`fun wrapMultiplatformBuffer(array: `[`ByteBuffer`](http://docs.oracle.com/javase/6/docs/api/java/nio/ByteBuffer.html)`): <ERROR CLASS>`<br>Make a MultiplatformBuffer that use a given ByteBuffer. |

