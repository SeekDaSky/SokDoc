---
title: JVMMultiplatformBuffer.destroy - sok
---

[sok](../../index.html) / [Sok.Buffer](../index.html) / [JVMMultiplatformBuffer](index.html) / [destroy](./destroy.html)

# destroy

`fun destroy(): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) [(source)](https://github.com/SeekDaSky/Sok/tree/master/jvm/sok-jvm/src/Sok/Buffer/JVMMultiplatformBuffer.kt#L269)

**Platform and version requirements:** JVM

Destroy the ByteBuffer, you cannot call any method on the buffer after calling destroy. This method MUST be called on native platforms
in order to free/unpin memory but you can skip it on any other platform

