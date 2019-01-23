---
title: wrapMultiplatformBuffer - sok
---

[sok](../index.html) / [Sok.Buffer](index.html) / [wrapMultiplatformBuffer](./wrap-multiplatform-buffer.html)

# wrapMultiplatformBuffer

`expect fun wrapMultiplatformBuffer(array: `[`ByteArray`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-byte-array/index.html)`): `[`MultiplatformBuffer`](-multiplatform-buffer/index.html) [(source)](https://github.com/SeekDaSky/Sok/tree/master/common/sok-common/src/Sok/Buffer/MultiplatformBuffer.kt#L511)

Wrap the array with a MultiplatformBuffer. The data will not be copied and the array will be linked to the
MultiplatformBuffer class

### Parameters

`array` - array to wrap

**Return**
buffer

`fun wrapMultiplatformBuffer(array: `[`ByteBuffer`](http://docs.oracle.com/javase/6/docs/api/java/nio/ByteBuffer.html)`): <ERROR CLASS>` [(source)](https://github.com/SeekDaSky/Sok/tree/master/jvm/sok-jvm/src/Sok/Buffer/JVMMultiplatformBuffer.kt#L324)

**Platform and version requirements:** JVM

Make a MultiplatformBuffer that use a given ByteBuffer.

### Parameters

`array` - array to wrap

**Return**
buffer

