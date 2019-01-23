---
title: JVMMultiplatformBuffer.getBytesImpl - sok
---

[sok](../../index.html) / [Sok.Buffer](../index.html) / [JVMMultiplatformBuffer](index.html) / [getBytesImpl](./get-bytes-impl.html)

# getBytesImpl

`fun getBytesImpl(length: `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)`, index: `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)`?): `[`ByteArray`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-byte-array/index.html) [(source)](https://github.com/SeekDaSky/Sok/tree/master/jvm/sok-jvm/src/Sok/Buffer/JVMMultiplatformBuffer.kt#L63)

**Platform and version requirements:** JVM

Get an array of bytes of a given length starting at the current buffer cursor position. If the index parameter is provided, the
cursor will be ignored and not modified

### Parameters

`length` - amount of data to get

`index` - index of the first byte, buffer.cursor is used if the index is null

**Return**
data copied from the buffer

`fun getBytesImpl(array: `[`ByteArray`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-byte-array/index.html)`, index: `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)`?, destinationOffset: `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)`, length: `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)`): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) [(source)](https://github.com/SeekDaSky/Sok/tree/master/jvm/sok-jvm/src/Sok/Buffer/JVMMultiplatformBuffer.kt#L79)

**Platform and version requirements:** JVM

Copy bytes into the array starting from the current cursor position or given index. You can start the copy with an offset in the
destination array and specify the number of byte you want to be copied.

### Parameters

`array` - destination array

`index` - index of the first byte, buffer.cursor is used if the index is null

`destinationOffset` - The offset within the array of the first byte to be written

`length` - amount of data to copy