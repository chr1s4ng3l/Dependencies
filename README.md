# Dependencies

```kotlin
    /**
     * GSON - A Java library that can be used to convert Java Objects into their JSON representation and vice versa.
     * Docs: https://www.javadoc.io/doc/com.google.code.gson/gson/latest/index.html
     **/
    implementation 'com.google.code.gson:gson:2.10.1'

    /*
     * Retrofit - A type-safe HTTP client for Android and Java.
     * Docs: https://square.github.io/retrofit/2.x/retrofit/
     */
    implementation 'com.squareup.retrofit2:converter-gson:2.9.0'
    implementation 'com.squareup.retrofit2:retrofit:2.9.0'

    /**
     * Okhttp - A modern HTTP client for Android and Java.
     * Docs: https://square.github.io/okhttp/4.x/okhttp/
     */
    implementation 'com.squareup.okhttp3:okhttp:5.0.0-alpha.6'
    implementation "com.squareup.okhttp3:logging-interceptor:5.0.0-alpha.6"

    /**
     * HILT - A dependency injection library for Android that reduces the boilerplate of doing manual dependency injection in your project.
     * Docs: https://dagger.dev/hilt/
     */
    implementation 'com.google.dagger:hilt-android:2.45'
    kapt 'com.google.dagger:hilt-android-compiler:2.45'
    implementation "androidx.hilt:hilt-navigation-compose:1.0.0"
    
    plugins {
   
    id 'kotlin-kapt'
    id 'dagger.hilt.android.plugin'
           }

    id 'com.google.dagger.hilt.android' version '2.44.2' apply false

    /**
     * Coroutines - A library for writing asynchronous, non-blocking code in a more concise and structured way.
     * Docs: https://kotlin.github.io/kotlinx.coroutines/kotlinx-coroutines-core/kotlinx.coroutines/
     */
    implementation 'org.jetbrains.kotlinx:kotlinx-coroutines-android:1.6.4'

    /**
     * Coil - A fast, lightweight, and modern image loading library for Android backed by Kotlin.
     * Docs: https://coil-kt.github.io/coil/api/coil/index.html
     */
    implementation "io.coil-kt:coil-compose:2.2.2"
