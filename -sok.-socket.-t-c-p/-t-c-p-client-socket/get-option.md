---
title: TCPClientSocket.getOption - sok
---

[sok](../../index.html) / [Sok.Socket.TCP](../index.html) / [TCPClientSocket](index.html) / [getOption](./get-option.html)

# getOption

`fun <T> getOption(name: `[`Options`](../../-sok.-socket.-options/-options/index.html)`): `[`SocketOption`](../../-sok.-socket.-options/-socket-option/index.html)`<`[`T`](get-option.html#T)`>` [(source)](https://github.com/SeekDaSky/Sok/tree/master/common/sok-common/src/Sok/Socket/TCP/TCPClientSocket.kt#L130)

**Platform and version requirements:** Common

get a socket option and try to convert it to the given type, throw an exception if the option is not of the correct type
exemple:

``` kotlin
client.getOption<Int>(Options.SO_RCVBUF)
```

### Parameters

`name` - Option to get

**Return**
the socket option

`actual fun <T> getOption(name: <ERROR CLASS>): <ERROR CLASS><`[`T`](get-option.html#T)`>` [(source)](https://github.com/SeekDaSky/Sok/tree/master/jvm/sok-jvm/src/Sok/Socket/TCP/TCPClientSocket.kt#L374)

**Platform and version requirements:** JVM, JS, Native

get a socket option and try to convert it to the given type

### Parameters

`name` - Option to get

**Return**
the socket option

