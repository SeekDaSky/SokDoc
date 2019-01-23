---
title: NativeMultiplatformBuffer.putLongImpl - sok
---

[sok](../../index.html) / [Sok.Buffer](../index.html) / [NativeMultiplatformBuffer](index.html) / [putLongImpl](./put-long-impl.html)

# putLongImpl

`fun putLongImpl(value: `[`Long`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-long/index.html)`, index: `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)`?): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) [(source)](https://github.com/SeekDaSky/Sok/tree/master/native/sok-native-linux/src/Sok/Buffer/NativeMultiplatformBuffer.kt#L247)

**Platform and version requirements:** Native

Put the given long inside the buffer starting at the buffer cursor position. If the index parameter is provided, the
cursor will be ignored and not modified

### Parameters

`value` - long to put in the buffer

`index` - index of the long, buffer.cursor is used if the index is null