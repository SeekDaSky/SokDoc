---
title: JSMultiplatformBuffer.putByteImpl - sok
---

[sok](../../index.html) / [Sok.Buffer](../index.html) / [JSMultiplatformBuffer](index.html) / [putByteImpl](./put-byte-impl.html)

# putByteImpl

`fun putByteImpl(value: `[`Byte`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-byte/index.html)`, index: `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)`?): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) [(source)](https://github.com/SeekDaSky/Sok/tree/master/js/sok-js/src/Sok/Buffer/JSMultiplateformBuffer.kt#L166)

**Platform and version requirements:** JS

Put the given byte inside the buffer at the buffer cursor position. If the index parameter is provided, the
cursor will be ignored and not modified

### Parameters

`value` - byte to put in the buffer

`index` - index of the byte, buffer.cursor is used if the index is null