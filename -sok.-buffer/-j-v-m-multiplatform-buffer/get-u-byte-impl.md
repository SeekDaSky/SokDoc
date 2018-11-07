---
title: JVMMultiplatformBuffer.getUByteImpl - sok
---

[sok](../../index.html) / [Sok.Buffer](../index.html) / [JVMMultiplatformBuffer](index.html) / [getUByteImpl](./get-u-byte-impl.html)

# getUByteImpl

`fun getUByteImpl(index: `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)`?): <ERROR CLASS>` [(source)](https://github.com/SeekDaSky/Sok/tree/master/jvm/sok-jvm/src/Sok/Buffer/JVMMultiplatformBuffer.kt#L77)

**Platform and version requirements:** JVM

Get the unsigned byte at the current cursor position. If the index parameter is provided, the cursor will be ignored and
not modified

### Parameters

`index` - index of the byte, buffer.cursor is used if the index is null

**Return**
byte

