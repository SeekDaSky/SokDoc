---
title: JVMMultiplatformBuffer.putBytesImpl - sok
---

[sok](../../index.html) / [Sok.Buffer](../index.html) / [JVMMultiplatformBuffer](index.html) / [putBytesImpl](./put-bytes-impl.html)

# putBytesImpl

`fun putBytesImpl(array: `[`ByteArray`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-byte-array/index.html)`, index: `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)`?): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) [(source)](https://github.com/SeekDaSky/Sok/tree/master/jvm/sok-jvm/src/Sok/Buffer/JVMMultiplatformBuffer.kt#L164)

**Platform and version requirements:** JVM

Put the given byte array inside the buffer starting at the buffer cursor position. If the index parameter is provided, the
cursor will be ignored and not modified

### Parameters

`array` - data to put in the buffer

`index` - index of the first byte, buffer.cursor is used if the index is null