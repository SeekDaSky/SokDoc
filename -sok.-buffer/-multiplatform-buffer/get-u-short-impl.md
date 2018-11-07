---
title: MultiplatformBuffer.getUShortImpl - sok
---

[sok](../../index.html) / [Sok.Buffer](../index.html) / [MultiplatformBuffer](index.html) / [getUShortImpl](./get-u-short-impl.html)

# getUShortImpl

`protected abstract fun getUShortImpl(index: `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)`? = null): <ERROR CLASS>` [(source)](https://github.com/SeekDaSky/Sok/tree/master/common/sok-common/src/Sok/Buffer/MultiplatformBuffer.kt#L177)

**Platform and version requirements:** Common

Get the unsigned short at the current cursor position. If the index parameter is provided, the cursor will be ignored and
not modified

### Parameters

`index` - index of the short, buffer.cursor is used if the index is null

**Return**
short

