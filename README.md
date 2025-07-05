<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>وكيل سحب وإيداع</title>
  <style>
    body {
      font-family: 'Tahoma', sans-serif;
      background: #f2f2f2;
      margin: 0;
      padding: 0;
      direction: rtl;
    }
    header {
      background: #2e2e2e;
      color: white;
      padding: 20px;
      text-align: center;
    }
    section {
      padding: 20px;
      max-width: 700px;
      margin: auto;
      background: white;
      margin-top: 20px;
      border-radius: 10px;
    }
    h2 {
      color: #333;
    }
    input, select, textarea, button {
      width: 100%;
      padding: 10px;
      margin-top: 10px;
      margin-bottom: 20px;
      border: 1px solid #ccc;
      border-radius: 5px;
    }
    button {
      background: #4CAF50;
      color: white;
      border: none;
      cursor: pointer;
    }
    button:hover {
      background: #45a049;
    }
    footer {
      text-align: center;
      padding: 20px;
      font-size: 14px;
      color: #777;
    }
    .contact {
      text-align: center;
    }
    .wallet-info {
      background: #f9f9f9;
      border: 1px solid #ccc;
      padding: 15px;
      margin-top: 10px;
      border-radius: 10px;
    }
    .wallet-info p {
      margin: 5px 0;
    }
  </style>
</head>
<body>
  <header>
    <h1>وكيل سحب وإيداع معتمد</h1>
    <p>متاح 24 ساعة لخدمتكم</p>
  </header>

  <section>
    <h2>أرقام المحافظ للتحويل</h2>
    <div class="wallet-info">
      <p><strong>فودافون كاش:</strong> 01124725116</p>
      <p><strong>اتصالات كاش:</strong> 01124725116</p>
      <p><strong>بايير:</strong> P12345678</p>
      <p><strong>USDT TRC20:</strong> TX7xyzabc1234567890</p>
    </div>
  </section>

  <section>
    <h2>طلب إيداع</h2>
    <form>
      <label>اسمك:</label>
      <input type="text" required />
      <label>رقم حسابك على الموقع:</label>
      <input type="text" required />
      <label>المبلغ المطلوب إيداعه:</label>
      <input type="number" required />
      <label>وسيلة التحويل:</label>
      <select>
        <option>فودافون كاش</option>
        <option>اتصالات كاش</option>
        <option>بايير</option>
        <option>USDT</option>
      </select>
      <label>التطبيق الذي تريد الشحن عليه:</label>
      <select>
        <option>DB BET</option>
        <option>1XBET</option>
        <option>MELBET</option>
        <option>XPARIBET</option>
        <option>WINWIN</option>
      </select>
      <label>ارفق صورة التحويل:</label>
      <input type="file" accept="image/*" />
      <p style="color: #555; font-size: 14px;">بعد اختيار الصورة، يُرجى إرسالها على <a href="https://wa.me/201124725116" target="_blank">واتساب</a> أو <a href="https://t.me/username" target="_blank">تيليجرام</a>.</p>
      <button type="submit">إرسال الطلب</button>
    </form>
  </section>

  <section>
    <h2>طلب سحب</h2>
    <form>
      <label for="withdrawApp">اختر التطبيق الذي تسحب منه:</label>
      <select id="withdrawApp" name="withdrawApp" onchange="showPopup()">
        <option value="">-- اختر --</option>
        <option value="DBBET">DB BET</option>
        <option value="1XBET">1XBET</option>
        <option value="MELBET">MELBET</option>
        <option value="WINWIN">WINWIN</option>
        <option value="XPARIBET">XPARI BET</option>
      </select>
      <div id="popup" style="display:none; padding:10px; border:1px solid #ccc; margin-top:10px;">
        <span style="cursor:pointer;" onclick="hidePopup()">✖</span>
        <p><strong>اسم المدينة:</strong> Khusus</p>
        <p><strong>اسم الشارع:</strong> babaElmagal(wallet)</p>
      </div>
      <label for="withdrawCode">قم بإرسال كود السحب هنا:</label>
      <input type="text" id="withdrawCode" name="withdrawCode" placeholder="ادخل كود السحب" required>
      <label for="withdrawScreenshot">ارفق صورة لعملية التحويل:</label>
      <input type="file" id="withdrawScreenshot" name="withdrawScreenshot" accept="image/*">
      <p style="font-size: 14px; color: #555;">
        بعد اختيار الصورة، يُرجى إرسالها إلى واتساب:
        <a href="https://wa.me/201066070695" target="_blank">اضغط هنا</a>
        أو تيليجرام:
        <a href="https://t.me/username" target="_blank">@username</a>
      </p>
      <p>التحويل إلى فودافون كاش على الرقم: <strong>01066070695</strong></p>
      <button type="submit">إرسال الطلب</button>
    </form>
  </section>

  <section>
    <h2>تواصل معنا</h2>
    <div class="contact">
      <p>واتساب: <a href="https://wa.me/201124725116" target="_blank">اضغط هنا</a></p>
      <p>تيليجرام: <a href="https://t.me/username" target="_blank">t.me/username</a></p>
    </div>
  </section>

  <footer>
    جميع الحقوق محفوظة &copy; 2025
  </footer>

  <script>
    function showPopup() {
      var sel = document.getElementById("withdrawApp").value;
      document.getElementById("popup").style.display = sel ? "block" : "none";
    }
    function hidePopup() {
      document.getElementById("popup").style.display = "none";
      document.getElementById("withdrawApp").value = "";
    }
  </script>
</body>
</html>
