### BASIC-ANDROID-_EX_01_Implementation of a Hello world Activity using all lifecycles methods using Android Studio.
## AIM:

To create Hello world Activity using all lifecycles methods to display messages using android studio.

## EQUIPMENTS REQUIRED:
Android Studio(Min. required Artic Fox)

## ALGORITHM:

Step 1: Open Android Stdio and then click on File -> New -> New project.


Step 2: Then type the Application name as HelloWorld and click Next.


Step 3: Then select the Minimum SDK as shown below and click Next.


Step 4: Then select the Empty Activity and click Next. Finally click Finish.


Step 5: Design layout in activity_main.xml.

Step 6: Display message give in MainActivity file.


Step 7: Save and run the application.


## PROGRAM

DEVELOPED BY : Monika D
REGISTER NO: 212223240096

## MainActivity.java:
```
package com.example.sec;

import android.os.Bundle;
import android.widget.Toast;

import androidx.activity.EdgeToEdge;
import androidx.appcompat.app.AppCompatActivity;
import androidx.core.graphics.Insets;
import androidx.core.view.ViewCompat;
import androidx.core.view.WindowInsetsCompat;

public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        Toast t=Toast.makeText(this, "oncreat called", Toast.LENGTH_SHORT);
        t.show();

    }
    protected void onStart() {
        super.onResume();
        setContentView(R.layout.activity_main);
        Toast toast = Toast.makeText(getApplicationContext(), "onStart called", Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onResume() {
        super.onResume();
        setContentView(R.layout.activity_main);
        Toast toast = Toast.makeText(getApplicationContext(), "onResume called", Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onRestart() {
        super.onResume();
        setContentView(R.layout.activity_main);
        Toast toast = Toast.makeText(getApplicationContext(), "onRestart called", Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onPause() {
        super.onResume();
        setContentView(R.layout.activity_main);
        Toast toast = Toast.makeText(getApplicationContext(), "onpasue called", Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onStop() {
        super.onResume();
        setContentView(R.layout.activity_main);
        Toast toast = Toast.makeText(getApplicationContext(), "onstop called", Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onDestroy() {
        super.onResume();
        setContentView(R.layout.activity_main);
        Toast toast = Toast.makeText(getApplicationContext(), "ondestroy called", Toast.LENGTH_LONG);
        toast.show();
    }
}
```

## Activity_Main.XML:
```
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:id="@+id/main"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">

    <TextView
        android:id="@+id/textView"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Hello World!"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent" />

    <Button
        android:id="@+id/button"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Button"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.5"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_bias="0.5" />

    <TextView
        android:id="@+id/textView3"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        tools:layout_editor_absoluteX="163dp"
        tools:layout_editor_absoluteY="187dp" />

    <TextView
        android:id="@+id/textView4"
        android:layout_width="250dp"
        android:layout_height="0dp"
        android:layout_marginStart="59dp"
        android:layout_marginTop="102dp"
        android:text="Name:Monika"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent" />

    <TextView
        android:id="@+id/textView5"
        android:layout_width="226dp"
        android:layout_height="24dp"
        android:layout_marginStart="59dp"
        android:layout_marginTop="40dp"
        android:text="Reg No:212223240096"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toBottomOf="@+id/textView4" />

    <TextView
        android:id="@+id/textView6"
        android:layout_width="226dp"
        android:layout_height="22dp"
        android:layout_marginStart="59dp"
        android:layout_marginBottom="503dp"
        android:text="Dept:AIML"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="@+id/textView3" />

    <TextView
        android:id="@+id/textView7"
        android:layout_width="241dp"
        android:layout_height="22dp"
        android:layout_marginStart="59dp"
        android:text="Batch:2023-2027"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toBottomOf="@+id/textView6" />

</androidx.constraintlayout.widget.ConstraintLayout>
```


## OUTPUT:
![WhatsApp Image 2024-08-24 at 09 58 29_2600c46e](https://github.com/user-attachments/assets/1fe9465b-1a4b-48d7-b4e0-de6dd6422d20)
![WhatsApp Image 2024-08-24 at 09 58 33_08432914](https://github.com/user-attachments/assets/a1fe7648-5df0-46cb-8668-4d843ec99f9f)
![WhatsApp Image 2024-08-24 at 09 58 32_f6d74803](https://github.com/user-attachments/assets/c8750742-dae1-45fd-81ce-8fde9acd51a4)

![WhatsApp Image 2024-08-24 at 09 58 33_d6c38082](https://github.com/user-attachments/assets/93fe87e0-9b94-4136-92a8-f379d619db72)
![WhatsApp Image 2024-08-24 at 09 58 31_f32af562](https://github.com/user-attachments/assets/de45f1c4-fee0-4103-81a2-22b42dec2a93)


## RESULT:
Thus a program to implement the various life cycles of an activity is written and successfully executed using Android Studio.
