# Penugasan MA
# activity_main 
    <?xml version="1.0" encoding="utf-8"?>
    <androidx.constraintlayout.widget.ConstraintLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:tools="http://schemas.android.com/tools"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">

    <TextView
        android:id="@+id/et_judul"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginTop="116dp"
        android:text="Menghitung Luas Segitiga"
        android:textColor="@color/black"
        android:textSize="24sp"
        android:textStyle="bold"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.497"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent" />

    <EditText
        android:id="@+id/et_alas"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:ems="10"
        android:hint="Alas"
        android:inputType="textPersonName"
        tools:layout_editor_absoluteX="34dp"
        tools:layout_editor_absoluteY="240dp" />

    <TextView
        android:id="@+id/tv_hasil"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Hasil"
        android:textColor="@android:color/holo_blue_dark"
        android:textSize="36sp"
        android:textStyle="normal|bold|italic"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent" 
        tools:layout_editor_absoluteY="415dp" />

    <Button
        android:id="@+id/bt_samadengan"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Sama Dengan"
        app:layout_constraintBottom_toTopOf="@+id/tv_hasil"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toBottomOf="@+id/et_alas" />

    <EditText
        android:id="@+id/et_tinggi"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:ems="10"
        android:hint="Tinggi"
        android:inputType="textPersonName"
        app:layout_constraintBottom_toTopOf="@+id/et_alas"
        app:layout_constraintTop_toBottomOf="@+id/textView"
        tools:layout_editor_absoluteX="34dp" />

    </androidx.constraintlayout.widget.ConstraintLayout>

# mainactivity
    package com.example.myapplication

    import androidx.appcompat.app.AppCompatActivity
    import android.os.Bundle
    import android.widget.Button
    import android.widget.EditText
    import android.widget.TextView
    import kotlin.math.E

    class MainActivity : AppCompatActivity() {

    private lateinit var etjudul = EditText
    private lateinit var ettinggi = EditText
    private lateinit var etalas = EditText
    private lateinit var btsamadengan = Button
    private lateinit var tvhasil = TextView
    private lateinit var this = 
    override fun onCreate(savedInstanceState: Bundle?) {
        super.onCreate(savedInstanceState)
        setContentView(R.layout.activity_main)

        etjudul = findViewById(R.id.et_judul)
        ettinggi = findViewById(R.id.et_tinggi)
        etalas = findViewById(R.id.et_alas)
        btsamadengan = findViewById(R.id.bt_samadengan)
        tvhasil = findViewById(R.id.tv_hasil)

        btsamadengan.setOnClicklistener(this)
    }
}





