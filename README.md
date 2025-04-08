# kido
an application which helps to kids to learn mathematics with fun and joy.
package com.example.mathfun

import android.content.Intent
import android.os.Bundle
import androidx.appcompat.app.AppCompatActivity
import com.example.mathfun.databinding.ActivityMainBinding

class MainActivity : AppCompatActivity() {
    private lateinit var binding: ActivityMainBinding

    override fun onCreate(savedInstanceState: Bundle?) {
        super.onCreate(savedInstanceState)
        binding = ActivityMainBinding.inflate(layoutInflater)
        setContentView(binding.root)

        binding.btnLessons.setOnClickListener {
            startActivity(Intent(this, LessonActivity::class.java))
        }

        binding.btnGames.setOnClickListener {
            startActivity(Intent(this, GameActivity::class.java))
        }

        binding.btnQuizzes.setOnClickListener {
            startActivity(Intent(this, QuizActivity::class.java))
        }

        binding.btnProfile.setOnClickListener {
            startActivity(Intent(this, ProfileActivity::class.java))
        }

        binding.btnParentalControls.setOnClickListener {
            startActivity(Intent(this, ParentalControlActivity::class.java))
        }
    }
}
package com.example.mathfun

import android.os.Bundle
import androidx.appcompat.app.AppCompatActivity
import com.example.mathfun.databinding.ActivityLessonBinding

class LessonActivity : AppCompatActivity() {
    private lateinit var binding: ActivityLessonBinding

    override fun onCreate(savedInstanceState: Bundle?) {
        super.onCreate(savedInstanceState)
        binding = ActivityLessonBinding.inflate(layoutInflater)
        setContentView(binding.root)

        // TODO: Implement interactive lessons and tutorials
    }
}
package com.example.mathfun

import android.os.Bundle
import androidx.appcompat.app.AppCompatActivity
import com.example.mathfun.databinding.ActivityGameBinding

class GameActivity : AppCompatActivity() {
    private lateinit var binding: ActivityGameBinding

    override fun onCreate(savedInstanceState: Bundle?) {
        super.onCreate(savedInstanceState)
        binding = ActivityGameBinding.inflate(layoutInflater)
        setContentView(binding.root)

        // TODO: Implement fun math games
    }
}
package com.example.mathfun

import android.os.Bundle
import androidx.appcompat.app.AppCompatActivity
import com.example.mathfun.databinding.ActivityQuizBinding

class QuizActivity : AppCompatActivity() {
    private lateinit var binding: ActivityQuizBinding

    override fun onCreate(savedInstanceState: Bundle?) {
        super.onCreate(savedInstanceState)
        binding = ActivityQuizBinding.inflate(layoutInflater)
        setContentView(binding.root)

        // TODO: Implement quizzes
    }
}
package com.example.mathfun

import android.os.Bundle
import androidx.appcompat.app.AppCompatActivity
import com.example.mathfun.databinding.ActivityProfileBinding

class ProfileActivity : AppCompatActivity() {
    private lateinit var binding: ActivityProfileBinding

    override fun onCreate(savedInstanceState: Bundle?) {
        super.onCreate(savedInstanceState)
        binding = ActivityProfileBinding.inflate(layoutInflater)
        setContentView(binding.root)

        // TODO: Implement progress tracking and rewards system
    }
}
package com.example.mathfun

import android.os.Bundle
import androidx.appcompat.app.AppCompatActivity
import com.example.mathfun.databinding.ActivityParentalControlBinding

class ParentalControlActivity : AppCompatActivity() {
    private lateinit var binding: ActivityParentalControlBinding

    override fun onCreate(savedInstanceState: Bundle?) {
        super.onCreate(savedInstanceState)
        binding = ActivityParentalControlBinding.inflate(layoutInflater)
        setContentView(binding.root)

        // TODO: Implement parental controls and reporting
    }
}
<?xml version="1.0" encoding="utf-8"?>
<layout xmlns:android="http://schemas.android.com/apk/res/android">

    <data>
        <!-- Declare any binding variables here -->
    </data>

    <RelativeLayout
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        android:padding="16dp">

        <Button
            android:id="@+id/btnLessons"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="Lessons" />

        <Button
            android:id="@+id/btnGames"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="Games"
            android:layout_below="@id/btnLessons"
            android:layout_marginTop="16dp" />

        <Button
            android:id="@+id/btnQuizzes"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="Quizzes"
            android:layout_below="@id/btnGames"
            android:layout_marginTop="16dp" />

        <Button
            android:id="@+id/btnProfile"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="Profile"
            android:layout_below="@id/btnQuizzes"
            android:layout_marginTop="16dp" />

        <Button
            android:id="@+id/btnParentalControls"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="Parental Controls"
            android:layout_below="@id/btnProfile"
            android:layout_marginTop="16dp" />

    </RelativeLayout>

</layout>
<?xml version="1.0" encoding="utf-8"?>
<layout xmlns:android="http://schemas.android.com/apk/res/android">

    <data>
        <!-- Declare any binding variables here -->
    </data>

    <RelativeLayout
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        android:padding="16dp">

        <!-- TODO: Add UI elements for interactive lessons -->

    </RelativeLayout>

</layout>
<?xml version="1.0" encoding="utf-8"?>
<layout xmlns:android="http://schemas.android.com/apk/res/android">

    <data>
        <!-- Declare any binding variables here -->
    </data>

    <RelativeLayout
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        android:padding="16dp">

        <!-- TODO: Add UI elements for fun math games -->

    </RelativeLayout>

</layout>
<?xml version="1.0" encoding="utf-8"?>
<layout xmlns:android="http://schemas.android.com/apk/res/android">

    <data>
        <!-- Declare any binding variables here -->
    </data>

    <RelativeLayout
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        android:padding="16dp">

        <!-- TODO: Add UI elements for quizzes -->

    </RelativeLayout>

</layout>
<?xml version="1.0" encoding="utf-8"?>
<layout xmlns:android="http://schemas.android.com/apk/res/android">

    <data>
        <!-- Declare any binding variables here -->
    </data>

    <RelativeLayout
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        android:padding="16dp">

        <!-- TODO: Add UI elements for progress tracking and rewards -->

    </RelativeLayout>

</layout>
<?xml version="1.0" encoding="utf-8"?>
<layout xmlns:android="http://schemas.android.com/apk/res/android">

    <data>
        <!-- Declare any binding variables here -->
    </data>

    <RelativeLayout
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        android:padding="16dp">

        <!-- TODO: Add UI elements for parental controls and reporting -->

    </RelativeLayout>

</layout>
