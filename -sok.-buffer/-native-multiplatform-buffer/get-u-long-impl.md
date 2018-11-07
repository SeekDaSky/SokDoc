---
title: NativeMultiplatformBuffer.getULongImpl - sok
---

[sok](../../index.html) / [Sok.Buffer](../index.html) / [NativeMultiplatformBuffer](index.html) / [getULongImpl](./get-u-long-impl.html)

# getULongImpl

`fun getULongImpl(index: `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)`?): <ERROR CLASS>` [(source)](https://github.com/SeekDaSky/Sok/tree/master/native/sok-native-linux/src/Sok/Buffer/NativeMultiplatformBuffer.kt#L153)

**Platform and version requirements:** Native

Get the unsigned long at the current cursor position. If the index parameter is provided, the cursor will be ignored and not modified

### Parameters

`index` - index of the long, buffer.cursor is used if the index is null

**Return**
long

