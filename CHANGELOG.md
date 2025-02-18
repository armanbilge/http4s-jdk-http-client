# changelog

This file summarizes **notable** changes for each release, but does not describe internal changes unless they are particularly exciting. This change log is ordered chronologically, so each release contains all changes described below it.

----

## v1.0.0-M9 (2023-02-08)

### "Breaking" changes

* Due to internal changes, the dependency on reactive-streams has been dropped.

### Dependency updates

* scala-3.2.2
* fs2-3.6.0
* http4s-1.0.0-M39

## v1.0.0-M8 (2023-01-05)

### Dependency updates

* **http4s-1.0.0-M38**

## v1.0.0-M7 (2022-11-20)

### Breaking changes

* On creation, the `Client` and `WSClient` are no longer wrapped in a `Resource` due to an internal refactoring.

### Dependency updates

* cats-effect-3.4.1
* fs2-3.4.0

## v1.0.0-M6 (2022-09-20)

### Dependency updates

* **http4s-1.0.0-M37**

## v1.0.0-M5 (2022-08-27)

### Dependency updates

* **http4s-1.0.0-M36**

## v1.0.0-M4 (2022-07-29)

### Dependency updates

* **http4s-1.0.0-M35**

## v1.0.0-M3 (2022-07-07)

### Dependency updates

* cats-2.8.0
* **http4s-1.0.0-M34**

## v1.0.0-M2 (2022-05-31)

### Improvements

* Optimizations via new entity model. [#644](https://github.com/http4s/http4s-jdk-http-client/pull/644)
* Use Cats Effect EC as `HttpClient` executor. [#641](https://github.com/http4s/http4s-jdk-http-client/pull/641)

### Dependency updates

* cats-effect-3.3.12
* fs2-3.2.7
* **http4s-1.0.0-M33**

## v1.0.0-M1 (2022-03-23)

This is the spiritual successor to v0.6.0-M7.

### Breaking changes

* We now use the upstream WebSocket model made public in http4s-1.0.0-M32.

### Dependency updates

* scala-2.13.8, scala-3.1.1
* cats-effect-3.3.8
* fs2-3.2.5
* http4s-1.0.0-M32

## v0.6.0-M7 (2021-12-09)

### Dependency updates

* **http4s-1.0.0-M30**
* **scala-3.1.0**
* scala-2.13.7
* cats-2.7.0
* cats-effect-3.3.0
* fs2-3.2.3
* scodec-bits-1.1.30
* case-insensitive-1.2.0

## v0.6.0-M6 (2021-10-13)

### Dependency updates

* **http4s-1.0.0-M29**
* fs2-3.1.5

## v0.6.0-M5 (2021-10-07)

### Dependency updates

* **http4s-1.0.0-M28**
* fs2-3.1.4
* scodec-1.1.29

## v0.6.0-M4 (2021-09-21)

### Dependency updates

* **http4s-1.0.0-M27**
* scala-2.12.15
* cats-effect-3.2.9
* vault-3.1.0

## v0.6.0-M3 (2021-09-15)

### Dependency updates

* **http4s-1.0.0-M25**
* scala-3.0.2
* cats-effect-3.2.8
* fs2-3.1.2
* scodec-bits-1.1.28

## v0.6.0-M2 (2021-08-08)

### Dependency updates

* **http4s-1.0.0-M24**
* scala-2.12.14
* scala-3.0.1
* cats-effect-3.2.2
* fs2-3.1.0
* vault-3.0.4

## v0.6.0-M1 (2021-05-28)

This is the moral successor to v0.5.0-M4, tracking the 1.x releases of http4s.

### Breaking changes

* Rename package from `org.http4s.client.jdkhttpclient` to `org.http4s.jdkhttpclient`. [#442](https://github.com/http4s/http4s-jdk-http-client/pull/442)

### Dependency updates

* **scala-3.0.0**
* **http4s-1.0.0-M23**
* scala-2.13.6
* cats-2.6.1
* cats-effect-3.1.1
* fs2-3.0.4
* scodec-bits-1.1.27
* vault-3.0.3
* case-insensitive-1.1.4

## v0.5.0-M4 (2021-04-11)

### Dependency updates

* scala-3.0.0-RC2
* cats-2.5.0
* cats-effect-3.0.2
* fs2-3.0.1
* scodec-bits-1.1.25
* http4s-1.0.0-M21
* vault-3.0.1
* case-insensitive-1.1.2

## v0.5.0-M3 (2021-03-22)

### Bugfixes

* [#395](https://github.com/http4s/http4s-jdk-http-client/issues/395) Handle `Content-Length: 0` correctly.

### Dependency updates

* scala-2.13.5
* case-insensitive-1.1.0
* cats-effect-3.0.0-RC3

## v0.5.0-M2 (2021-03-05)

### Dependency updates

* http4s-1.0.0-M19

## v0.5.0-M1 (2021-03-03)

### Dependency updates

* scala-3.0.0-RC1
* scodec-bits-1.1.24
* case-insensitive-1.0.0
* cats-effect-3.0.0-RC2
* fs2-3.0.0-M9
* vault-3.0.0-RC2
* http4s-1.0.0-M18

## v0.3.4 (2021-01-19)

This release is considered stable.

### Bugfixes

* [#335](https://github.com/http4s/http4s-jdk-http-client/pull/335) Fix a resource leak if the response body is not touched at all.

### Dependency updates

* http4s-0.21.15

## v0.3.3 (2021-01-01)

This release is considered stable.

### Bugfixes

* [#331](https://github.com/http4s/http4s-jdk-http-client/pull/331) Fix resource leaks in certain cases of request cancellation.

### Dependency updates

* scodec-bits-1.1.23
* fs2-2.5.0
* http4s-0.21.14

## v0.3.2 (2020-12-10)

This release is considered stable.

In particular, the dependency on fs2 is updated to 2.4.6 w.r.t. [#321](https://github.com/http4s/http4s-jdk-http-client/issues/321).

### Dependency updates

* cats-2.3.0
* cats-effect-2.3.0
* scodec-bits-1.1.22
* fs2-2.4.6
* http4s-0.21.13

## v0.3.1 (2020-08-10)

This release is considered stable.

### Bugfixes

* [#260](https://github.com/http4s/http4s-jdk-http-client/pull/260) Workaround for a spurious deadlock with Java 11 and TLS 1.3

### Dependency updates

* cats-effect-2.1.4
* fs2-2.4.2
* http4s-0.21.7
* scodec-bits-1.1.18
* scala-2.12.12 and scala-2.13.3

## v0.3.0 (2020-04-05)

This release is considered stable.

### Bugfixes

* [#191](https://github.com/http4s/http4s-jdk-http-client/pull/191) Now shifting back from the HTTP thread pool. This adds `ContextShift` bounds to client creation.
* [#207](https://github.com/http4s/http4s-jdk-http-client/pull/207) Fix connection leak if body is not consumed

### Dependency updates

* cats-core-2.1.1
* fs2-2.3.0
* http4s-0.21.3
* scodec-bits-1.1.14
* scala-2.12.11

### Documentation

* [#187](https://github.com/http4s/http4s-jdk-http-client/pull/187) mention restricted headers
* [#206](https://github.com/http4s/http4s-jdk-http-client/pull/206) document spurious deadlocks with Java 11 and TLS 1.3

## v0.2.0 (2020-02-09)

This release is considered stable.

### Dependency updates

* http4s-0.21.0

## v0.2.0-RC5 (2020-02-03)

This release is fully source compatible with v0.2.0-RC4, but has a binary-incompatible dependency on http4s.

### Dependency updates

* http4s-0.21.0-RC3

## v0.2.0-RC4 (2020-02-01)

This release is fully source compatible with v0.2.0-RC2, but has a binary-incompatible dependency on http4s.

### Dependency updates

* http4s-0.21.0-RC2
* scodec-bits-1.1.13

~~## v0.2.0-RC3 (2020-02-01)~~

Cursed release. Sonatype says it's there, Maven Central says it's not.

## v0.2.0-RC2 (2020-01-22)

### Dependency updates

* http4s-0.21.0-RC1

## v0.2.0-RC1 (2020-01-22)

### Enhancements

* [#139](https://github.com/http4s/http4s-jdk-http-client/pull/139): Re-raise error in finalizer of web socket listener

### Dependency updates

* cats-2.1.0
* fs2-2.2.1

## v0.2.0-M4 (2019-12-01)

### Dependency updates

* fs2-2.1.0
* http4s-0.21.0-M6

## v0.2.0-M3 (2019-10-02)

### Breaking changes

* [#65](https://github.com/http4s/http4s-jdk-http-client/pull/65): Add `receive[F[Option[WSDataFrame]]]` to the high-level interface. `receiveStream` is now final.

### Dependency updates

* cats-2.0.0-RC2
* fs2-2.0.1
* http4s-0.21.0-M5
* scala-2.12.9 (2.12 cross build)

## v0.2.0-M2 (2019-08-14)

### Enhancements

* [#53](https://github.com/http4s/http4s-jdk-http-client/pull/53): Adds an experimental WebSocket client. In the long term, the plan is to move the `WSClient` interface into http4s-core and unify the client and server frame ADT, but we encourage users to give this a try.

### Documentation

* [#44](https://github.com/http4s/http4s-jdk-http-client/pull/44): Fix supported Scala versions in docs
* [#45](https://github.com/http4s/http4s-jdk-http-client/pull/45): Generate `/stable` redirect in docs

### Dependency updates

* better-monadic-for-0.3.1
* cats-2.0.0-RC1
* cats-effect-2.0.0-RC1
* http4s-0.21.0-M4

## v0.2.0-M1 (2019-06-20)

### Cross-build changes

* Adds Scala 2.13 support. 
* Drops Scala 2.13.0-M5 support.

### Dependency updates

* cats-2.0.0-M4
* cats-effect-2.0.0-M4
* fs2-1.1.0-M1
* http4s-client-0.21.0-M1

## v0.1.0 (2019-06-20)

* Initial release
