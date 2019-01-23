---
title: MultiplatformBuffer.putInt - sok
---

[sok](../../index.html) / [Sok.Buffer](../index.html) / [MultiplatformBuffer](index.html) / [putInt](./put-int.html)

# putInt

`fun putInt(value: `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)`, index: `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)`? = null): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) [(source)](https://github.com/SeekDaSky/Sok/tree/master/common/sok-common/src/Sok/Buffer/MultiplatformBuffer.kt#L372)

**Platform and version requirements:** Common

Put the given integer inside the buffer starting at the buffer cursor position. If the index parameter is provided, the
cursor will be ignored and not modified

### Parameters

`value` - int to put in the buffer

`index` - index of the int, buffer.cursor is used if the index is null