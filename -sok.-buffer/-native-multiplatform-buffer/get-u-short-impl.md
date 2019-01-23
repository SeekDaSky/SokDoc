---
title: NativeMultiplatformBuffer.getUShortImpl - sok
---

[sok](../../index.html) / [Sok.Buffer](../index.html) / [NativeMultiplatformBuffer](index.html) / [getUShortImpl](./get-u-short-impl.html)

# getUShortImpl

`fun getUShortImpl(index: `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)`?): <ERROR CLASS>` [(source)](https://github.com/SeekDaSky/Sok/tree/master/native/sok-native-linux/src/Sok/Buffer/NativeMultiplatformBuffer.kt#L128)

**Platform and version requirements:** Native

Get the unsigned short at the current cursor position. If the index parameter is provided, the cursor will be ignored and
not modified

### Parameters

`index` - index of the short, buffer.cursor is used if the index is null

**Return**
short

