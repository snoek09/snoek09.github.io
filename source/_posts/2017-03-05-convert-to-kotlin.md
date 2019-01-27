---
title: Setting up Kotlin in Android Studio
date_lastmod: 2017-03-05
hero: /images/kotlin-logo.png
---

[Last time](/blog/2017/02/22/revisiting-android-development/) I made a simple
[Android app using the Spotify SDK](https://github.com/snoek09/SpotifyAndroidSdkExample).
Now, it's time to convert this to [Kotlin](http://kotlinlang.org) code.
Kotlin is a statically-typed programming language that runs on the Java Virtual Machine.

<!-- more -->
### Install Kotlin plugin

In Android Studio first download the Kotlin plugin.
To use the plugin you can automatically configure or update your build configuration.
In this example it will be configured manually:

- In `build.gradle` add the different version string and classpath for the plugin.
These values will vary depending on the version you're using:

```
buildscript {
    ext.support_version = '25.2.0'
    ext.kotlin_version = '1.1.0'
    repositories {
        jcenter()
    }
    dependencies {
        classpath 'com.android.tools.build:gradle:2.3.0'
        classpath "org.jetbrains.kotlin:kotlin-gradle-plugin:$kotlin_version"
    }
}

allprojects {
    repositories {
        jcenter()
    }
}
```

- Add the new dependency in `app/build.gradle`:

```
...
    compile "com.android.support:appcompat-v7:$support_version"
    compile "org.jetbrains.kotlin:kotlin-stdlib:$kotlin_version"
...
```

### Convert to Kotlin

After syncing the new build configuration you should now be able to convert Java
to Kotlin code. In the `Code` menu select `Convert Java File to Kotlin File`.
Or use this short-cut on Linux: `Ctrl+Alt+Shift+K`.

All changes made for the example app are viewable in this
[pull request](https://github.com/snoek09/SpotifyAndroidSdkExample/pull/1/files).
