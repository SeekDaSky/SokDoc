---
title: NativeMultiplatformBuffer.toArray - sok
---

[sok](../../index.html) / [Sok.Buffer](../index.html) / [NativeMultiplatformBuffer](index.html) / [toArray](./to-array.html)

# toArray

`fun toArray(): `[`ByteArray`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-byte-array/index.html) [(source)](https://github.com/SeekDaSky/Sok/tree/master/native/sok-native-linux/src/Sok/Buffer/NativeMultiplatformBuffer.kt#L263)

**Platform and version requirements:** Native

Get all the data between the start of the buffer and its limit, the data is copied and is not linked to the content
of the buffer. WARNING this behaviour is different from the ByteBuffer array() method, please read the documentation
carefully

**Return**
data copied from the start fo the buffer to the limit

