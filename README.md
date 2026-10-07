<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>موقعي الشخصي</title>
    <!-- استدعاء خط عربي أنيق -->
    <link href="https://fonts.googleapis.com/css2?family=Cairo:wght@400;600;700&display=swap" rel="stylesheet">
    <style>
        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
            font-family: 'Cairo', sans-serif;
        }

        body {
            /* ألوان خلفية متدرجة وجذابة */
            background: linear-gradient(135deg, #667eea 0%, #764ba2 50%, #f64f59 100%);
            height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            overflow: hidden;
        }

        /* حاوية الموقع الشخصي في المنتصف تماماً */
        .profile-container {
            background: rgba(255, 255, 255, 0.15);
            backdrop-filter: blur(15px);
            -webkit-backdrop-filter: blur(15px);
            border: 1px solid rgba(255, 255, 255, 0.3);
            border-radius: 20px;
            padding: 40px 30px;
            width: 100%;
            max-width: 400px;
            box-shadow: 0 15px 35px rgba(0, 0, 0, 0.2);
            text-align: center; /* توسيط كل النص داخل الحاوية */
        }

        h1 {
            color: #ffffff;
            margin-bottom: 25px;
            font-size: 26px;
            font-weight: 700;
            text-align: center;
        }

        .input-group {
            margin-bottom: 20px;
            width: 100%;
        }

        /* توسيط كل محتويات حقول الإدخال والنصوص بداخلها */
        input {
            width: 100%;
            padding: 14px 20px;
            background: rgba(255, 255, 255, 0.2);
            border: 1px solid rgba(255, 255, 255, 0.4);
            border-radius: 12px;
            color: #fff;
            font-size: 16px;
            text-align: center; /* توسيط الكلام المكتوب والنصوص المؤقتة */
            outline: none;
            transition: all 0.3s ease;
        }

        input::placeholder {
            color: rgba(255, 255, 255, 0.7);
            text-align: center; /* ضمان توسيط النص المؤقت */
        }

        input:focus {
            background: rgba(255, 255, 255, 0.3);
            border-color: #ffffff;
            box-shadow: 0 0 15px rgba(255, 255, 255, 0.4);
        }

        .btn-submit {
            width: 100%;
            padding: 14px;
            background: linear-gradient(135deg, #f093fb 0%, #f5576c 100%);
            border: none;
            border-radius: 12px;
            color: white;
            font-size: 18px;
            font-weight: 600;
            cursor: pointer;
            transition: all 0.3s ease;
            margin-top: 10px;
            text-align: center;
            box-shadow: 0 5px 15px rgba(245, 87, 108, 0.4);
        }

        .btn-submit:hover {
            transform: translateY(-2px);
            box-shadow: 0 8px 20px rgba(245, 87, 108, 0.6);
        }
    </style>
</head>
<body>

    <div class="profile-container">
        <h1>موقعي الشخصي</h1>
        
        <form>
            <div class="input-group">
                <input type="text" placeholder="اسم المستخدم أو البريد الإلكتروني" required>
            </div>
            
            <div class="input-group">
                <input type="password" placeholder="كلمة المرور" required>
            </div>
            
            <button type="submit" class="btn-submit">دخول</button>
        </form>
    </div>

</body>
</html>
