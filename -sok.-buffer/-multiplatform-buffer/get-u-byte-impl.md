---
title: MultiplatformBuffer.getUByteImpl - sok
---

[sok](../../index.html) / [Sok.Buffer](../index.html) / [MultiplatformBuffer](index.html) / [getUByteImpl](./get-u-byte-impl.html)

# getUByteImpl

`protected abstract fun getUByteImpl(index: `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)`? = null): <ERROR CLASS>` [(source)](https://github.com/SeekDaSky/Sok/tree/master/common/sok-common/src/Sok/Buffer/MultiplatformBuffer.kt#L167)

**Platform and version requirements:** Common

Get the unsigned byte at the current cursor position. If the index parameter is provided, the cursor will be ignored and
not modified

### Parameters

`index` - index of the byte, buffer.cursor is used if the index is null

**Return**
byte

