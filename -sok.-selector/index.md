---
title: Sok.Selector - sok
---

[sok](../index.html) / [Sok.Selector](./index.html)

## Package Sok.Selector

### Types

| [Interests](-interests/index.html)<br>(Native) | `enum class Interests`<br>Enum representing the possible interests of a `SelectionKey` |
| [Selector](-selector/index.html)<br>(JVM, Native) | `class Selector`<br>Class wrapping the NIO Selector class for a more "coroutine-friendly" approach. Each `SelectableCHannel` will have a `SuspentionMap` as attachment, this map contains all teh Continuations/Lambda to resume/call when an event come in. |
| [SelectorPool](-selector-pool/index.html)<br>(JVM) | `class SelectorPool`<br>A SelectorPool will order the Selectors by the number of channels registered. This allow us to do a basic load balancing between all the Selectors |

