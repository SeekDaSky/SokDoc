---
title: MultiplatformBuffer.toArray - sok
---

[sok](../../index.html) / [Sok.Buffer](../index.html) / [MultiplatformBuffer](index.html) / [toArray](./to-array.html)

# toArray

`abstract fun toArray(): `[`ByteArray`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-byte-array/index.html) [(source)](https://github.com/SeekDaSky/Sok/tree/master/common/sok-common/src/Sok/Buffer/MultiplatformBuffer.kt#L416)

**Platform and version requirements:** Common

Get all the data between the start of the buffer and its limit, the data is copied and is not linked to the content
of the buffer. WARNING this behaviour is different from the ByteBuffer array() method, please read the documentation
carefully

**Return**
data copied from the start fo the buffer to the limit

