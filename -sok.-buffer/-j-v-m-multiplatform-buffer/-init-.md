---
title: JVMMultiplatformBuffer.<init> - sok
---

[sok](../../index.html) / [Sok.Buffer](../index.html) / [JVMMultiplatformBuffer](index.html) / [&lt;init&gt;](./-init-.html)

# &lt;init&gt;

`JVMMultiplatformBuffer(size: `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)`)`

**Platform and version requirements:** JVM

Allocate a new MultiplatformBuffer

### Parameters

`size` - size of the buffer`JVMMultiplatformBuffer(array: `[`ByteArray`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-byte-array/index.html)`)`

**Platform and version requirements:** JVM

Create a new MultiplatformBuffer wrapping a byteArray , thus avoiding copy

### Parameters

`array` - array wrapped`JVMMultiplatformBuffer(array: `[`ByteBuffer`](http://docs.oracle.com/javase/6/docs/api/java/nio/ByteBuffer.html)`)`

**Platform and version requirements:** JVM

Create a MultiplatformBuffer with a specific NIO ByteBuffer

### Parameters

`NIO` - ByteBuffer