---
title: Interests - sok
---

[sok](../../index.html) / [Sok.Selector](../index.html) / [Interests](./index.html)

# Interests

`enum class Interests` [(source)](https://github.com/SeekDaSky/Sok/tree/master/native/sok-native-linux/src/Sok/Selector/SelectionKey.kt#L173)

**Platform and version requirements:** Native

Enum representing the possible interests of a `SelectionKey`

### Enum Values

| [OP_READ](-o-p_-r-e-a-d.html) | Equivalent to linux POLLIN event, fired if there is data to read or a socket to accept |
| [OP_WRITE](-o-p_-w-r-i-t-e.html) | Equivalent to linux POLLOUT event, fired when the socket is readable |

### Properties

| [interest](interest.html) | `val interest: `[`Short`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-short/index.html)<br>raw interest value defined in poll.h |

