Based on https://codelabs.developers.google.com/codelabs/kotlin-android-training-app-anatomy/index.html

Things learned:
Linearlayout
android:layout_width
android:layout_height
android:layout_gravity="center_horizontal"
string resources -> string.xml
android:layout_gravity="center_vertical"
android:textSize
sp -> Scalable Pixels
findViewById(R.id.roll_button);
setOnClickListener
val randomInt = Random.nextInt(6) + 1;

Exception handling:
try {
            if (text.toInt() < 6) {
                resultText.text = (text.toInt() + 1).toString();
            }
        } catch(e: NumberFormatException) {
            resultText.text = "1";
        }