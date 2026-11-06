# Ex.No:1 To create a HelloWorld Activity using all lifecycles methods to display messages.


## AIM:

To create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio.

## EQUIPMENTS REQUIRED:

Latest Version Android Studio

## ALGORITHM:

Step 1: Open Android Stdio and then click on File -> New -> New project.

Step 2: Then type the Application name as HelloWorld and click Next. 

Step 3: Then select the Minimum SDK as shown below and click Next.

Step 4: Then select the Empty Activity and click Next. Finally click Finish.

Step 5: Design layout in activity_main.xml.

Step 6: Display message give in MainActivity file.

Step 7: Save and run the application.

## PROGRAM:
## MainActivity.java
```
package com.example.helloworld;

import android.os.Bundle;
import android.widget.Toast;
import androidx.appcompat.app.AppCompatActivity;

public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        Toast.makeText(this, "onCreate Called", Toast.LENGTH_SHORT).show();
    }

    @Override
    protected void onStart() {
        super.onStart();
        Toast.makeText(this, "onStart Called", Toast.LENGTH_SHORT).show();
    }

    @Override
    protected void onResume() {
        super.onResume();
        Toast.makeText(this, "onResume Called", Toast.LENGTH_SHORT).show();
    }

    @Override
    protected void onPause() {
        super.onPause();
        Toast.makeText(this, "onPause Called", Toast.LENGTH_SHORT).show();
    }

    @Override
    protected void onStop() {
        super.onStop();
        Toast.makeText(this, "onStop Called", Toast.LENGTH_SHORT).show();
    }

    @Override
    protected void onDestroy() {
        Toast.makeText(this, "onDestroy Called", Toast.LENGTH_SHORT).show();
        super.onDestroy();
    }
}

```
## Activity_main.xml
```
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    android:layout_width="match_parent"
    android:layout_height="match_parent">

    <TextView
        android:id="@+id/helloText"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="@string/hello_world"
        android:textSize="24sp"
        android:textColor="#000000"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintEnd_toEndOf="parent" />

</androidx.constraintlayout.widget.ConstraintLayout>

```

## OUTPUT
<img width="1917" height="1078" alt="Screenshot 2026-11-05 211119" src="https://github.com/user-attachments/assets/72c6b85d-119a-4a42-a5b6-19e918b1d0a0" />
<img width="1917" height="1078" alt="Screenshot 2026-11-05 211139" src="https://github.com/user-attachments/assets/bdc15c3b-555a-4f11-a797-5a2f7ca324ce" />
<img width="1917" height="1078" alt="Screenshot 2026-11-05 211158" src="https://github.com/user-attachments/assets/ab31846b-6e61-44db-a5da-ea99a3360c40" />
<img width="1917" height="1078" alt="Screenshot 2026-11-05 211207" src="https://github.com/user-attachments/assets/3fb582fd-c49c-4200-8f99-f7e7a6cb1fee" />
<img width="1917" height="1078" alt="Screenshot 2026-11-05 211554" src="https://github.com/user-attachments/assets/3fbafd91-1834-4acd-b452-1c41a24a56c9" />


## RESULT
Thus a Simple Android Application create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio is developed and executed successfully.
