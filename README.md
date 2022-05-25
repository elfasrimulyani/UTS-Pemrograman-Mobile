# UTS-Pemrograman-Mobile

<?xml version="1.0" encoding="utf-8"?>
<RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".DaftarActivity">

    <LinearLayout
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:orientation="vertical"
        android:gravity="center">
        <TextView
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:gravity="center"
            android:text="Daftar"
            android:textSize="25sp"
            android:textStyle="bold"
            android:layout_marginBottom="20dp"/>
            <EditText
                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:hint="Email"
                android:inputType="textEmailAddress"
                android:layout_marginBottom="5dp"/>
            <EditText
                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:hint="No.Hp"
                android:inputType="number"
                android:layout_marginBottom="5dp"/>
            <EditText
                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:hint="Password"
                android:inputType="textPassword"
                android:layout_marginBottom="30dp"/>
            <Button
                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:text="Daftar"
                android:gravity="center"/>
    </LinearLayout>

</RelativeLayout>
