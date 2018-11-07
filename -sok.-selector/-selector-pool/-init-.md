---
title: SelectorPool.<init> - sok
---

[sok](../../index.html) / [Sok.Selector](../index.html) / [SelectorPool](index.html) / [&lt;init&gt;](./-init-.html)

# &lt;init&gt;

`SelectorPool(NbrOfSelector: `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)`)`

**Platform and version requirements:** JVM

A SelectorPool will order the Selectors by the number of channels registered. This allow us to do a basic load balancing between all the Selectors

