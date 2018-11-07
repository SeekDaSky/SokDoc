---
title: SelectorPool - sok
---

[sok](../../index.html) / [Sok.Selector](../index.html) / [SelectorPool](./index.html)

# SelectorPool

`class SelectorPool` [(source)](https://github.com/SeekDaSky/Sok/tree/master/jvm/sok-jvm/src/Sok/Selector/SelectorPool.kt#L15)

**Platform and version requirements:** JVM

A SelectorPool will order the Selectors by the number of channels registered. This allow us to do a basic load balancing between all the Selectors

### Constructors

| [&lt;init&gt;](-init-.html) | `SelectorPool(NbrOfSelector: `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)`)`<br>A SelectorPool will order the Selectors by the number of channels registered. This allow us to do a basic load balancing between all the Selectors |

### Properties

| [isClosed](is-closed.html) | `var isClosed: `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)<br>state of the pool |

### Functions

| [close](close.html) | `fun close(): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)<br>Close the pool and all the selectors inside it |
| [getLessbusySelector](get-lessbusy-selector.html) | `suspend fun getLessbusySelector(): `[`Selector`](../-selector/index.html)<br>Get the less busy selector (first in the pool list), the method is suspending because an actor is used behind the scene to allow multiple threads accessing the pool and still get the right selector. This may not be the most efficient way to do it but a socket get a selector once so it is not critical. |

