---
title: MultiplatformBuffer.getIntImpl - sok
---

[sok](../../index.html) / [Sok.Buffer](../index.html) / [MultiplatformBuffer](index.html) / [getIntImpl](./get-int-impl.html)

# getIntImpl

`protected abstract fun getIntImpl(index: `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)`? = null): `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html) [(source)](https://github.com/SeekDaSky/Sok/tree/master/common/sok-common/src/Sok/Buffer/MultiplatformBuffer.kt#L232)

**Platform and version requirements:** Common

Get the integer at the current cursor position. If the index parameter is provided, the cursor will be ignored and not modified

### Parameters

`index` - index of the int, buffer.cursor is used if the index is null

**Return**
int

