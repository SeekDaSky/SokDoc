---
title: MultiplatformBuffer.getUInt - sok
---

[sok](../../index.html) / [Sok.Buffer](../index.html) / [MultiplatformBuffer](index.html) / [getUInt](./get-u-int.html)

# getUInt

`fun getUInt(index: `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)`? = null): <ERROR CLASS>` [(source)](https://github.com/SeekDaSky/Sok/tree/master/common/sok-common/src/Sok/Buffer/MultiplatformBuffer.kt#L207)

**Platform and version requirements:** Common

Get the unsigned integer at the current cursor position. If the index parameter is provided, the cursor will be ignored and
not modified

### Parameters

`index` - index of the int, buffer.cursor is used if the index is null

**Return**
int

