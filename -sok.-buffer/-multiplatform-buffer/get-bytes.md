---
title: MultiplatformBuffer.getBytes - sok
---

[sok](../../index.html) / [Sok.Buffer](../index.html) / [MultiplatformBuffer](index.html) / [getBytes](./get-bytes.html)

# getBytes

`fun getBytes(length: `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)`, index: `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)`? = null): `[`ByteArray`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-byte-array/index.html) [(source)](https://github.com/SeekDaSky/Sok/tree/master/common/sok-common/src/Sok/Buffer/MultiplatformBuffer.kt#L94)

**Platform and version requirements:** Common

Get an array of bytes of a given length starting at the current buffer cursor position. If the index parameter is provided, the
cursor will be ignored and not modified

### Parameters

`length` - amount of data to get

`index` - index of the first byte, buffer.cursor is used if the index is null

**Return**
data copied from the buffer

