
# Ex.No:10 To create a option menu to display menu items.


## AIM:

To create a option menu to display menu items using Android Studio.

## EQUIPMENTS REQUIRED:

Latest Version Android Studio

## ALGORITHM:
Step 1: Open Android Stdio and then click on File -> New -> New project.

Step 2: Then type the Application name as “menuinandroid″ and click Next.

Step 3: Then select the Minimum SDK as shown below and click Next.

Step 4: Then select the Empty Activity and click Next. Finally click Finish.

Step 5: Design layout in activity_main.xml.

Step 6: Click option menu and Display menu details give in MainActivity file.

Step 7: Save and run the application.


## PROGRAM:
```
/*
Program to print the text “optionmenu”.
Developed by: YUVARAJ B
Registeration Number : 212221040187
*/
```
## ACTIVITY_MAIN.XML
```
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">

    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Hello World!"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent" />

</androidx.constraintlayout.widget.ConstraintLayout>
```
## OPTION.XML
```
<?xml version="1.0" encoding="utf-8"?>
<menu xmlns:android="http://schemas.android.com/apk/res/android">
    <item android:title="Item 1" />
    <item android:title="Item 2" />
    <item android:title="Item 3" />
</menu>
```
## MAINACTIVITY.JAVA
```
package com.example.menuoption;

import androidx.appcompat.app.AppCompatActivity;

import android.os.Bundle;
import android.view.Menu;
import android.view.MenuInflater;

public class MainActivity extends AppCompatActivity {
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
    }
    @Override
    public boolean onCreateOptionsMenu(Menu menu) {
        MenuInflater m = getMenuInflater();
        m.inflate(R.menu.option,menu);
        return true;
    }
}
```

## OUTPUT

![239758865-e5634791-56b4-4011-b3e9-9bb772e79872](https://github.com/yuvaraj-csk/menuinandroid/assets/134052574/8c0860c3-a445-4425-8e88-f55abc16b210)

![239759041-6b5239b8-2b62-4d17-9949-4658bfa88d68](https://github.com/yuvaraj-csk/menuinandroid/assets/134052574/14f09fc4-2739-4bb6-b91a-c8b52ee160fb)
![239758928-a7b34f8e-93f9-4685-9960-383ad17c271e](https://github.com/yuvaraj-csk/menuinandroid/assets/134052574/1bd69a8d-f847-4d90-866d-9f20782fbfcc)


## RESULT
Thus a Simple Android Application to create a option menu to display menu items using Android Studio is developed and executed successfully.
