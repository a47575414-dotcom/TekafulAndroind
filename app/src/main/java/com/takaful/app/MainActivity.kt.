package com.takaful.app

import android.app.Activity
import android.os.Bundle
import android.view.Gravity
import android.widget.Button
import android.widget.EditText
import android.widget.LinearLayout
import android.widget.TextView
import android.widget.Toast

class MainActivity : Activity() {
    override fun onCreate(savedInstanceState: Bundle?) {
        super.onCreate(savedInstanceState)

        val layout = LinearLayout(this)
        layout.orientation = LinearLayout.VERTICAL
        layout.gravity = Gravity.CENTER
        layout.setPadding(24, 24, 24, 24)

        val title = TextView(this)
        title.text = "تطبيق التكافل"
        title.textSize = 28f
        title.gravity = Gravity.CENTER
        layout.addView(title)

        val description = TextView(this)
        description.text = "منصة خيرية لمساعدة المحتاجين في موريتانيا"
        description.textSize = 18f
        description.gravity = Gravity.CENTER
        layout.addView(description)

        val name = EditText(this)
        name.hint = "الاسم الكامل"
        layout.addView(name)

        val wilaya = EditText(this)
        wilaya.hint = "الولاية"
        layout.addView(wilaya)

        val need = EditText(this)
        need.hint = "نوع المساعدة المطلوبة"
        layout.addView(need)

        val button = Button(this)
        button.text = "إرسال طلب المساعدة"
        layout.addView(button)

        button.setOnClickListener {
            if (name.text.isBlank() ||
                wilaya.text.isBlank() ||
                need.text.isBlank()
            ) {
                Toast.makeText(
                    this,
                    "يرجى ملء جميع الخانات",
                    Toast.LENGTH_SHORT
                ).show()
            } else {
                Toast.makeText(
                    this,
                    "تم تجهيز الطلب على الهاتف",
                    Toast.LENGTH_LONG
                ).show()
            }
        }

        setContentView(layout)
    }
}
