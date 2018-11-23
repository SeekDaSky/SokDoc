---
title: TCPClientSocket.setOption - sok
---

[sok](../../index.html) / [Sok.Socket.TCP](../index.html) / [TCPClientSocket](index.html) / [setOption](./set-option.html)

# setOption

`fun <T> setOption(option: `[`SocketOption`](../../-sok.-socket.-options/-socket-option/index.html)`<`[`T`](set-option.html#T)`>): `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html) [(source)](https://github.com/SeekDaSky/Sok/tree/master/common/sok-common/src/Sok/Socket/TCP/TCPClientSocket.kt#L143)

**Platform and version requirements:** Common

set a socket option
exemple:

``` kotlin
client.setOption(SocketOption(Options.SO_KEEPALIVE,true))
```

### Parameters

`option` - option to set

**Return**
success of the operation

`actual fun <T> setOption(option: <ERROR CLASS><`[`T`](set-option.html#T)`>): `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html) [(source)](https://github.com/SeekDaSky/Sok/tree/master/jvm/sok-jvm/src/Sok/Socket/TCP/TCPClientSocket.kt#L390)

**Platform and version requirements:** JVM, JS, Native

set a socket option

### Parameters

`option` - option to set

**Return**
success of the operation

