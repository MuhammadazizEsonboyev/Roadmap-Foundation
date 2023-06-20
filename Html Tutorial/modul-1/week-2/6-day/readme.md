## CSS displeyi

CSS Layout - displey xususiyati

Tartibni boshqarish uchun eng muhim CSS xususiyati "displey" xususiyati bo'lib, u qanday qilib

element ko'rsatilishi kerak. Ko'pgina HTML elementlari uchun standart displey qiymati blok yoki inline hisoblanadi


Blok darajasidagi elementlar


Blok darajasidagi element har doim yangi satrdan boshlanadi va mavjud bo'lgan to'liq kenglikni egallaydi (

iloji boricha chap va o'ng).
<div> elementi blok darajasidagi element hisoblanadi.

Blok darajasidagi elementlarga misollar:

     <div>
     <h1> - <h6>
     <p>
     <form>
     <sarlavha>
     <footer>
     <bo'lim>


Inline elementlar

Inline elementlar

Inline element yangi satrda boshlanmaydi va faqat kerak bo'lganda shuncha kenglikni egallaydi.

Bu paragraf ichidagi satr <span> elementidir.

Inline elementlarga misollar:

     <span>
     <a>
     <img>


Displey: yo'q;

ko'rsatish: yo'q; odatda JavaScript bilan elementlarni oʻchirmasdan va qayta yaratmasdan yashirish va koʻrsatish uchun ishlatiladi

ular. Bunga qanday erishish mumkinligini bilmoqchi bo'lsangiz, ushbu sahifadagi so'nggi misolimizni ko'rib chiqing.

<script> elementi displeydan foydalanadi: none; sukut bo'yicha.






Standart ko'rsatish qiymatini bekor qiling
Har bir elementning standart displey qiymatini bekor qilish uchun oddiy elementni blok elementiga o'zgartiring

yoki aksincha. Bu shuningdek, veb-sahifani o'zingiz yoqtirgan tarzda qilish imkonini beradi

standartlar. Quyidagi rasmga qarang:


<!DOCTYPE html>
<html>
<head>
<uslub>
li {
   displey: inline;
}
</style>
</head>
<tana>

<p>Havolalar roʻyxatini gorizontal menyu sifatida koʻrsatish:</p>

<ul>
   <li><a href="/html/default.asp" target="_blank">HTML</a></li>
   <li><a href="/css/default.asp" target="_blank">CSS</a></li>
   <li><a href="/js/default.asp" target="_blank">JavaScript</a></li>
</ul>

</body>
</html>


Eslatma: Elementning ko'rsatish xususiyatini o'rnatish faqat elementning qanday ko'rsatilishini o'zgartiradi, qanday turdagi emas

element hisoblanadi. Shunday qilib, displeyli inline element: blok; ichida boshqa blok elementlari bo'lishiga yo'l qo'yilmaydi

bu.


<span> elementlarini blok elementlari sifatida ko'rsatish uchun:


<!DOCTYPE html>
<html>
<head>
<uslub>
oraliq {
   displey: blok;
}
</style>
</head>
<tana>

<span>"Blok" qiymatiga ega bo'lgan ko'rsatish xususiyati</span> <span>ikkisi o'rtasida qator uzilishiga olib keladi

elementlar.</span>

</body>
</html>



Quyidagi misolda <a> elementlar blok elementlari sifatida ko‘rsatilgan:


<!DOCTYPE html>
<html>
<head>
<uslub>
a {
   displey: blok;
}
</style>
</head>
<tana>

<p>Havolalarni blok elementlari sifatida ko'rsatish:</p>

<a href="/html/default.asp" target="_blank">HTML</a>
<a href="/css/default.asp" target="_blank">CSS</a>
<a href="/js/default.asp" target="_blank">JavaScript</a>

</body>
</html>



Elementni yashirish - displey: yo'q yoki ko'rinish: yashirinmi?

Displey xususiyatini none ga o'rnatish elementni yashirish va sahifani element kabi ko'rsatish imkonini beradi

u erda yo'q. Quyidagi misolga qarang:


<!DOCTYPE html>
<html>
<head>
<uslub>
h1. yashirin {
   ko'rsatish: yo'q;
}
</style>
</head>
<tana>

<h1>Bu ko'rinadigan sarlavha</h1>
<h1 class="hidden">Bu yashirin sarlavha</h1>
<p>E'tibor bering, h1 elementi displeyli: none; hech qanday joy egallamaydi.</p>

</body>
</html>





Ko'rinishni sozlash: yashirin; elementni ham yashiradi. Biroq, element hali ham bir xil joyni egallaydi

oldin. Element yashirin bo'ladi, lekin baribir tartibga ta'sir qiladi:


<!DOCTYPE html>
<html>
<head>
<uslub>
h1. yashirin {
   ko'rinish: yashirin;
}
</style>
</head>
<tana>

<h1>Bu ko'rinadigan sarlavha</h1>
<h1 class="hidden">Bu yashirin sarlavha</h1>
<p>E'tibor bering, yashirin sarlavha hali ham joy egallaydi.</p>

</body>
</html>


Qo'shimcha misollar:

Displey orasidagi farqlar:none; va ko'rinish: yashirin; quyidagi misolda ko'rsatilgan.

visibility:hidden elementni yashiradi, lekin u baribir tartibda joy egallaydi.

display:none elementni hujjatdan olib tashlamaydi. Hech qanday joy egallamaydi.
<!DOCTYPE html>
<html>
<head>
<uslub>
.imgbox {
   float: chap;
   matnni tekislash: markaz;
   kengligi: 120px;
   chegara: 1px qattiq kulrang;
   chegara: 4px;
   to'ldirish: 6px;
}

tugma {
   kengligi: 100%;
}
</style>
</head>
<tana>

<h3>Displey: yo'q va ko'rinish: yashirin</h3> o'rtasidagi farq
<p><strong>visibility:hidden</strong> elementni yashiradi, lekin u baribir tartibda joy egallaydi.</p>
<p><strong>display:none</strong> hujjatdan elementni olib tashlaydi. U joy egallamaydi.</p>

<div class="imgbox" id="imgbox1">1-quti<br>
   <img src="img_5terre.jpg" alt="Italiya" style="width:100%">
   <button onclick="removeElement()">O'chirish</button>
</div>

<div class="imgbox" id="imgbox2">2-quti<br>
   <img src="img_lights.jpg" alt="Chiroqlar" style="width:100%">
   <button onclick="changeVisibility()">Yashirish</button>
</div>

<div class="imgbox">3-quti<br>
   <img src="img_forest.jpg" alt="O'rmon" style="width:100%">
   <button onclick="resetElement()">Hammasini tiklash</button>
</div>

<skript>
removeElement() funksiyasi {
   document.getElementById("imgbox1").style.display = "yo'q";
}

funktsiyani o'zgartirishVisibility() {
   document.getElementById("imgbox2").style.visibility = "yashirin";
}

funktsiya resetElement() {
   document.getElementById("imgbox1").style.display = "blok";
   document.getElementById("imgbox2").style.visibility = "ko'rinadigan";
}
</script>

</body>
</html>



Quyida ko'rsatilgandek bosish orqali elementni ko'rsatish uchun CSS Javascript bilan birgalikda ishlatilishi mumkin:

CSS displey/ko'rinish xususiyatlari
Mulk tavsifi
displey Element qanday ko'rsatilishi kerakligini belgilaydi
visibility Element ko'rinadigan yoki ko'rinmasligini belgilaydi

<kbd>qaytish</kbd>[Mundarijaga qaytish](#homepage)


--------

## HTML Iframes

U boshqa veb-sahifa ichida veb-sahifani ko'rsatish uchun ishlatiladi

* HTML Iframe sintaksisi

HTML Iframe sintaksisi:

```<iframe>``` tegi chiziqli ramkani belgilaydi. Ushbu inline ramka joriy html hujjatiga boshqa hujjatni joylashtirish uchun ishlatiladi

** Quyida sintaksis misoli

```<iframe src="url" title="ta'rif">```

Eslatma: Har doim <iframe> uchun nom atributini kiritish yaxshi amaliyotdir. Bu ekran o'quvchilari tomonidan iframe tarkibi nima ekanligini o'qish uchun ishlatiladi.


** Iframe o'lchamini belgilash uchun balandlik va kenglikdan foydalaning
```
<iframe src="demo_iframe.htm" height="200" width="300" title="Iframe misoli"></iframe>
```

** Shuningdek, siz uslub atributini qo'shishingiz va CSS balandligi va kengligi xususiyatlaridan foydalanishingiz mumkin:
```
<iframe src="demo_iframe.htm" style="height:200px;width:300px;" title="Iframe misoli"></iframe>
```
** Iframe - chegarani olib tashlang

* Chegara qo'shish uslubi atributini olib tashlash va CSS chegara xususiyatidan foydalanish.
```
<iframe src="demo_iframe.htm" style="border:none;" title="Iframe misoli"></iframe>
```

* Iframe chegarasining o'lchami va rangini o'zgartirish uchun CSS uslubidan ham foydalanishingiz mumkin:

```
<iframe src="demo_iframe.htm" style="border:2px qattiq qizil;" title="Iframe misoli"></iframe>
```

Iframe - havola uchun maqsad

Iframe havola uchun maqsadli ramka sifatida ishlatilishi mumkin. Havolaning maqsadli atributi iframe nomi atributiga murojaat qilishi kerak
```
<iframe src="demo_iframe.htm" name="iframe_a" title="Iframe misoli"></iframe>

<p><a href="https://www.w3schools.com" target="iframe_a">W3Schools.com</a></p>
```

** Agar havolaning maqsadli atributi iframe nomiga mos kelsa, havola iframe-da ochiladi.


Aslini olganda, url maqsadi yangi (_blank) sahifa boʻlishi va iframe nomi (atributi) ham boʻlishi mumkin.

<kbd>qaytish</kbd>[Mundarijaga qaytish](#homepage)

---------

## HTML JavaScript
HTML-ga Javascriptning kiritilishi uni yanada interaktiv va dinamik qiladi.


** Quyida sana va vaqtni ko'rsatadigan tugma mavjud.
```
<!DOCTYPE html>
<html>
<tana>

<h1>Mening birinchi JavaScriptim</h1>

<button type="tugma"
onclick="document.getElementById('demo').innerHTML = Sana()">
Sana va vaqtni ko'rsatish uchun meni bosing.</button>

<p id="demo"></p>

</body>
</html>
```

* HTML skript yorlig'i.

U mijoz tomoni JavaScript-ni belgilaydi... <script> elementi skript bayonotini o'z ichiga oladi yoki src atributi orqali tashqi skriptga ishora qiladi. JS tasvirni manipulyatsiya qilish, shaklni tekshirish va tarkibni dinamik o'zgartirish uchun ishlatiladi.

HTML elementini tanlash uchun JavaScript ko'pincha ```document.getElementById()``` usulidan foydalanadi.

Ushbu JavaScript misolida "Salom JavaScript!" id="demo" bilan HTML elementiga:
```
<h2>Matnni o'zgartirish uchun JavaScript-dan foydalaning</h2>
<p>Ushbu misolda "Salom JavaScript!" id="demo" bilan HTML elementiga:</p>

<p id="demo"></p>

<skript>
document.getElementById("demo").innerHTML = "Salom JavaScript!";
</script>
```

** HTML hujjatining uslubini o'zgartirish uchun JavaScript-dan foydalaning
```
<h1>Mening birinchi JavaScriptim</h1>

<p id="demo">JavaScript HTML elementining uslubini o'zgartirishi mumkin.</p>

<skript>
funktsiya myFunction() {
   document.getElementById("demo").style.fontSize = "25px";
   document.getElementById("demo").style.color = "qizil";
   document.getElementById("demo").style.backgroundColor = "sariq";
}
</script>

<button type="button" onclick="myFunction()">Menga bosing!</button>
```

** Rasmning src atributini oʻzgartirish uchun Javascriptdan foydalaning.
```document.getElementById("rasm").src = "rasm.gif";```

* quyida to'liq kodni ko'ring
```
<h1>Mening birinchi JavaScriptim</h1>
<p>Bu yerda JavaScript tasvirning src (manba) atributining qiymatini oʻzgartiradi.</p>

<skript>
funktsiya nuri (sw) {
   var pic;
   agar (sw == 0) {
     pic = "pic_bulboff.gif"
   } boshqa {
     pic = "pic_bulbon.gif"
   }
   document.getElementById('myImage').src = pic;
}
</script>

<img id="myImage" src="pic_bulboff.gif" width="100" height="180">

<p>
<button type="button" onclick="light(1)">Chiroq yoqilgan</button>
<button type="button" onclick="light(0)">Chiroq o'chirilgan</button>
</p>
```

* HTML ```<noscript>``` tegi

Brauzerlarida skriptlarni o‘chirib qo‘ygan yoki skriptlarni qo‘llab-quvvatlamaydigan brauzerlarga ega foydalanuvchilarga ko‘rsatiladigan muqobil kontentni belgilaydi.

* Bu skript
```
<skript>
document.getElementById("demo").innerHTML = "Salom JavaScript!";
</script>
<noscript>Kechirasiz, brauzeringiz JavaScript-ni qo‘llab-quvvatlamaydi!</noscript>

**To'liq skript:
<p id="demo"></p>

<skript>
document.getElementById("demo").innerHTML = "Salom JavaScript!";
</script>

<noscript>Kechirasiz, brauzeringiz JavaScript-ni qo‘llab-quvvatlamaydi!</noscript>

<p>JavaScript-ni qo'llab-quvvatlamaydigan brauzer noscript elementi ichida yozilgan matnni ko'rsatadi.</p>
```
<kbd>qaytish</kbd>[Mundarijaga qaytish](#homepage)