---
title: NativeMultiplatformBuffer.getIntImpl - sok
---

[sok](../../index.html) / [Sok.Buffer](../index.html) / [NativeMultiplatformBuffer](index.html) / [getIntImpl](./get-int-impl.html)

# getIntImpl

`fun getIntImpl(index: `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)`?): `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html) [(source)](https://github.com/SeekDaSky/Sok/tree/master/native/sok-native-linux/src/Sok/Buffer/NativeMultiplatformBuffer.kt#L138)

**Platform and version requirements:** Native

Get the integer at the current cursor position. If the index parameter is provided, the cursor will be ignored and not modified

### Parameters

`index` - index of the int, buffer.cursor is used if the index is null

**Return**
int

