---
title: MultiplatformBuffer.putByte - sok
---

[sok](../../index.html) / [Sok.Buffer](../index.html) / [MultiplatformBuffer](index.html) / [putByte](./put-byte.html)

# putByte

`fun putByte(value: `[`Byte`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-byte/index.html)`, index: `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)`? = null): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) [(source)](https://github.com/SeekDaSky/Sok/tree/master/common/sok-common/src/Sok/Buffer/MultiplatformBuffer.kt#L328)

**Platform and version requirements:** Common

Put the given byte inside the buffer at the buffer cursor position. If the index parameter is provided, the
cursor will be ignored and not modified

### Parameters

`value` - byte to put in the buffer

`index` - index of the byte, buffer.cursor is used if the index is null