---
title: Selector.setDefaultScope - sok
---

[sok](../../index.html) / [Sok.Selector](../index.html) / [Selector](index.html) / [setDefaultScope](./set-default-scope.html)

# setDefaultScope

`fun setDefaultScope(scope: <ERROR CLASS>): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) [(source)](https://github.com/SeekDaSky/Sok/tree/master/native/sok-native-linux/src/Sok/Selector/Selector.kt#L62)

**Platform and version requirements:** Native

Bind the Selector to a particular CoroutineScope, mainly used in order to prevent the
event loop from exiting while te selector is still running

exemple:

``` kotlin
runBlocking(){
     Selector.setDefaultScope(this)
     //the runBlocking statement will now not return until the Selector.closeSelectorAndWait() method is called
}
```

