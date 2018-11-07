---
title: JSMultiplatformBuffer.getBytesImpl - sok
---

[sok](../../index.html) / [Sok.Buffer](../index.html) / [JSMultiplatformBuffer](index.html) / [getBytesImpl](./get-bytes-impl.html)

# getBytesImpl

`fun getBytesImpl(length: `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)`, index: `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)`?): `[`ByteArray`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-byte-array/index.html) [(source)](https://github.com/SeekDaSky/Sok/tree/master/js/sok-js/src/Sok/Buffer/JSMultiplateformBuffer.kt#L55)

**Platform and version requirements:** JS

Get an array of bytes of a given length starting at the current buffer cursor position. If the index parameter is provided, the
cursor will be ignored and not modified

### Parameters

`length` - amount of data to get

`index` - index of the first byte, buffer.cursor is used if the index is null

**Return**
data copied from the buffer

