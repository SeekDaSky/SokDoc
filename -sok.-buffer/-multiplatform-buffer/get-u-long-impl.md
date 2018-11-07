---
title: MultiplatformBuffer.getULongImpl - sok
---

[sok](../../index.html) / [Sok.Buffer](../index.html) / [MultiplatformBuffer](index.html) / [getULongImpl](./get-u-long-impl.html)

# getULongImpl

`protected abstract fun getULongImpl(index: `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)`? = null): <ERROR CLASS>` [(source)](https://github.com/SeekDaSky/Sok/tree/master/common/sok-common/src/Sok/Buffer/MultiplatformBuffer.kt#L263)

**Platform and version requirements:** Common

Get the unsigned long at the current cursor position. If the index parameter is provided, the cursor will be ignored and not modified

### Parameters

`index` - index of the long, buffer.cursor is used if the index is null

**Return**
long

