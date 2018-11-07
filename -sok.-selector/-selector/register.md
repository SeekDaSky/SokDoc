---
title: Selector.register - sok
---

[sok](../../index.html) / [Sok.Selector](../index.html) / [Selector](index.html) / [register](./register.html)

# register

`fun register(channel: `[`SelectableChannel`](http://docs.oracle.com/javase/6/docs/api/java/nio/channels/SelectableChannel.html)`, interest: `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)`, attachment: `[`Any`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-any/index.html)`?): `[`SelectionKey`](http://docs.oracle.com/javase/6/docs/api/java/nio/channels/SelectionKey.html) [(source)](https://github.com/SeekDaSky/Sok/tree/master/jvm/sok-jvm/src/Sok/Selector/Selector.kt#L212)

**Platform and version requirements:** JVM

Register a `SelectableChannel` the NIO `Selector` and bind the attachment (`SuspentionMap`)

### Parameters

`channel` - Channel to register

`interest` - Initial interest (0)

`attachment` - `SuspentionMap` attached to the channel

**Return**
NIO SelectionKey used by the SuspentionMap for registrations

