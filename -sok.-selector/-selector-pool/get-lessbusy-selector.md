---
title: SelectorPool.getLessbusySelector - sok
---

[sok](../../index.html) / [Sok.Selector](../index.html) / [SelectorPool](index.html) / [getLessbusySelector](./get-lessbusy-selector.html)

# getLessbusySelector

`suspend fun getLessbusySelector(): `[`Selector`](../-selector/index.html) [(source)](https://github.com/SeekDaSky/Sok/tree/master/jvm/sok-jvm/src/Sok/Selector/SelectorPool.kt#L52)

**Platform and version requirements:** JVM

Get the less busy selector (first in the pool list), the method is suspending because an actor is used behind the scene to
allow multiple threads accessing the pool and still get the right selector. This may not be the most efficient way to do it
but a socket get a selector once so it is not critical.

**Return**
the less busy selector

