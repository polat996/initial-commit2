# initial-commit2
<!DOCTYPE html>
<html lang="ar">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>موقعي الشخصي - صفحة واحدة</title>
    <style>
        /* CSS للتنسيق الأساسي للموقع */
        body {
            font-family: 'Arial', sans-serif;
            margin: 0;
            padding: 0;
            box-sizing: border-box; /* لضمان أن الحشوة والحدود لا تزيد عن عرض العنصر */
            scroll-behavior: smooth; /* لجعل التمرير إلى الأقسام سلسًا */
            background-color: #f4f4f4;
            color: #333;
        }

        /* رأس الصفحة */
        header {
            background-color: #333;
            color: white;
            padding: 1rem 0;
            text-align: center;
        }

        header h1 {
            margin: 0;
            font-size: 2.5rem;
        }

        /* قائمة التنقل */
        nav {
            background-color: #444;
            padding: 0.5rem 0;
            text-align: center;
        }

        nav ul {
            list-style: none;
            padding: 0;
            margin: 0;
            display: flex; /* لعرض العناصر بجانب بعضها */
            justify-content: center; /* لتوسيط العناصر */
        }

        nav ul li {
            margin: 0 15px;
        }

        nav ul li a {
            color: white;
            text-decoration: none;
            font-weight: bold;
            padding: 5px 10px;
            transition: background-color 0.3s ease;
        }

        nav ul li a:hover {
            background-color: #555;
            border-radius: 5px;
        }

        /* الأقسام الرئيسية */
        section {
            padding: 60px 20px; /* حشوة علوية وسفلية أكبر */
            margin: 20px auto;
            max-width: 900px;
            background-color: white;
            border-radius: 8px;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
            text-align: center; /* توسيط المحتوى داخل القسم */
        }

        section:nth-of-type(even) { /* تنسيق مختلف للأقسام الزوجية */
            background-color: #e9e9e9;
        }

        section h2 {
            color: #0056b3;
            font-size: 2rem;
            margin-bottom: 20px;
            position: relative;
            padding-bottom: 10px;
        }

        section h2::after { /* خط تحت العنوان */
            content: '';
            position: absolute;
            left: 50%;
            bottom: 0;
            transform: translateX(-50%);
            width: 80px;
            height: 3px;
            background-color: #007bff;
            border-radius: 5px;
        }

        /* تذييل الصفحة */
        footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 1.5rem 0;
            margin-top: 30px;
        }

        /* تنسيق خاص بصفحة الاتصال */
        #contact form {
            display: flex;
            flex-direction: column;
            gap: 15px;
            max-width: 500px;
            margin: 0 auto;
        }

        #contact label {
            text-align: right;
            margin-bottom: 5px;
            font-weight: bold;
        }

        #contact input[type="text"],
        #contact input[type="email"],
        #contact textarea {
            padding: 12px;
            border: 1px solid #ddd;
            border-radius: 5px;
            font-size: 1rem;
            width: 100%; /* لضمان أن تأخذ 100% من العرض المتاح في الـ flex-direction column */
            box-sizing: border-box; /* للحفاظ على العرض ثابتًا مع الحشوة */
        }

        #contact textarea {
            resize: vertical; /* السماح بتغيير حجم مربع النص عموديا فقط */
            min-height: 100px;
        }

        #contact button {
            background-color: #007bff;
            color: white;
            padding: 12px 20px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            font-size: 1.1rem;
            transition: background-color 0.3s ease;
        }

        #contact button:hover {
            background-color: #0056b3;
        }

        /* تنسيقات إضافية للمحتوى داخل الأقسام */
        .section-content {
            margin-top: 20px;
            line-height: 1.8;
            font-size: 1.1rem;
        }
    </style>
</head>
<body>

    <header>
        <h1>موقعنا المميز</h1>
        <p>مكانك الأمثل لاكتشاف ما نقدمه</p>
    </header>

    <nav>
        <ul>
            <li><a href="#about">من نحن</a></li>
            <li><a href="#services">خدماتنا</a></li>
            <li><a href="#contact">اتصل بنا</a></li>
        </ul>
    </nav>

    <section id="about">
        <h2>من نحن</h2>
        <div class="section-content">
            <p>مرحباً بك في موقعنا! نحن فريق من المتخصصين الملتزمين بتقديم أفضل الحلول والخدمات لعملائنا. نسعى دائمًا للابتكار والتفوق في كل ما نقوم به، ونؤمن بأن الجودة هي مفتاح النجاح. مهمتنا هي بناء علاقات طويلة الأمد مع عملائنا من خلال تقديم قيمة حقيقية ودعم متواصل.</p>
            <p>لدينا خبرة واسعة في [اذكر مجالات خبرتك، مثل: تطوير الويب، التسويق الرقمي، التصميم الجرافيكي]، ونعمل بشغف لتحويل أفكارك إلى واقع ملموس.</p>
        </div>
    </section>

    <section id="services">
        <h2>خدماتنا</h2>
        <div class="section-content">
            <p>نقدم مجموعة واسعة من الخدمات المصممة لتلبية احتياجاتك المتنوعة. إليك بعض من أبرز خدماتنا:</p>
            <ul>
                <li>**تطوير الويب:** تصميم وتطوير مواقع إلكترونية متجاوبة وعصرية.</li>
                <li>**التسويق الرقمي:** استراتيجيات تسويقية فعالة لزيادة تواجدك على الإنترنت.</li>
                <li>**استشارات تقنية:** تقديم النصح والإرشاد للمشاريع التقنية.</li>
                <li>**التصميم الجرافيكي:** إنشاء تصاميم جذابة ومبتكرة لعلامتك التجارية.</li>
            </ul>
            <p>نحن نعمل معك خطوة بخطوة لضمان تحقيق أهدافك بأفضل صورة ممكنة.</p>
        </div>
    </section>

    <section id="contact">
        <h2>اتصل بنا</h2>
        <div class="section-content">
            <p>هل لديك أي أسئلة أو استفسارات؟ لا تتردد في التواصل معنا. يسعدنا دائمًا سماعك!</p>
            <form action="#" method="POST">
                <label for="name">الاسم الكامل:</label>
                <input type="text" id="name" name="name" required>

                <label for="email">البريد الإلكتروني:</label>
                <input type="email" id="email" name="email" required>

                <label for="message">رسالتك:</label>
                <textarea id="message" name="message" rows="5" required></textarea>

                <button type="submit">إرسال الرسالة</button>
            </form>
            <p style="margin-top: 20px;">يمكنك أيضًا التواصل معنا عبر: info@yourwebsite.com</p>
        </div>
    </section>

    <footer>
        <p>&copy; 2025 موقعنا المميز. جميع الحقوق محفوظة.</p>
    </footer>

</body>
</html>
