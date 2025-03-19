<!DOCTYPE html>
<html lang="ar">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>مؤسسة أعمال المنزل للصيانة المنزلية</title>
    <style>
        body { font-family: Arial, sans-serif; text-align: center; direction: rtl; }
        .container { max-width: 500px; margin: auto; padding: 20px; border: 1px solid #ddd; border-radius: 10px; }
        .icon { display: inline-block; margin: 15px; padding: 15px; border: 1px solid #ccc; cursor: pointer; }
        .form-container { display: none; margin-top: 20px; }
        input, select, button { display: block; width: 100%; padding: 10px; margin: 10px 0; }
        .contact { margin-top: 20px; }
    </style>
</head>
<body>
    <h1>مؤسسة أعمال المنزل للصيانة المنزلية</h1>
    <div class="container">
        <h2>الخدمات</h2>
        <div class="icon" onclick="showForm()">🔧 صيانة التكييف</div>
        <div class="icon" onclick="showForm()">💡 صيانة الكهرباء</div>
        <div class="icon" onclick="showForm()">🚰 صيانة الأدوات الصحية والسباكة</div>
        
        <div class="form-container" id="serviceForm">
            <h3>طلب الخدمة</h3>
            <input type="text" placeholder="الاسم" required>
            <input type="tel" placeholder="رقم الجوال" required>
            <select>
                <option>أبها</option>
                <option>خميس مشيط</option>
            </select>
            <input type="text" placeholder="اسم الحي" required>
            <input type="text" placeholder="الوقت المناسب" required>
            <button onclick="submitForm()">إرسال الطلب</button>
        </div>
    </div>
    
    <div class="contact">
        <h3>للتواصل</h3>
        <p>📞 0545162361</p>
        <p>⏰ أوقات الدوام: من 8 صباحًا إلى 10 مساءً</p>
    </div>

    <script>
        function showForm() {
            document.getElementById("serviceForm").style.display = "block";
        }
        function submitForm() {
            alert("تم إرسال الطلب بنجاح!");
        }
    </script>
</body>
</html>
