---
title: JVMMultiplatformBuffer.getUShortImpl - sok
---

[sok](../../index.html) / [Sok.Buffer](../index.html) / [JVMMultiplatformBuffer](index.html) / [getUShortImpl](./get-u-short-impl.html)

# getUShortImpl

`fun getUShortImpl(index: `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)`?): <ERROR CLASS>` [(source)](https://github.com/SeekDaSky/Sok/tree/master/jvm/sok-jvm/src/Sok/Buffer/JVMMultiplatformBuffer.kt#L98)

**Platform and version requirements:** JVM

Get the unsigned short at the current cursor position. If the index parameter is provided, the cursor will be ignored and
not modified

### Parameters

`index` - index of the short, buffer.cursor is used if the index is null

**Return**
short

