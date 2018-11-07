---
title: Options - sok
---

[sok](../../index.html) / [Sok.Socket.Options](../index.html) / [Options](./index.html)

# Options

`enum class Options` [(source)](https://github.com/SeekDaSky/Sok/tree/master/common/sok-common/src/Sok/Socket/Options/Options.kt#L6)

**Platform and version requirements:** Common

Enum representing all the available options. Please keep in mind that all options are not supported by al the platforms

### Enum Values

| [SO_RCVBUF](-s-o_-r-c-v-b-u-f.html) | Receive buffer size, this option is hint given to the system and may not apply depending on the configuration of the system. Not available on Node.JS |
| [SO_SNDBUF](-s-o_-s-n-d-b-u-f.html) | Send buffer size, this option is hint given to the system and may not apply depending on the configuration of the system. Not available on Node.JS |
| [SO_KEEPALIVE](-s-o_-k-e-e-p-a-l-i-v-e.html) | socket keepalive |
| [TCP_NODELAY](-t-c-p_-n-o-d-e-l-a-y.html) | Naggle's algorithm |

