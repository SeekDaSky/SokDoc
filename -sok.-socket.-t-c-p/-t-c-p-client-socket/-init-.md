---
title: TCPClientSocket.<init> - sok
---

[sok](../../index.html) / [Sok.Socket.TCP](../index.html) / [TCPClientSocket](index.html) / [&lt;init&gt;](./-init-.html)

# &lt;init&gt;

`TCPClientSocket(channel: `[`SocketChannel`](http://docs.oracle.com/javase/6/docs/api/java/nio/channels/SocketChannel.html)`, selectorPool: `[`SelectorPool`](../../-sok.-selector/-selector-pool/index.html)`)`

**Platform and version requirements:** JVM

Helper contrutor that simply get the less busy selector from the pool then use the "standard" constructor

### Parameters

`channel` - NIO channel

`selectorPool` - Selector pool to use`TCPClientSocket(channel: `[`SocketChannel`](http://docs.oracle.com/javase/6/docs/api/java/nio/channels/SocketChannel.html)`, selector: `[`Selector`](../../-sok.-selector/-selector/index.html)`)`

**Platform and version requirements:** JVM

Wrap a NIO channel with a Sok client socket class

### Parameters

`channel` - NIO channel

`selector` - Selector used to track the NIO channel`TCPClientSocket(socket: dynamic)`

**Platform and version requirements:** JS

Wrap a Node.js socket with Sok Client socket class

### Parameters

`socket` - Node.js socket class