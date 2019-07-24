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