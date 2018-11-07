---
title: makeNonBlocking - sok
---

[sok](../index.html) / [Sok.Utils](index.html) / [makeNonBlocking](./make-non-blocking.html)

# makeNonBlocking

`fun makeNonBlocking(fd: `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)`): `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html) [(source)](https://github.com/SeekDaSky/Sok/tree/master/native/sok-native-linux/src/Sok/Utils/MakeNonBlocking.kt#L11)

**Platform and version requirements:** Native

Make a linux file descriptor non-blocking (mandatory for poll calls)

### Parameters

`fd` - file descriptor of the socket

**Return**
did the opertion succeed

