---
title: JSMultiplatformBuffer.putIntImpl - sok
---

[sok](../../index.html) / [Sok.Buffer](../index.html) / [JSMultiplatformBuffer](index.html) / [putIntImpl](./put-int-impl.html)

# putIntImpl

`fun putIntImpl(value: `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)`, index: `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)`?): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) [(source)](https://github.com/SeekDaSky/Sok/tree/master/js/sok-js/src/Sok/Buffer/JSMultiplateformBuffer.kt#L208)

**Platform and version requirements:** JS

Put the given integer inside the buffer starting at the buffer cursor position. If the index parameter is provided, the
cursor will be ignored and not modified

### Parameters

`value` - int to put in the buffer

`index` - index of the int, buffer.cursor is used if the index is null