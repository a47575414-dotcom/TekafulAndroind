package com.takaful.app

import android.app.Activity
import android.os.Bundle
import android.graphics.Color
import android.view.Gravity
import android.widget.LinearLayout
import android.widget.TextView
import android.widget.Button
import android.widget.EditText
import android.widget.Toast

class MainActivity : Activity() {

    override fun onCreate(savedInstanceState: Bundle?) {
        super.onCreate(savedInstanceState)

        val layout = LinearLayout(this)
        layout.orientation = LinearLayout.VERTICAL
        layout.gravity = Gravity.CENTER
        layout.setPadding(32, 32, 32, 32)
        layout.setBackgroundColor(Color.WHITE)

        val title = TextView(this)
        title.text = "🤝 تطبيق التكافل"
        title.textSize = 30f
        title.gravity = Gravity.CENTER
        title.setTextColor(Color.rgb(0, 120, 70))
        layout.addView(title)

        val description = TextView(this)
        description.text = "معًا لمساعدة المحتاجين في موريتانيا"
        description.textSize = 18f
        description.gravity = Gravity.CENTER
        layout.addView(description)

        val name = EditText(this)
        name.hint = "الاسم الكامل"
        layout.addView(name)

        val region = EditText(this)
        region.hint = "الولاية"
        layout.addView(region)

        val request = EditText(this)
        request.hint = "اكتب نوع المساعدة المطلوبة"
        layout.addView(request)

        val button = Button(this)
        button.text = "إرسال طلب المساعدة"
        layout.addView(button)

        button.setOnClickListener {
            Toast.makeText(
                this,
                "شكرًا لك. هذه نسخة أولية للتجربة.",
                Toast.LENGTH_LONG
            ).show()
        }

        setContentView(layout)
    }
}
