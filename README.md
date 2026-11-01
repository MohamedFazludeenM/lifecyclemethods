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
<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:gravity="center"
    android:orientation="vertical"
    android:padding="16dp">
    <TextView
        android:layout_width="310dp"
        android:layout_height="86dp"
        android:gravity="center"
        android:text="@string/hello_details"
        android:textColor="#333333"
        android:textSize="18sp" />

</LinearLayout>
```

## OUTPUT
```
<img width="1916" height="1078" alt="Screenshot 2026-11-01 215530" src="https://github.com/user-attachments/assets/2f9afe20-ca71-458b-aa19-b65e4c3b6595" />
<img width="1917" height="1078" alt="Screenshot 2026-11-01 215737" src="https://github.com/user-attachments/assets/8f6c2003-67ae-41c6-a785-e90020549d5d" />
<img width="1917" height="1078" alt="Screenshot 2026-11-01 215755" src="https://github.com/user-attachments/assets/4c3a765a-54df-4021-9518-f9ee0ab015e1" />
<img width="1917" height="1078" alt="Screenshot 2026-11-01 215813" src="https://github.com/user-attachments/assets/927161cf-682d-4f55-8c29-d863cb11b495" />
<img width="1917" height="1078" alt="Screenshot 2026-11-01 220150" src="https://github.com/user-attachments/assets/5e545504-4934-44d1-afa4-84cce6fcba96" />
```




## RESULT
Thus a Simple Android Application create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio is developed and executed successfully.
