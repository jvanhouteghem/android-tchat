# android-tchat

Step 1 : Create our first activity
---

A. Create empty activity named SignInActivity (layout name : activity_sign_in.xml)

B. Fill the activity_sign.xml : 
```
<?xml version="1.0" encoding="utf-8"?>
<RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:paddingBottom="@dimen/activity_vertical_margin"
    android:paddingLeft="@dimen/activity_horizontal_margin"
    android:paddingRight="@dimen/activity_horizontal_margin"
    android:paddingTop="@dimen/activity_vertical_margin"
    tools:context="com.jonathan.vanhouteghem.android_tchat.SignInActivity">

    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Login"
        android:id="@+id/signInLoginTextView"
        android:layout_alignParentLeft="true"
        android:layout_alignParentStart="true"
        android:layout_marginTop="31dp" />

    <EditText
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:id="@+id/signInLoginTextEditor"
        android:layout_below="@+id/signInLoginTextView"
        android:layout_alignParentLeft="true"
        android:layout_alignParentStart="true"
        android:text="jo" />

    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Pass"
        android:id="@+id/signInPassTextView"
        android:layout_below="@+id/signInLoginTextEditor"
        android:layout_alignParentLeft="true"
        android:layout_alignParentStart="true" />

    <EditText
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:id="@+id/signInPassTextEditor"
        android:layout_below="@+id/signInPassTextView"
        android:layout_alignParentLeft="true"
        android:layout_alignParentStart="true"
        android:text="pass" />

    <Button
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Sign In"
        android:id="@+id/signInButtonConnexion"
        android:layout_below="@+id/signInPassTextEditor"
        android:layout_alignParentLeft="true"
        android:layout_alignParentStart="true"
        android:layout_alignParentRight="true"
        android:layout_alignParentEnd="true" />

    <Button
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Sign Up"
        android:id="@+id/signInButtonSignUp"
        android:layout_centerVertical="true"
        android:layout_alignParentLeft="true"
        android:layout_alignParentStart="true"
        android:layout_alignRight="@+id/signInButtonConnexion"
        android:layout_alignEnd="@+id/signInButtonConnexion" />

</RelativeLayout>

```

NB : if you have this problem "The following classes could not be found: android.support.v7.internal.app.WindowDecorActionBar"
then try "compile to use this 'com.android.support:appcompat-v7:23.0.1'" in your build.gradle.