---
title: handleException - sok
---

[sok](../index.html) / [Sok.Exceptions](index.html) / [handleException](./handle-exception.html)

# handleException

`fun <ERROR CLASS>.handleException(exception: `[`Throwable`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-throwable/index.html)`): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) [(source)](https://github.com/SeekDaSky/Sok/tree/master/common/sok-common/src/Sok/Exceptions/Exceptions.kt#L109)

**Platform and version requirements:** Common

Extension function used to throw an exception in a particular `CoroutineExceptionHandler` without having to pass
an `EmptyCoroutineContext`

