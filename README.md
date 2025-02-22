# AndroidToKMPState
State of popular libraries/APIs in Android apps and their KMP support state

_KMP support - support Kotlin Multiplatform with more than one target_

## Android libraries

| Library/Techology | Has KMP support | Supported Targets | KMP Alternatives | Useful Links |
| ----------------- | --------------- | ----------------- | ---------------- | ------------ |
| [Jetpack Room](https://developer.android.com/jetpack/androidx/releases/room) | in 2.7 (base features only) | Android, iOS, JVM | [SQLDelight](https://github.com/cashapp/sqldelight) | [Guide "Migrate Room to KMP"](https://developer.android.com/training/data-storage/room/room-kmp-migration) |
| [Moshi](https://github.com/square/moshi) | ❌ | | [KotlinX Serialization](https://github.com/Kotlin/kotlinx.serialization) | |
| [Jetpack Paging](https://developer.android.com/jetpack/androidx/releases/paging) | ✅ | | - | |
| [Jetpack Collections](https://developer.android.com/jetpack/androidx/releases/collection) | ✅ | | [Kotlin stdlib](https://kotlinlang.org/api/latest/jvm/stdlib/) | |
| [Jetpack Viewmodel](https://developer.android.com/jetpack/androidx/releases/lifecycle) | ✅ | | - | [Using Common ViewModel](https://www.jetbrains.com/help/kotlin-multiplatform-dev/compose-viewmodel.html#using-viewmodel-in-common-code) |
| [Jetpack Lifecycle](https://developer.android.com/jetpack/androidx/releases/lifecycle) | ✅ | | - | [Using Common Lifecycle](https://www.jetbrains.com/help/kotlin-multiplatform-dev/compose-lifecycle.html) |
| [Jetpack Livedata](https://developer.android.com/jetpack/androidx/releases/lifecycle) | ❌ | | [StateFlow from KotlinX Coroutines](https://github.com/Kotlin/kotlinx.coroutines), [Reaktive](https://github.com/badoo/Reaktive) | |
| [Jetpack Compose](https://developer.android.com/develop/ui/compose) | [JetBrains Compose Multiplatform](https://github.com/JetBrains/compose-multiplatform) | Android, Desktop JVM, iOS (Beta), WASM (Alpha) | - | |
| [Android Resources](https://developer.android.com/guide/topics/resources/providing-resources) | ❌ | | [Compose Multiplatform Resources](https://www.jetbrains.com/help/kotlin-multiplatform-dev/compose-images-resources.html) | |
| [Jetpack Compose Navigation](https://developer.android.com/develop/ui/compose/navigation) | [Jetbrains Compose Navigation](https://www.jetbrains.com/help/kotlin-multiplatform-dev/compose-navigation-routing.html#setup) | Android, iOS, JVM | [Voyager](https://voyager.adriel.cafe/), [Decompose](https://arkivanov.github.io/Decompose/), [Appyx](https://bumble-tech.github.io/appyx/), [PreCompose](https://tlaster.github.io/PreCompose/) | [Using Common Navigation](https://www.jetbrains.com/help/kotlin-multiplatform-dev/compose-navigation-routing.html) |
| [Glide](https://github.com/bumptech/glide) | ❌ | - | [CoIL](https://github.com/coil-kt/coil), [Kamel](https://github.com/Kamel-Media/Kamel), [Compose ImageLoader](https://github.com/qdsfdhvh/compose-imageloader) | - |
| [CoIL](https://github.com/coil-kt/coil) | 3.0 | Android, JVM, iOS, macOS, JS, WASM | - | [Coil KMP Migration](https://coil-kt.github.io/coil/upgrading_to_coil3/#multiplatform) |
| [Shared Preferences](https://developer.android.com/training/data-storage/shared-preferences) | ❌ | - | [Jetpack DataStore](https://developer.android.com/jetpack/androidx/releases/datastore) | - |
| [Jetpack DataStore](https://developer.android.com/jetpack/androidx/releases/datastore) | 1.1.0 | Android, iOS, JVM, Linux, macOS, JVM| - | - |
| [Build Config](https://developer.android.com/build/gradle-tips#share-custom-fields-and-resource-values-with-your-app-code) (AGP feature) | - | - | [BuildKonfig](https://github.com/yshrsmz/BuildKonfig) | - |

## JAVA libraries

All libraries that has been writtent in Java or Kotlin for JVM and can be used only on JVM or Android. They have no planned KMP support or possibility to do it in future.
Projects that use libraries/APIs from the table below must be replaced to use in KMP projects.

| Library/Techology | KMP Alternatives | Useful Links |
| ----------------- | ---------------- | ------------ |
| [Retrofit](https://github.com/square/retrofit) | [Ktorfit](https://github.com/Foso/Ktorfit) | |
| [OkHttp](https://github.com/square/okhttp) | [Ktor Client](https://ktor.io/docs/welcome.html) | |
| [RxJava](https://github.com/ReactiveX/RxJava) | [Reaktive](https://github.com/badoo/Reaktive), [KotlinX Coroutines + Flow](https://github.com/Kotlin/kotlinx.coroutines) | |
| [APT](https://docs.oracle.com/javase%2F8%2Fdocs%2Fapi%2F%2F/javax/annotation/processing/Processor.html)/[KAPT](https://kotlinlang.org/docs/kapt.html) | [KSP](https://github.com/google/ksp) | |
| [Java Dynamic Proxy](https://docs.oracle.com/javase/8/docs/technotes/guides/reflection/proxy.html) | Code generation with KSP/Gradle | |
| [Java Date](https://developer.android.com/reference/java/util/Date) | [KotlinX-datetime](https://github.com/Kotlin/kotlinx-datetime) | |
| [GSON](https://github.com/google/gson) | [KotlinX Serialization](https://github.com/Kotlin/kotlinx.serialization) | |
| [Java I/O](https://docs.oracle.com/javase/8/docs/api/java/io/package-summary.html), [Java NIO](https://docs.oracle.com/javase/8/docs/api/java/nio/package-summary.html) | [OkIO](https://github.com/square/okio)
| [Dagger/Hilt](https://dagger.dev/) | [Koin](https://github.com/InsertKoinIO/koin), [Kodein](https://github.com/kosi-libs/Kodein), Manual DI, etc. | |
| [Timber](https://github.com/JakeWharton/timber) | [Khronicle](https://github.com/JuulLabs/khronicle) | |
