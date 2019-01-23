---
title: Selector.<init> - sok
---

[sok](../../index.html) / [Sok.Selector](../index.html) / [Selector](index.html) / [&lt;init&gt;](./-init-.html)

# &lt;init&gt;

`Selector()`

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

