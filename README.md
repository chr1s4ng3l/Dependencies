# Dependencies

```kotlin
    /**
     * GSON - A Java library that can be used to convert Java Objects into their JSON representation and vice versa.
     * Docs: https://www.javadoc.io/doc/com.google.code.gson/gson/latest/index.html
     **/
    implementation 'com.google.code.gson:gson:2.10.1'
    
     // Moshi - is a modern JSON library for Android and Java. The moshi-kotlin artifact contains Kotlin adapters for Moshi, which enable seamless serialization and 
     // deserialization of Kotlin classes.
    implementation("com.squareup.moshi:moshi-kotlin:1.14.0")

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
       * Koin for Android
       **/
    implementation "io.insert-koin:koin-android:$koin_version"

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
    //Coil gift
    implementation("io.coil-kt:coil-gif:2.4.0")
    
    /**
     * Glide
     */
    implementation 'com.github.bumptech.glide:glide:4.12.0'
    kapt 'com.github.bumptech.glide:compiler:4.12.0'
    
    //PICASSO
    implementation "com.squareup.picasso:picasso:2.71828"
    
    // Mockk
    testImplementation "io.mockk:mockk:1.13.4"
    testImplementation 'junit:junit:4.13.2'
    androidTestImplementation 'androidx.test.ext:junit:1.1.5'

    // Unit testing coroutines
    testImplementation 'org.jetbrains.kotlinx:kotlinx-coroutines-test:1.6.4'
    testImplementation 'androidx.arch.core:core-testing:2.1.0'
    
    // ViewModel
    implementation "androidx.lifecycle:lifecycle-viewmodel-ktx:2.5.1"
    implementation "androidx.lifecycle:lifecycle-runtime-ktx:2.5.1"
    // LiveData
    implementation "androidx.lifecycle:lifecycle-livedata-ktx:2.5.1"

    //Room
    implementation "androidx.room:room-ktx:2.5.0"
    kapt "androidx.room:room-compiler:2.5.0"
    
    //Constraint
    implementation "androidx.constraintlayout:constraintlayout-compose:1.0.1"

    //Navigation compose
    implementation "androidx.hilt:hilt-navigation-compose:1.0.0"
    implementation "androidx.compose.runtime:runtime-livedata:$compose_ui_version"

    //CameraX
    def camerax_version = "1.0.2"
    implementation "androidx.camera:camera-core:${camerax_version}"
    implementation "androidx.camera:camera-camera2:${camerax_version}"
    implementation "androidx.camera:camera-lifecycle:${camerax_version}"
    implementation "androidx.camera:camera-view:1.0.0-alpha29"

    //Barcode
    implementation 'com.google.mlkit:barcode-scanning:17.0.0'

    //Permission
    implementation "com.google.accompanist:accompanist-permissions:0.19.0"

    //WorkManager
    implementation "androidx.work:work-runtime-ktx:$work_version"

    //Swipe and refresh
    implementation "me.saket.swipe:swipe:1.1.1"
    
    /**
     * Mockk library for creating mock objects in tests.
     */
    testImplementation "io.mockk:mockk:1.13.4"
    androidTestImplementation "io.mockk:mockk-android:1.13.4"

    /**
     * JUnit 4 for unit testing.
     */
    testImplementation 'junit:junit:4.13.2'

    /**
     * AndroidX JUnit extension for running JUnit tests on Android.
     */
    androidTestImplementation 'androidx.test.ext:junit:1.1.5'

    /**
     * Kotlin coroutines test library for testing coroutines in unit tests.
     */
    testImplementation 'org.jetbrains.kotlinx:kotlinx-coroutines-test:1.6.4'
    
    // Dependency for Exoplayer
    implementation 'com.google.android.exoplayer:exoplayer:2.18.2'

    // for core support in exoplayer.
    implementation 'com.google.android.exoplayer:exoplayer-core:2.18.2'

    // for adding dash support in our exoplayer.
    implementation 'com.google.android.exoplayer:exoplayer-dash:2.18.2'

    // for adding hls support in exoplayer.
    implementation 'com.google.android.exoplayer:exoplayer-hls:2.18.2'

    // for smooth streaming of video in our exoplayer.
    implementation 'com.google.android.exoplayer:exoplayer-smoothstreaming:2.18.2'

    // for generating default ui of exoplayer
    implementation 'com.google.android.exoplayer:exoplayer-ui:2.18.2'
    
    //Agora vide call
    
    allprojects {
  repositories {
    ...
    maven { url 'https://jitpack.io' }
  }
}

dependencies {
  implementation 'com.github.AgoraIO-Community:VideoUIKit-Android:version'
}

//Google maps api
classpath 'com.google.gms:google-services:<latest_version>'

apply plugin: 'com.android.application'
apply plugin: 'com.google.gms.google-services'

implementation 'com.google.android.gms:play-services-maps:<latest_version>'

//Material Components: A set of UI components following the Material Design guidelines, including buttons, cards, etc.
implementation 'com.google.android.material:material:<latest_version>'

//ButterKnife: A view binding library that reduces boilerplate code for binding views and listeners.
implementation 'com.jakewharton:butterknife:<latest_version>'

//LeakCanary: A memory leak detection library that helps identify and fix memory leaks in your app.
implementation 'com.squareup.leakcanary:leakcanary-android:<latest_version>'

//Firebase: A suite of tools and services provided by Google, including authentication, cloud messaging, real-time
//database, and more.
implementation 'com.google.firebase:firebase-analytics:<latest_version>'
implementation 'com.google.firebase:firebase-auth:<latest_version>'

//RxJava: A library for composing asynchronous and event-based programs using observable sequences.
implementation 'io.reactivex.rxjava3:rxjava:<latest_version>'

//Espresso: A testing framework for UI testing in Android, allowing you to write UI tests to validate user interactions.
androidTestImplementation 'androidx.test.espresso:espresso-core:<latest_version>'

//Play Core: A library that provides in-app updates, in-app reviews, and other Play Store features for your app.\
implementation 'com.google.android.play:core:<latest_version>'
