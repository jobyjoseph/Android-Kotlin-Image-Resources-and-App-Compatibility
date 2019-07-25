To get the reference of an imageView
```kotlin
val diceImage: ImageView = findViewById(R.id.dice_image);
```

Using `when` to assign dice image based on random generated number
```kotlin
val drawableResource = when(randomInt) {
            1 -> R.drawable.dice_1
            2 -> R.drawable.dice_2
            3 -> R.drawable.dice_3
            4 -> R.drawable.dice_4
            5 -> R.drawable.dice_5
            else -> R.drawable.dice_6
        }
```

To set the source of an imageView dynamically
```kotlin
diceImage.setImageResource(drawableResource);
```

The `lateinit` keyword promises the Kotlin compiler that the variable will be initialized before the code calls any operations on it.
```kotlin
lateinit var diceImage : ImageView
```

The `tools` namespace is used when you want to define placeholder content that is only used in the preview or the design editor in Android Studio. Attributes using the `tools` namespace are removed when you compile the app.

Android Oreo shipped with support for Picture-in-picture apps, while Android Pie introduced Slices.

The namespace for the Android Jetpack libraries is __androidx__.

An important thing to note about _vector drawables_ is that they are supported in API 21 onwards. But your app's minimum SDK is set to API 19.

Every time that a build.gradle file is modified, you need to sync the build files with the project.

The app:srcCompat attribute uses the Android X library to support vector drawables in older versions of Android, back to API level 7.