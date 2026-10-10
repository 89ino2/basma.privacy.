# basma.privacy.
Basma Privacy 🦊 | A privacy awareness website providing educational guidance on microphone permissions, account security, and protecting personal information online.

<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Luma</title>
<style>
*{box-sizing:border-box}
body{margin:0;font-family:Arial;background:#fff5cf;color:#641f35;
display:grid;place-items:center;min-height:100vh}
.card{background:#fffdf5;padding:30px;border-radius:24px;
width:min(90%,380px);box-shadow:0 12px 35px #641f3515}
h1{text-align:center;font-size:36px}
p{text-align:center;color:#866773}
input,button{width:100%;padding:14px;margin-top:12px;
border-radius:12px;font-size:16px}
input{border:1px solid #ead8ad;background:white}
button{border:0;background:#641f35;color:white;cursor:pointer}
#home{display:none}
</style>
</head>
<body>
<div class="card" id="login">
<h1>Luma</h1>
<p>أهلاً بيج، سجّلي دخولج</p>
<form id="form">
<input id="email" type="email" placeholder="البريد الإلكتروني" required>
<input id="password" type="password" placeholder="كلمة المرور" required>
<button type="submit">تسجيل الدخول</button>
</form>
<p id="message"></p>
</div>

<div class="card" id="home">
<h1>أهلاً بيج ✨</h1>
<p>نورتي عالم Luma</p>
<button onclick="logout()">تسجيل الخروج</button>
</div>

<script>
const form=document.getElementById('form');
form.addEventListener('submit',function(e){
 e.preventDefault();
 document.getElementById('login').style.display='none';
 document.getElementById('home').style.display='block';
});
function logout(){
 document.getElementById('home').style.display='none';
 document.getElementById('login').style.display='block';
}
</script>
</body>
</html>
