---
title: JSMultiplatformBuffer.toArray - sok
---

[sok](../../index.html) / [Sok.Buffer](../index.html) / [JSMultiplatformBuffer](index.html) / [toArray](./to-array.html)

# toArray

`fun toArray(): `[`ByteArray`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-byte-array/index.html) [(source)](https://github.com/SeekDaSky/Sok/tree/master/js/sok-js/src/Sok/Buffer/JSMultiplateformBuffer.kt#L249)

**Platform and version requirements:** JS

Get all the data between the start of the buffer and its limit, the data is copied and is not linked to the content
of the buffer. WARNING this behaviour is different from the ByteBuffer array() method, please read the documentation
carefully

**Return**
data copied from the start fo the buffer to the limit

