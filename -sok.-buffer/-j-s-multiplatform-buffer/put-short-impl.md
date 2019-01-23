---
title: JSMultiplatformBuffer.putShortImpl - sok
---

[sok](../../index.html) / [Sok.Buffer](../index.html) / [JSMultiplatformBuffer](index.html) / [putShortImpl](./put-short-impl.html)

# putShortImpl

`fun putShortImpl(value: `[`Short`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-short/index.html)`, index: `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)`?): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) [(source)](https://github.com/SeekDaSky/Sok/tree/master/js/sok-js/src/Sok/Buffer/JSMultiplateformBuffer.kt#L192)

**Platform and version requirements:** JS

Put the given short inside the buffer starting at the buffer cursor position. If the index parameter is provided, the
cursor will be ignored and not modified

### Parameters

`value` - short to put in the buffer

`index` - index of the short, buffer.cursor is used if the index is null