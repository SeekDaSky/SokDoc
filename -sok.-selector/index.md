---
title: Sok.Selector - sok
---

[sok](../index.html) / [Sok.Selector](./index.html)

## Package Sok.Selector

Internal package containing selector-related classes for JVM and Native platforms. The only usefull methods for a developper are the `Seletor` companion object methods.

### Types

| [Interests](-interests/index.html)<br>(Native) | `enum class Interests`<br>Enum representing the possible interests of a `SelectionKey` |
| [Selector](-selector/index.html)<br>(JVM, Native) | `class Selector`<br>The Sok Selector class helps to go from a crappy blocking NIO Selector interface to a nice coroutine based interface. The Selector will take care of registrations to the underlying NIO Selector in a non-blocking and non-suspending way in order to have the best performances possible. In order to do that (and because the NIO Selector is blocking) the Selector have a single thread executor to which we will give "ticks" tasks, when a socket wants to register we will pause the ticking, register and send a resume task to the executor, if the registration task is fast enough the ticking will not be paused. |
| [SelectorPool](-selector-pool/index.html)<br>(JVM) | `class SelectorPool`<br>A SelectorPool will order the Selectors by the number of channels registered. This allow us to do a basic load balancing between all the Selectors |

