---
title: alltypes - sok
---

### All Types

| [Sok.Exceptions.BufferDestroyedException](../-sok.-exceptions/-buffer-destroyed-exception/index.html) | Exception thrown when trying to modify the buffer after the destroy() method was called |
| [Sok.Exceptions.BufferOverflowException](../-sok.-exceptions/-buffer-overflow-exception/index.html) | Exception thrown when trying to put a value too large for the remaining space in the buffer |
| [Sok.Buffer.BufferPool](../-sok.-buffer/-buffer-pool/index.html) | In order to avoid garbage collection pressure it is a common practice to pre-allocate objects that are known to be long-living for a later use, Kotlin channels give us a great way to implement a quite straightforward object pool. The pool will allocate all the buffers lazily when needed, this means that the pool will never suspend until reaching the maximum size. |
| [Sok.Exceptions.BufferUnderflowException](../-sok.-exceptions/-buffer-underflow-exception/index.html) | Exception thrown when trying to read a value too large for the remaining space in the buffer |
| [Sok.Exceptions.ConnectionRefusedException](../-sok.-exceptions/-connection-refused-exception/index.html) | Exception thrown when a client tries to connect and fails |
| [Sok.Selector.Interests](../-sok.-selector/-interests/index.html) | Enum representing the possible interests of a `SelectionKey` |
| [Sok.Buffer.JSMultiplatformBuffer](../-sok.-buffer/-j-s-multiplatform-buffer/index.html) | JS implementation of the `MultiplatformBuffer` class |
| [Sok.Buffer.JVMMultiplatformBuffer](../-sok.-buffer/-j-v-m-multiplatform-buffer/index.html) | JVM implementation of the `MultiplatformBuffer` class |
| [Sok.Buffer.MultiplatformBuffer](../-sok.-buffer/-multiplatform-buffer/index.html) | A `MultiplatformBuffer` is the primitive type of Sok, you will use it to receive, send and manipulate data |
| [Sok.Buffer.NativeMultiplatformBuffer](../-sok.-buffer/-native-multiplatform-buffer/index.html) | Native implementation of the `MultiplatformBuffer` class |
| [Sok.Selector.Selector](../-sok.-selector/-selector/index.html) | Class wrapping the NIO Selector class for a more "coroutine-friendly" approach. Each `SelectableCHannel` will have a `SuspentionMap` as attachment, this map contains all teh Continuations/Lambda to resume/call when an event come in. |
| [Sok.Selector.SelectorPool](../-sok.-selector/-selector-pool/index.html) | A SelectorPool will order the Selectors by the number of channels registered. This allow us to do a basic load balancing between all the Selectors |
| [Sok.Socket.TCP.TCPClientSocket](../-sok.-socket.-t-c-p/-t-c-p-client-socket/index.html) | Class representing a client socket. You can use it to perform any I/O operation. Keep in mind that this class keep an internal queue for write operations thus storing data until written so you should have some kind of backpressure mechanism to prevent the accumulation of too many data. |
| [Sok.Socket.TCP.TCPServerSocket](../-sok.-socket.-t-c-p/-t-c-p-server-socket/index.html) | Class representing a listening socket. You can use it to perform accept() operation only. |
