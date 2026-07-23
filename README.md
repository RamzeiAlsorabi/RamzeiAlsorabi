<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>سيرتي الذاتية - تقنية معلومات</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        body {
            background: linear-gradient(-45deg, #0f0c29, #302b63, #24243e);
            background-size: 400% 400%;
            animation: gradient 15s ease infinite;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            color: #fff;
            min-height: 100vh;
            padding: 30px 15px;
        }
        @keyframes gradient {
            0% {background-position: 0% 50%;}
            50% {background-position: 100% 50%;}
            100% {background-position: 0% 50%;}
        }

        .container {
            max-width: 750px;
            margin: auto;
        }

        /* البطاقات الزجاجية */
        .glass-card {
            background: rgba(255, 255, 255, 0.08);
            backdrop-filter: blur(12px);
            border-radius: 25px;
            border: 1px solid rgba(255, 255, 255, 0.15);
            padding: 30px 25px;
            margin-bottom: 25px;
            box-shadow: 0 20px 35px rgba(0,0,0,0.4);
        }

        /* البطاقة التعريفية */
        .profile-header {
            text-align: center;
        }
        .avatar {
            width: 100px;
            height: 100px;
            border-radius: 50%;
            background: linear-gradient(135deg, #00c6ff, #0072ff);
            margin: 0 auto 15px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 45px;
            box-shadow: 0 8px 25px rgba(0,198,255,0.4);
            border: 3px solid rgba(255,255,255,0.25);
        }
        .name {
            font-size: 32px;
            font-weight: bold;
        }
        .specialty {
            font-size: 20px;
            background: rgba(0,198,255,0.2);
            display: inline-block;
            padding: 6px 22px;
            border-radius: 30px;
            margin: 10px 0 5px;
        }
        .level {
            font-size: 18px;
            opacity: 0.9;
            margin-bottom: 10px;
        }

        h2 {
            font-size: 22px;
            margin-bottom: 18px;
            display: flex;
            align-items: center;
            gap: 10px;
            border-bottom: 1px solid rgba(255,255,255,0.2);
            padding-bottom: 10px;
        }
        h2 i {
            font-style: normal;
            font-size: 24px;
        }

        /* شريط المهارات */
        .skill-item {
            margin-bottom: 15px;
        }
        .skill-info {
            display: flex;
            justify-content: space-between;
            margin-bottom: 5px;
        }
        .skill-bar {
            height: 10px;
            background: rgba(255,255,255,0.15);
            border-radius: 10px;
            overflow: hidden;
        }
        .skill-fill {
            height: 100%;
            width: 0%;
            background: linear-gradient(90deg, #00c6ff, #0072ff);
            border-radius: 10px;
            transition: width 1s ease;
        }

        /* الجدول الزمني - سيرة ذاتية */
        .timeline-item {
            display: flex;
            gap: 15px;
            margin-bottom: 20px;
            position: relative;
        }
        .timeline-icon {
            width: 40px;
            height: 40px;
            background: rgba(0,198,255,0.2);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            flex-shrink: 0;
        }
        .timeline-content h3 {
            font-size: 18px;
            margin-bottom: 3px;
        }
        .timeline-content span {
            font-size: 14px;
            opacity: 0.7;
            display: block;
            margin-bottom: 4px;
        }

        .contact-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 15px;
        }
        .contact-item {
            background: rgba(255,255,255,0.05);
            padding: 12px;
            border-radius: 12px;
            text-align: center;
            font-size: 15px;
        }
        a {
            color: #7dd3fc;
            text-decoration: none;
        }

        @media (max-width: 500px) {
            .contact-grid {
                grid-template-columns: 1fr;
            }
        }

        /* animation for bars */
        .show .skill-fill {
            /* widths are set inline via style attribute or we can set them manually */
        }
    </style>
</head>
<body>
    <div class="container">

        <!-- البطاقة التعريفية -->
        <div class="glass-card profile-header">
            <div class="avatar">🎓</div>
            <!-- 👇 غير إلى اسمك -->
            <div class="name">أحمد محمد</div>
            <div class="specialty">تقنية المعلومات</div>
            <div class="level">المستوى الثالث</div>
            <p style="margin-top:15px; opacity:0.8;">🎯 أسعى لاكتساب خبرة عملية في تطوير الويب والشبكات</p>
        </div>

        <!-- المهارات التقنية -->
        <div class="glass-card">
            <h2><i>⚙️</i> المهارات التقنية</h2>
            <!-- كل مهارة تقدر تغير النسبة المئوية -->
            <div class="skill-item">
                <div class="skill-info"><span>HTML & CSS</span><span>85%</span></div>
                <div class="skill-bar"><div class="skill-fill" style="width: 85%;"></div></div>
            </div>
            <div class="skill-item">
                <div class="skill-info"><span>JavaScript</span><span>60%</span></div>
                <div class="skill-bar"><div class="skill-fill" style="width: 60%;"></div></div>
            </div>
            <div class="skill-item">
                <div class="skill-info"><span>شبكات الحاسب</span><span>70%</span></div>
                <div class="skill-bar"><div class="skill-fill" style="width: 70%;"></div></div>
            </div>
            <div class="skill-item">
                <div class="skill-info"><span>أمن المعلومات</span><span>50%</span></div>
                <div class="skill-bar"><div class="skill-fill" style="width: 50%;"></div></div>
            </div>
            <div class="skill-item">
                <div class="skill-info"><span>Python</span><span>65%</span></div>
                <div class="skill-bar"><div class="skill-fill" style="width: 65%;"></div></div>
            </div>
        </div>

        <!-- السيرة الذاتية / التعليم والخبرات -->
        <div class="glass-card">
            <h2><i>📋</i> السيرة الذاتية</h2>
            <div class="timeline-item">
                <div class="timeline-icon">🎓</div>
                <div class="timeline-content">
                    <h3>بكالوريوس تقنية معلومات</h3>
                    <span>2024 - الآن | جامعة العلوم والتكنولوجيا</span>
                    <p>المستوى الثالث – معدل 4.2 من 5</p>
                </div>
            </div>
            <div class="timeline-item">
                <div class="timeline-icon">💼</div>
                <div class="timeline-content">
                    <h3>مشروع تطوير موقع تعريفي</h3>
                    <span>2025 | مشروع جامعي</span>
                    <p>صممت موقعًا تعريفيًا للكلية باستخدام HTML وCSS وJavaScript</p>
                </div>
            </div>
            <div class="timeline-item">
                <div class="timeline-icon">📜</div>
                <div class="timeline-content">
                    <h3>شهادة CCNA (مبادئ الشبكات)</h3>
                    <span>2025 | دورة عبر الإنترنت</span>
                    <p>فهم أساسيات الشبكات والتوجيه والتحويل</p>
                </div>
            </div>
            <!-- تقدر تضيف المزيد من الخبرات بنفس التنسيق -->
        </div>

        <!-- التواصل -->
        <div class="glass-card">
            <h2><i>📬</i> تواصل معي</h2>
            <div class="contact-grid">
                <div class="contact-item">📧 <br>ahmed@example.com</div>
                <div class="contact-item">📱 <br>+966 5X XXX XXXX</div>
                <div class="contact-item">💼 <br><a href="#">linkedin.com/in/ahmed</a></div>
                <div class="contact-item">🐙 <br><a href="#">github.com/ahmed</a></div>
            </div>
        </div>

        <p style="text-align:center; opacity:0.6; margin-top:10px;">© 2025 جميع الحقوق محفوظة</p>
    </div>

    <!-- تأثير بسيط لظهور المهارات عند التمرير (اختياري) -->
    <script>
        // لا حاجة لتعديل هذا السكربت، فقط يحسّن العرض
        const observer = new IntersectionObserver(entries => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.classList.add('show');
                }
            });
        }, {threshold:0.3});
        document.querySelectorAll('.skill-fill').forEach(el => observer.observe(el));
    </script>
</body>
</html>
