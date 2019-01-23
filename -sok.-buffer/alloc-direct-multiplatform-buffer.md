---
title: allocDirectMultiplatformBuffer - sok
---

[sok](../index.html) / [Sok.Buffer](index.html) / [allocDirectMultiplatformBuffer](./alloc-direct-multiplatform-buffer.html)

# allocDirectMultiplatformBuffer

`fun allocDirectMultiplatformBuffer(size: `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)`): <ERROR CLASS>` [(source)](https://github.com/SeekDaSky/Sok/tree/master/jvm/sok-jvm/src/Sok/Buffer/JVMMultiplatformBuffer.kt#L303)

**Platform and version requirements:** JVM

Allocate a new MultiplatformBuffer. The buffer is not zeroed, be careful.

The create buffer will use a DirectByteBuffer instead of a HeapByteBuffer, please read the Java NIO documentation
to know the difference between the two

### Parameters

`size` - size of the buffer

**Return**
allocated buffer

