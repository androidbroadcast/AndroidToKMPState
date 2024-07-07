# AndroidToKMPState
State of popular libraries/APIs in Android apps and their KMP support state

| Library/Techology | Has KMP support | KMP Alternatives |
| ----------------- | --------------- | ---------------- |
| [Retrofit](https://github.com/square/retrofit) | ❌ | [Ktorfit](https://github.com/Foso/Ktorfit) |
| [OkHttp](https://github.com/square/okhttp) | ❌ | [Ktor Client](https://ktor.io/docs/welcome.html) |
| [Dagger/Hilt](https://dagger.dev/) | ❌ | [Koin](https://github.com/InsertKoinIO/koin), [Kodein](https://github.com/kosi-libs/Kodein), Manual DI, etc. |
| [Jetpack Room](https://developer.android.com/jetpack/androidx/releases/room) | 2.7 и выше | [SQLDelight](https://github.com/cashapp/sqldelight) |
| [RxJava](https://github.com/ReactiveX/RxJava) | ❌ | [Reaktive](https://github.com/badoo/Reaktive), [KotlinX Coroutines + Flow](https://github.com/Kotlin/kotlinx.coroutines) |
| [APT](https://docs.oracle.com/javase%2F8%2Fdocs%2Fapi%2F%2F/javax/annotation/processing/Processor.html)/[KAPT](https://kotlinlang.org/docs/kapt.html) | ❌ | [KSP](https://github.com/google/ksp) |
| [Java Dynamic Proxy](https://docs.oracle.com/javase/8/docs/technotes/guides/reflection/proxy.html) | ❌ | Code generation with KSP/Gradle |
| [Java Date](https://developer.android.com/reference/java/util/Date) | ❌ | [KotlinX-datetime](https://github.com/Kotlin/kotlinx-datetime) |
| [GSON](https://github.com/google/gson) | ❌ | [KotlinX Serialization](https://github.com/Kotlin/kotlinx.serialization) |
| [Moshi](https://github.com/square/moshi) | ❌ | [KotlinX Serialization](https://github.com/Kotlin/kotlinx.serialization) |
| [Java I/O](https://docs.oracle.com/javase/8/docs/api/java/io/package-summary.html), [Java NIO](https://docs.oracle.com/javase/8/docs/api/java/nio/package-summary.html) | ❌ | [OkIO](https://github.com/square/okio), [Kotlin stdlib](https://kotlinlang.org/api/latest/jvm/stdlib/), [KotlinX I/O](https://github.com/Kotlin/kotlinx-io) |
| [Jetpack Paging](https://developer.android.com/jetpack/androidx/releases/paging) | ✅ |- |
| [Jetpack Collections](https://developer.android.com/jetpack/androidx/releases/collection) | ✅ | [Kotlin stdlib](https://kotlinlang.org/api/latest/jvm/stdlib/) |
| [Jetpack Viewmodel](https://developer.android.com/jetpack/androidx/releases/lifecycle) | ✅ | - |
| [Jetpack Lifecycle](https://developer.android.com/jetpack/androidx/releases/lifecycle) | ✅ | - |
| [Jetpack Livedata](https://developer.android.com/jetpack/androidx/releases/lifecycle) | ❌ | [StateFlow из KotlinX Coroutines](https://github.com/Kotlin/kotlinx.coroutines), [Reaktive](https://github.com/badoo/Reaktive) |
| [Jetpack Compose](https://developer.android.com/develop/ui/compose) | ✅ | [JetBrains Compose Multiplatform](https://github.com/JetBrains/compose-multiplatform) |
| [Android Resources](https://developer.android.com/guide/topics/resources/providing-resources) | ❌ | [Compose Multiplatform Resources](https://www.jetbrains.com/help/kotlin-multiplatform-dev/compose-images-resources.html) |
