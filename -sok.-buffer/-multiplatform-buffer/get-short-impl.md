---
title: MultiplatformBuffer.getShortImpl - sok
---

[sok](../../index.html) / [Sok.Buffer](../index.html) / [MultiplatformBuffer](index.html) / [getShortImpl](./get-short-impl.html)

# getShortImpl

`protected abstract fun getShortImpl(index: `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)`? = null): `[`Short`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-short/index.html) [(source)](https://github.com/SeekDaSky/Sok/tree/master/common/sok-common/src/Sok/Buffer/MultiplatformBuffer.kt#L188)

**Platform and version requirements:** Common

Get the short at the current cursor position. If the index parameter is provided, the cursor will be ignored and not modified

### Parameters

`index` - index of the short, buffer.cursor is used if the index is null

**Return**
short

