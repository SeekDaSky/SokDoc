---
title: Selector - sok
---

[sok](../../index.html) / [Sok.Selector](../index.html) / [Selector](./index.html)

# Selector

`class Selector` [(source)](https://github.com/SeekDaSky/Sok/tree/master/jvm/sok-jvm/src/Sok/Selector/Selector.kt#L40)

**Platform and version requirements:** JVM, Native

The Sok Selector class helps to go from a crappy blocking NIO Selector interface to a nice coroutine based interface.
The Selector will take care of registrations to the underlying NIO Selector in a non-blocking and non-suspending way
in order to have the best performances possible. In order to do that (and because the NIO Selector is blocking) the
Selector have a single thread executor to which we will give "ticks" tasks, when a socket wants to register we will
pause the ticking, register and send a resume task to the executor, if the registration task is fast enough the ticking
will not be paused.

The Selector uses the SuspentionMap class to get and resume the suspention or execute the callback. There is two kinds
of operation for the SuspentionMap, resume the continuation and unregister the interest directly (for single read operations)
or execute a callback that will return whether or not we should unregister. The goal of those two "modes" is to reduce the
number of (expensive) interest update operations. The counterpart is that the Selector now execute user-code which can
greatly slow down the ticking rate, the developer should be careful.

### Constructors

| [&lt;init&gt;](-init-.html) | `Selector()`<br>The Sok Selector class helps to go from a crappy blocking NIO Selector interface to a nice coroutine based interface. The Selector will take care of registrations to the underlying NIO Selector in a non-blocking and non-suspending way in order to have the best performances possible. In order to do that (and because the NIO Selector is blocking) the Selector have a single thread executor to which we will give "ticks" tasks, when a socket wants to register we will pause the ticking, register and send a resume task to the executor, if the registration task is fast enough the ticking will not be paused. |

### Properties

| [isClosed](is-closed.html) | `var isClosed: `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)<br>is the Selector still running |
| [isInSelection](is-in-selection.html)<br>(Native) | `var isInSelection: `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)<br>is the selector in a selection loop |
| [numberOfChannel](number-of-channel.html)<br>(JVM) | `var numberOfChannel: `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)<br>Used for load balancing by the SelectorPool |

### Functions

| [close](close.html) | `fun close(): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)<br>Close the selector, close all SuspentionMap, cancel the main loop and close the thread |
| [register](register.html)<br>(JVM) | `fun register(channel: `[`SelectableChannel`](http://docs.oracle.com/javase/6/docs/api/java/nio/channels/SelectableChannel.html)`, interest: `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)`, attachment: `[`Any`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-any/index.html)`?): `[`SelectionKey`](http://docs.oracle.com/javase/6/docs/api/java/nio/channels/SelectionKey.html)<br>Register a `SelectableChannel` the NIO `Selector` and bind the attachment (`SuspentionMap`) |
| [updateInterest](update-interest.html)<br>(JVM) | `fun updateInterest(sk: `[`SelectionKey`](http://docs.oracle.com/javase/6/docs/api/java/nio/channels/SelectionKey.html)`, interest: `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)`): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)<br>Update the interest of a `SelectionKey` with the given `interest` |
| [wakeup](wakeup.html)<br>(JVM) | `fun wakeup(): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)<br>Wake the NIO selector up if needed to allow registrations |

### Companion Object Properties

| [defaultSelector](default-selector.html) | `val defaultSelector: <ERROR CLASS>`<br>default selector |
| [defaultSelectorPool](default-selector-pool.html)<br>(JVM) | `val defaultSelectorPool: <ERROR CLASS>`<br>default selector pool |
| [isSelectorPoolInit](is-selector-pool-init.html)<br>(JVM) | `var isSelectorPoolInit: `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)<br>is the selector pool initialized. |

### Companion Object Functions

| [closeSelectorAndWait](close-selector-and-wait.html)<br>(Native) | `suspend fun closeSelectorAndWait(): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)<br>Close the selector |
| [setDefaultScope](set-default-scope.html)<br>(Native) | `fun setDefaultScope(scope: <ERROR CLASS>): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)<br>Bind the Selector to a particular CoroutineScope, mainly used in order to prevent the event loop from exiting while te selector is still running |

