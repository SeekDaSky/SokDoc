---
title: Selector - sok
---

[sok](../../index.html) / [Sok.Selector](../index.html) / [Selector](./index.html)

# Selector

`class Selector` [(source)](https://github.com/SeekDaSky/Sok/tree/master/jvm/sok-jvm/src/Sok/Selector/Selector.kt#L39)

**Platform and version requirements:** JVM, Native

Class wrapping the NIO Selector class for a more "coroutine-friendly" approach. Each `SelectableCHannel` will have a `SuspentionMap` as
attachment, this map contains all teh Continuations/Lambda to resume/call when an event come in.

Sockets register quite frequently and as the NIO Selector class blocks any registration while selecting we have to implement a way to
synchronize registrations and the Selector class. This is done by sharing the `CoroutineScope` of the Selector to the `SuspentionMap`
classes, this way the `SuspentionMap` is able to launch coroutine on the Selector Thread, thus ensuring mutual-exclusion.

To reduce the number of registration, a socket may register for a unknown number of event. If so the selector will call a lambda after
each event and this lambda will return if the Selector should keep the registration or not. This method slow down the selector but
the performance gain is worth it.

### Constructors

| [&lt;init&gt;](-init-.html) | `Selector()`<br>Class wrapping the NIO Selector class for a more "coroutine-friendly" approach. Each `SelectableCHannel` will have a `SuspentionMap` as attachment, this map contains all teh Continuations/Lambda to resume/call when an event come in. |

### Properties

| [coroutineScope](coroutine-scope.html)<br>(JVM) | `val coroutineScope: <ERROR CLASS>`<br>scope given to the `SuspentionMap` classes to run registration coroutine on the right thread |
| [isClosed](is-closed.html) | `var isClosed: `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)<br>is the Selector still running |
| [isInSelection](is-in-selection.html) | `var isInSelection: `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)<br>is the selector in selection |
| [numberOfChannel](number-of-channel.html)<br>(JVM) | `var numberOfChannel: `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)<br>number fo channel registered to this selector, used for load balancing |

### Functions

| [close](close.html) | `fun close(): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)<br>Close the selector, close all SuspentionMap, cancel the main loop and close the thread |
| [register](register.html)<br>(JVM) | `suspend fun register(channel: `[`SelectableChannel`](http://docs.oracle.com/javase/6/docs/api/java/nio/channels/SelectableChannel.html)`, interest: `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)`, attachment: `[`Any`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-any/index.html)`?): `[`SelectionKey`](http://docs.oracle.com/javase/6/docs/api/java/nio/channels/SelectionKey.html)<br>Register a `SelectableChannel` the NIO `Selector` and bind the attachment (`SuspentionMap`) |
| [wakeup](wakeup.html)<br>(JVM) | `fun wakeup(): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)<br>Wake the NIO selector up, thus making registrations non-blocking |

### Companion Object Properties

| [defaultSelector](default-selector.html) | `val defaultSelector: <ERROR CLASS>`<br>selector |
| [defaultSelectorPool](default-selector-pool.html)<br>(JVM) | `val defaultSelectorPool: <ERROR CLASS>`<br>selector pool |
| [isSelectorPoolInit](is-selector-pool-init.html)<br>(JVM) | `var isSelectorPoolInit: `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)<br>is the selector pool initialized. |

### Companion Object Functions

| [closeSelectorAndWait](close-selector-and-wait.html)<br>(Native) | `suspend fun closeSelectorAndWait(): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)<br>Close the selector |
| [setDefaultScope](set-default-scope.html)<br>(Native) | `fun setDefaultScope(scope: <ERROR CLASS>): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)<br>Bind the Selector to a particular CoroutineScope, mainly used in order to prevent the event loop from exiting while te selector is still running |

