package com.example.android.userprofile;

import android.graphics.Color;
import android.support.v7.app.AppCompatActivity;
import android.os.Bundle;
import android.view.View;
import android.widget.ImageView;
import android.widget.TextView;

public class MainActivity extends AppCompatActivity {

    TextView nameView;
    TextView birthdayText;
    TextView countryText;

    @Override
    protected void onCreate(Bundle savedInstanceState) {

        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        nameView = (TextView) findViewById(R.id.name_text_view);
        nameView.setText("Cristina");
        birthdayText = (TextView) findViewById(R.id.birthday_text_view);
        countryText = (TextView) findViewById(R.id.country_text_view);
    }

    public void tulips(View view) {
        ImageView tulipsImageView = (ImageView) findViewById(R.id.android_profile_picture);
        tulipsImageView.setImageResource(R.drawable.emmanualm);
    }




<?xml version="1.0" encoding="utf-8"?>
<RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">

    <ImageView
        android:id="@+id/android_profile_picture"
        android:layout_width="wrap_content"
        android:layout_height="match_parent"
        android:src="@drawable/emmanualm"/>

    <TextView
        android:id="@+id/name_text_view"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="@string/name"
        android:gravity="center_horizontal"
        android:padding="4dp"/>

    <TextView
        android:id="@+id/birthday_text_view"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:text="@string/birthday"
        android:gravity="center_horizontal"
        android:padding="4dp"/>

    <TextView
        android:id="@+id/country_text_view"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:text="@string/country"
        android:gravity="center_horizontal"
        android:padding="4dp"/>


</RelativeLayout>



