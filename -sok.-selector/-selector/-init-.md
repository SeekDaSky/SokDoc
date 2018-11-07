---
title: Selector.<init> - sok
---

[sok](../../index.html) / [Sok.Selector](../index.html) / [Selector](index.html) / [&lt;init&gt;](./-init-.html)

# &lt;init&gt;

`Selector()`

**Platform and version requirements:** JVM, Native

Class wrapping the NIO Selector class for a more "coroutine-friendly" approach. Each `SelectableCHannel` will have a `SuspentionMap` as
attachment, this map contains all teh Continuations/Lambda to resume/call when an event come in.

Sockets register quite frequently and as the NIO Selector class blocks any registration while selecting we have to implement a way to
synchronize registrations and the Selector class. This is done by sharing the `CoroutineScope` of the Selector to the `SuspentionMap`
classes, this way the `SuspentionMap` is able to launch coroutine on the Selector Thread, thus ensuring mutual-exclusion.

To reduce the number of registration, a socket may register for a unknown number of event. If so the selector will call a lambda after
each event and this lambda will return if the Selector should keep the registration or not. This method slow down the selector but
the performance gain is worth it.

