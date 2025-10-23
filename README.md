<p align="center"><img width="260" src="https://filedn.com/lssh2fV92SE8dRT5CWJvvSy/lazysodium_large_transparent.png" /></p>
  
# EDIT: OCT 22 2025 - COMPILED NEW .SO FILES ON NDK 29
## How the artifacts were built

The [jniLibs](https://github.com/emersonsoftware/lazysodium-android/tree/master/app/src/main/jniLibs) directory contains `.so` library files built
with [libsodium](https://github.com/copelandsoftware/libsodium)'s Android release scripts located in
[dist-build](https://github.com/copelandsoftware/libsodium/tree/stable/dist-build) using their stable branch as of October 22rd 2025,
SHA `0b1d032e31c68a4230010b82a44592f7345a6d27`.  Android NDK LTS `29.0.14206865` (r29) was used with platform target of API 29.
SHA256 hashes are as follows

- `c256f4994699e8f1804959122217ee0361c79d1a8271ce46f1f3a841ef22ec2c`  `arm64-v8a/libsodium.so`
- `66018fa617b284e2c1410a6ba2037fe4d64a6f5b5cb03f498793c4620331abbc`  `armeabi-v7a/libsodium.so`
- `d3a482cfd19a8dc55023a149063cbec2bb62a4693bd8db012ab2a1b698562d89`  `x86/libsodium.so`
- `a20feaee31bb66e575aca58275190a47da04eb63a2d07e729447855fd94d950f`  `x86_64/libsodium.so`

# Lazysodium Android
  
Lazysodium is a **complete** Android implementation of the [Libsodium](https://github.com/jedisct1/libsodium) library that provides developers with a **smooth and effortless** cryptography experience. 

[![Checks](https://github.com/terl/lazysodium-android/actions/workflows/primary.yml/badge.svg)](https://github.com/terl/lazysodium-android/actions/workflows/primary.yml)
![Maven Central](https://img.shields.io/maven-central/v/com.goterl/lazysodium-android?color=%23fff&label=Maven%20Central)

**Note: Min SDK of 24 required**

## About
We created Lazysodium because we really wanted a solid Libsodium compatible Java/Android library that would just work without fuss. We were exasperated and annoyed with current Libsodium implementations as some of them were just poorly maintained and poorly architected.

You can find more info [here](https://github.com/terl/lazysodium-java/wiki/about).


## Features
**This library is fully compatible with Kotlin powered Android projects.**

You can find an up-to-date feature list [here](https://github.com/terl/lazysodium-java/wiki/features).

## Quick start

This is by no means a comprehensive introduction to Lazysodium. Please view the [official documentation](https://github.com/terl/lazysodium-java/wiki) for a more comprehensive guide.

Whatever build tool you're using the general gist is to add the `mavenCentral()` repository and then add the Lazysodium dependency.
More detailed instructions [here](https://github.com/terl/lazysodium-java/wiki/installation).

The following example is for users of the build tool Gradle:

```groovy
// Top level build file
repositories {
    // Add this to the end of any existing repositories
    mavenCentral()
}

// Project level dependencies section
dependencies {
    implementation "com.goterl:lazysodium-android:VERSION_NUMBER@aar"
    implementation "net.java.dev.jna:jna:5.17.0@aar"
}
```

Substitute `VERSION_NUMBER` for the version in this box:

![Maven Central](https://img.shields.io/maven-central/v/com.goterl/lazysodium-android?color=%23fff&label=Maven%20Central)

## Documentation

See our [official documentation](https://github.com/terl/lazysodium-java/wiki) to get started.

## Apps

You can preview some of the features in our free Lazysodium app available on Google Play:

<a href='https://play.google.com/store/apps/details?id=com.goterl.lazysodium.example&pcampaignid=MKT-Other-global-all-co-prtnr-py-PartBadge-Mar2515-1'><img alt='Get it on Google Play' src='https://play.google.com/intl/en_gb/badges/images/generic/en_badge_web_generic.png' width="140"/></a>


## Lazysodium for Java
We also have a Java implementation available at [Lazysodium for Java](https://github.com/terl/lazysodium-java). It has the same API as this library so you can share code easily!


---

<a href="https://terl.co"><img width="100" style="float: left: display: inline;" src="https://filedn.com/lssh2fV92SE8dRT5CWJvvSy/terl.png" /></a>

Created by [Terl](https://terl.co).
