# ZXing C++ Android Integration

This guide explains how to integrate the ZXing C++ library for barcode scanning into your Android project.

---

## Adding the Library to Your Project

To use this library, you need to include it in your project dependencies and specify the required Maven repository.

### Step 1: Add Required Maven Repositories

Ensure the following repositories are added to your project’s `build.gradle` and `settings.gradle` file:

- settings.gradle

```gradle
allprojects {
    repositories {
        maven { 
            url 'https://raw.githubusercontent.com/althafvly/zxingcpp-android/v2.2.1/.m2'
        }
        google()
        mavenCentral()
    }
}
```

OR

```gradle
allprojects {
    repositories {
        maven { url 'https://raw.githubusercontent.com/althafvly/zxingcpp-android/v2.2.1/.m2' }
        google()
        mavenCentral()
    }
}
```

### Step 2: Add the Dependency

- build.gradle

```gradle
dependencies {
    implementation 'io.github.zxing-cpp:android:2.2.1'
}
```

OR 

```gradle
dependencies {
    implementation("io.github.zxing-cpp:android:2.2.1")
}
```
