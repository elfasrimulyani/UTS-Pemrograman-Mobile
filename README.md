# UTS-Pemrograman-Mobile
<?xml version="1.0" encoding="utf-8"?>
<RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">

    <LinearLayout
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        android:gravity="center"
        android:orientation="vertical">

        <TextView
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="Login"
            android:textSize="20sp"
            android:layout_marginBottom="30dp"/>
        <EditText
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:hint="Username"
            android:inputType="textEmailAddress"
            android:layout_marginBottom="10dp"/>
        <EditText
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:hint="Password"
            android:inputType="textPassword"
            android:layout_marginBottom="10dp"/>
        <Button
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:text="Login"
            android:gravity="center"
            android:layout_marginBottom="20dp"/>

        <TextView
            android:id="@+id/txtDaftar"
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:text="Daftar ?"
            android:gravity="right"
            android:textStyle="bold" />
    </LinearLayout>

</RelativeLayout>

package com.example.myapplication;

import android.content.Intent
import androidx.appcompat.app.AppCompatActivity;
import android.os.Bundle;
import android.view.View
import android.widget.TextView;

class MainActivity : AppCompatActivity() {

    override
    fun onCreate(savedInstanceState: Bundle?) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);

        TextView daftar = (TextView)findViewById(R.id.txtDaftar);
        daftar setOnClickListener(new.View.OnClickListener(){
            override
            public void onClick (View v){
                Intent i = new Intent (PackageContxt; MainActivity.this, DaftarActivity.class);
                startActivity(i);

            }
        });
    }
}


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

package com.example.myapplication

import androidx.appcompat.app.AppCompatActivity
import android.os.Bundle

class DaftarActivity : AppCompatActivity() {

    override fun onCreate(savedInstanceState: Bundle?) {
        super.onCreate(savedInstanceState)
        setContentView(R.layout.activity_daftar)
    }
}



