---
title: MultiplatformBuffer.putLong - sok
---

[sok](../../index.html) / [Sok.Buffer](../index.html) / [MultiplatformBuffer](index.html) / [putLong](./put-long.html)

# putLong

`fun putLong(value: `[`Long`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-long/index.html)`, index: `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)`? = null): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) [(source)](https://github.com/SeekDaSky/Sok/tree/master/common/sok-common/src/Sok/Buffer/MultiplatformBuffer.kt#L394)

**Platform and version requirements:** Common

Put the given long inside the buffer starting at the buffer cursor position. If the index parameter is provided, the
cursor will be ignored and not modified

### Parameters

`value` - long to put in the buffer

`index` - index of the long, buffer.cursor is used if the index is null