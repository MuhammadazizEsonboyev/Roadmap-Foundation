6-qism HTML API
## HTML GEOLOCATION
HTML GEOLOCATION API
* HTML Geolocation API foydalanuvchi pozitsiyasini aniqlash uchun ishlatiladi.

* Foydalanuvchining pozitsiyasini toping

HTML Geolocation API foydalanuvchining geografik joylashuvini olish uchun ishlatiladi.

Bu maxfiylikni buzishi mumkinligi sababli, agar foydalanuvchi ma'qullamasa, pozitsiya mavjud emas.

Eslatma: Geolokatsiya smartfonlar kabi GPSga ega qurilmalar uchun eng aniq hisoblanadi.


Eslatma: Chrome 50 dan boshlab Geolocation API faqat HTTPS kabi xavfsiz kontekstlarda ishlaydi. Agar sizning saytingiz xavfsiz bo'lmagan manbada (masalan, HTTP) joylashtirilgan bo'lsa, foydalanuvchilarning joylashuvini aniqlash so'rovlari endi ishlamaydi.


```getCurrentPosition()``` usuli foydalanuvchi o`rnini qaytarish uchun ishlatiladi.

Quyidagi misol foydalanuvchi joylashuvining kenglik va uzunligini qaytaradi (xatolarsiz asosiy geolokatsiya):
```
<p id="demo"></p>

<skript>
var x = document.getElementById("demo");

getLocation() funksiyasi
   agar (navigator.geolocation) {
     navigator.geolocation.getCurrentPosition(showPosition);
   } boshqa {
     x.innerHTML = "Ushbu brauzer geografik joylashuvni qo'llab-quvvatlamaydi.";
   }
}

funktsiyani ko'rsatishPosition(pozitsiya) {
   x.innerHTML = "Latitude: " + position.coords.latitude +
   "<br>Boylik: " + position.coords.longitude;
}
</script>
```

yuqoridagi kod tushuntirilgan.

Misol tushuntirildi:
Geolocation qo'llab-quvvatlanishini tekshiring
Agar qo'llab-quvvatlansa, ```getCurrentPosition() usuli```ni ishga tushiring. Agar yo'q bo'lsa, foydalanuvchiga xabarni ko'rsating
Agar ```getCurrentPosition()``` usuli muvaffaqiyatli bo`lsa, u koordinatalar obyektini parametrda ko`rsatilgan funksiyaga qaytaradi (showPosition)
```showPosition()``` funksiyasi kenglik va uzunlikni chiqaradi

Yuqoridagi misol juda oddiy Geolocation skripti bo'lib, hech qanday xatolik yo'q.

* Xatolar va rad etishlarni boshqarish

GetCurrentPosition() usulining ikkinchi parametri xatolarni qayta ishlash uchun ishlatiladi. U foydalanuvchining joylashuvini ololmasa, ishga tushirish funksiyasini belgilaydi:
```
<button onclick="getLocation()">Sinab ko'ring</button>

<p id="demo"></p>

<skript>
var x = document.getElementById("demo");

getLocation() funksiyasi
   agar (navigator.geolocation) {
     navigator.geolocation.getCurrentPosition(showPosition, showError);
   } boshqa {
     x.innerHTML = "Ushbu brauzer geografik joylashuvni qo'llab-quvvatlamaydi.";
   }
}

funktsiyani ko'rsatishPosition(pozitsiya) {
   x.innerHTML = "Latitude: " + position.coords.latitude +
   "<br>Boylik: " + position.coords.longitude;
}

funktsiya showError(xato) {
   switch(xato.kod) {
     hodisa xatosi.PERMISSION_DENIED:
       x.innerHTML = "Foydalanuvchi Geolocation so'rovini rad etdi."
       sindirish;
     hodisa xatosi.POSITION_UNAVAILABLE:
       x.innerHTML = "Joylashuv ma'lumoti mavjud emas."
       sindirish;
     hodisa xatosi.TIMEOUT:
       x.innerHTML = "Foydalanuvchi manzilini aniqlash so'rovi vaqti tugadi."
       sindirish;
     hodisa xatosi.UNKNOWN_ERROR:
       x.innerHTML = "Noma'lum xatolik yuz berdi."
       sindirish;
   }
}
</script>
```

* Natijani xaritada ko'rsatish

Natijani xaritada ko'rsatish uchun sizga Google Xaritalar kabi xarita xizmatiga kirishingiz kerak.

Quyidagi misolda qaytarilgan kenglik va uzunlik Google Xaritadagi joylashuvni ko'rsatish uchun ishlatiladi (statik rasm yordamida):

```
funktsiyani ko'rsatishPosition(pozitsiya) {
   var latlon = position.coords.latitude + "," + position.coords.longitude;

   var img_url = "https://maps.googleapis.com/maps/api/staticmap?center=
   "+latlon+"&zoom=14&size=400x300&sensor=false&key=YOUR_KEY";

   document.getElementById("mapholder").innerHTML = "<img src='"+img_url+"'>";
}
```

* Joylashuvga oid ma'lumotlar

Ushbu sahifada foydalanuvchining xaritadagi o'rnini qanday ko'rsatish mumkinligi ko'rsatilgan.

Geolokatsiya shuningdek, joylashuvga oid ma'lumotlar uchun juda foydali, masalan:

    Yangilangan mahalliy ma'lumotlar
    Foydalanuvchi yaqinidagi qiziqish nuqtalarini ko'rsatish
    Navbatma-navbat navigatsiya (GPS)


```getCurrentPosition()``` usuli - Ma'lumotlarni qaytarish

```getCurrentPosition()``` usuli ob'ektni muvaffaqiyatli qaytaradi. Kenglik, uzunlik va aniqlik xususiyatlari har doim qaytariladi. Agar mavjud bo'lsa, boshqa xususiyatlar qaytariladi:
Mulkni qaytarish
coords.latitude O'nlik son sifatida kenglik (har doim qaytariladi)
coords.longitude Uzunlik o'nlik son sifatida (har doim qaytariladi)
coords.accuracy joylashuvning aniqligi (har doim qaytariladi)
koordinatlar.altitude o'rtacha dengiz sathidan metrlarda balandlik (mavjud bo'lsa qaytariladi)
coords.altitudeAccuracy Manzilning balandlik aniqligi (mavjud bo'lsa qaytariladi)
coords.heading Shimoldan soat yo'nalishi bo'yicha gradus bo'yicha sarlavha (mavjud bo'lsa qaytariladi)
coords.speed sekundiga metrdagi tezlik (mavjud bo'lsa qaytariladi)
vaqt tamg'asi Javobning sanasi/vaqti (mavjud bo'lsa qaytariladi)


Geolokatsiya ob'ekti - Boshqa qiziqarli usullar

Geolocation obyektida boshqa qiziqarli usullar ham mavjud:

    ```watchPosition()``` - foydalanuvchining joriy holatini qaytaradi va foydalanuvchi harakatlanayotganda yangilangan pozitsiyasini qaytarishda davom etadi (masalan, mashinadagi GPS).
    ```clearWatch()``` - ```watchPosition()``` usulini to`xtatadi.

Quyidagi misol watchPosition() usulini ko'rsatadi. Buni tekshirish uchun sizga aniq GPS qurilmasi kerak (masalan, smartfon):
```
<p>Koordinatalaringizni olish uchun tugmani bosing.</p>

<button onclick="getLocation()">Sinab ko'ring</button>

<p id="demo"></p>

<skript>
var x = document.getElementById("demo");

getLocation() funksiyasi
   agar (navigator.geolocation) {
     navigator.geolocation.watchPosition(showPosition);
   } boshqa {
     x.innerHTML = "Ushbu brauzer geografik joylashuvni qo'llab-quvvatlamaydi.";
   }
}
    
funktsiyani ko'rsatishPosition(pozitsiya) {
     x.innerHTML="Latitude: " + position.coords.latitude +
     "<br>Boylik: " + position.coords.longitude;
}
</script>

```
<kbd>qaytish</kbd>[Mundarijaga qaytish](#homepage)


------

## CSS navigatsiya paneli

Navigatsiya paneli::

Veb-sayt auditoriyasi uchun uni oson o'tishni topish juda muhimdir. CSS sizga o'zgartirish imkonini beradi

HTML menyularini jozibali navigatsiya paneliga aylantiring.


Navigatsiya paneli = Havolalar ro'yxati

Navigatsiya paneli uchun asos sifatida standart HTML kerak. Ushbu bobdagi misollarda navigatsiya paneli mavjud

standart HTML ro'yxatidan tuzilgan. Navigatsiya panelida <ul> va <li> elementlaridan foydalanish maqsadga muvofiqdir, chunki a

navigatsiya paneli asosan havolalar ro'yxatidir.



Navigatsiya menyusi sifatida oddiy HTML roʻyxatining quyidagi misolini koʻring:

<!DOCTYPE html>
<html>
<tana>

<ul>
   <li><a href="#home">Uy</a></li>
   <li><a href="#news">Yangiliklar</a></li>
   <li><a href="#contact">Aloqa</a></li>
   <li><a href="#about">Haqida</a></li>
</ul>

<p>Eslatma: Sinov havolalari uchun href="#" dan foydalanamiz. Haqiqiy veb-saytda bu URL manzillar bo'ladi.</p>

</body>
</html>


Keyinchalik jozibador ko'rinishi uchun ro'yxatdagi o'qlarni, chekkalarni va to'ldirishlarni olib tashlashimiz mumkin:


<!DOCTYPE html>
<html>
<head>
<uslub>
ul {
   ro'yxat uslubi turi: yo'q;
   chegara: 0;
   to'ldirish: 0;
}
</style>
</head>
<tana>

<p>Ushbu misolda biz roʻyxatdagi oʻqlarni, uning birlamchi toʻldirish va chetini olib tashlaymiz.</p>

<ul>
   <li><a href="#home">Uy</a></li>
   <li><a href="#news">Yangiliklar</a></li>
   <li><a href="#contact">Aloqa</a></li>
   <li><a href="#about">Haqida</a></li>
</ul>

</body>
</html>


Eslatma: Yuqoridagi misolda:

ro'yxat uslubi turi: yo'q; - O'qlarni olib tashlaydi. Navigatsiya paneli ro'yxat belgilariga muhtoj emas
  
Belgilangan chegara: 0; va to'ldirish: 0; brauzerning standart sozlamalarini o'chirish uchun

Yuqorida ishlatilgan kod vertikal va gorizontal navigatsiya panellarida ishlatiladigan standart koddir.



CSS vertikal navigatsiya paneli::


Vertikal navigatsiya paneli:

Vertikal navbat satrini yaratish uchun siz tushuntirilgan kodga qo'shimcha ravishda ro'yxat ichidagi <a> elementlarini uslublashingiz mumkin

yuqorida. :


<head>
<uslub>
ul {
   ro'yxat uslubi turi: yo'q;
   chegara: 0;
   to'ldirish: 0;
}

li a {
   displey: blok;
   kengligi: 60px;
   fon rangi: #dddddd;
}
</style>
</head>
<tana>

<ul>
   <li><a href="#home">Uy</a></li>
   <li><a href="#news">Yangiliklar</a></li>
   <li><a href="#contact">Aloqa</a></li>
   <li><a href="#about">Haqida</a></li>
</ul>

<p>Havola maydonini ko'rsatish uchun havolalarga fon rangi qo'shiladi.</p>
<p>E'tibor bering, faqat matnni emas, balki butun havola maydonini bosish mumkin.</p>

</body>
</html>


Yuqoridagi misolda:

displey: blok; - Havolani blok elementlari sifatida ko'rsatish butun havola maydonini bosish imkoniyatini beradi (nafaqat

matn) va u bizga kenglikni (va agar xohlasangiz, to'ldirish, chekka, balandlik va h.k.) belgilash imkonini beradi.
    
kengligi: 60px; - Blok elementlari sukut bo'yicha mavjud bo'lgan to'liq kenglikni egallaydi. Biz 60 pikselni belgilamoqchimiz

kengligi


Shuningdek, siz <ul> kengligini belgilashingiz va <a> kengligini olib tashlashingiz mumkin, chunki ular butun kenglikni egallaydi.

blok elementlari sifatida ko'rsatilganda mavjud. Bu avvalgi misolimiz bilan bir xil natija beradi:


<!DOCTYPE html>
<html>
<head>
<uslub>
ul {
   ro'yxat uslubi turi: yo'q;
   chegara: 0;
   to'ldirish: 0;
   kengligi: 60px;
}

li a {
   displey: blok;
   fon rangi: #dddddd;
}
</style>
</head>
<tana>

<ul>
   <li><a href="#home">Uy</a></li>
   <li><a href="#news">Yangiliklar</a></li>
   <li><a href="#contact">Aloqa</a></li>
   <li><a href="#about">Haqida</a></li>
</ul>

<p>Havola maydonini ko'rsatish uchun havolalarga fon rangi qo'shiladi.</p>
<p>E'tibor bering, faqat matnni emas, balki butun havola maydonini bosish mumkin.</p>

</body>
</html>


Vertikal navigatsiya paneliga misollar:::


Kulrang fon rangi bilan asosiy vertikal navigatsiya panelini olish va fon rangini o'zgartirish uchun

foydalanuvchi sichqonchani ularning ustiga siljitganda havolalar:

<!DOCTYPE html>
<html>
<head>
<uslub>
ul {
   ro'yxat uslubi turi: yo'q;
   chegara: 0;
   to'ldirish: 0;
   kengligi: 200px;
   fon rangi: #f1f1f1;
}

li a {
   displey: blok;
   rang: #000;
   to'ldirish: 8px 16px;
   matn-bezak: yo'q;
}

/* kursor ustidagi havola rangini o'zgartiring */
li a: suring {
   fon rangi: #555;
   rang: oq;
}
</style>
</head>
<tana>

<h2>Vertikal navigatsiya paneli</h2>

<ul>
   <li><a href="#home">Uy</a></li>
   <li><a href="#news">Yangiliklar</a></li>
   <li><a href="#contact">Aloqa</a></li>
   <li><a href="#about">Haqida</a></li>
</ul>

</body>
</html>

Active/Current Navigation Link:::

Add an "active" class to the current link to let the user know which page he/she is on:

<!DOCTYPE html>
<html>
<head>
<style>
ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  width: 200px;
  background-color: #f1f1f1;
}

li a {
  display: block;
  color: #000;
  padding: 8px 16px;
  text-decoration: none;
}

li a.active {
  background-color: #04AA6D;
  color: white;
}

li a:hover:not(.active) {
  background-color: #555;
  color: white;
}
</style>
</head>
<body>

<h2>Vertical Navigation Bar</h2>
<p>In this example, we create an "active" class with a green background color and a white text. The class is 

added to the "Home" link.</p>

<ul>
  <li><a class="active" href="#home">Home</a></li>
  <li><a href="#news">News</a></li>
  <li><a href="#contact">Contact</a></li>
  <li><a href="#about">About</a></li>
</ul>

</body>
</html>



Center Links & Add Borders


Adding text-align: center to <li> or <a> centers the links. To add border around the navbar, add border 

property to <ul>. To add borders inside the navbar, add border-bottom to all <li> elements except for the 

last one. See illustration below:


<!DOCTYPE html>
<html>
<head>
<style>
ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  width: 200px;
  background-color: #f1f1f1;
  border: 1px solid #555;
}

li a {
  display: block;
  color: #000;
  padding: 8px 16px;
  text-decoration: none;
}

li {
  text-align: center;
  border-bottom: 1px solid #555;
}

li:last-child {
  border-bottom: none;
}

li a.active {
  background-color: #04AA6D;
  color: white;
}

li a:hover:not(.active) {
  background-color: #555;
  color: white;
}
</style>
</head>
<body>

<h2>Vertical Navigation Bar</h2>
<p>In this example, we center the navigation links and add a border to the navigation bar.</p>

<ul>
  <li><a class="active" href="#home">Home</a></li>
  <li><a href="#news">News</a></li>
  <li><a href="#contact">Contact</a></li>
  <li><a href="#about">About</a></li>
</ul>

</body>
</html>



Toʻliq balandlikdagi Ruxsat etilgan vertikal Navbar :::

Toʻliq balandlikdagi yopishqoq yon navigatsiya yaratish uchun quyidagi kodni qoʻllang (u mobil qurilmada toʻgʻri ishlamasligi mumkin).

qurilmalar):

<!DOCTYPE html>
<html>
<head>
<uslub>
tana {
   chegara: 0;
}

ul {
   ro'yxat uslubi turi: yo'q;
   chegara: 0;
   to'ldirish: 0;
   kengligi: 25%;
   fon rangi: #f1f1f1;
   pozitsiyasi: qattiq;
   balandligi: 100%;
   toshib ketish: avtomatik;
}

li a {
   displey: blok;
   rang: #000;
   to'ldirish: 8px 16px;
   matn-bezak: yo'q;
}

li a.faol {
   fon rangi: #04AA6D;
   rang: oq;
}

li a:hover:not(.active) {
   fon rangi: #555;
   rang: oq;
}
</style>
</head>
<tana>

<ul>
   <li><a class="active" href="#home">Uy</a></li>
   <li><a href="#news">Yangiliklar</a></li>
   <li><a href="#contact">Aloqa</a></li>
   <li><a href="#about">Haqida</a></li>
</ul>

<div style="margin-left:25%;padding:1px 16px;height:1000px;">
   <h2>Toʻliq balandlikda oʻrnatilgan Yon Navigatsiya</h2>
   <h3>Ushbu hududni aylantirib ko'ring va sidenav sahifaga qanday yopishganini ko'ring</h3>
   <p>E'tibor bering, ushbu div elementi chap chekkasi 25%. Buning sababi, yon navigatsiya o'rnatilgan

25% kengligi. Agar siz chetni olib tashlasangiz, sidenav bu boʻlimning ustiga qoʻyadi/oʻtiradi.</p>
   <p>Shuningdek, biz overflow:auto-ni sidenav-ga o'rnatganimizga e'tibor bering. Bu sidenav bo'lganda aylantirish paneli qo'shadi

juda uzun (masalan, uning ichida 50 dan ortiq havola bo'lsa).</p>
   <p>Ba'zi matn..</p>
   <p>Ba'zi matn..</p>
   <p>Ba'zi matn..</p>
   <p>Ba'zi matn..</p>
   <p>Ba'zi matn..</p>
   <p>Ba'zi matn..</p>
   <p>Ba'zi matn..</p>
</div>

</body>
</html>




CSS gorizontal navigatsiya paneli::

Inline yoki suzuvchi ro'yxat elementlaridan foydalanib, gorizontal navigatsiya panelini yaratishingiz mumkin.


Inline ro'yxat elementlari

Yuqorida tavsiflangan standart kodga qo'shimcha ravishda siz <li> elementlarni qurish uchun inline sifatida belgilashingiz mumkin

gorizontal navigatsiya paneli. <li> elementlari sukut bo'yicha blok elementlari bo'lgani uchun ularni displey bilan uslublash:

mos ravishda; Roʻyxatning har bir elementidan oldingi va keyingi qatorlarni bir qatorda koʻrsatish uchun ularni olib tashlaydi. Qarang

quyidagi rasm:


<!DOCTYPE html>
<html>
<head>
<uslub>
ul {
   ro'yxat uslubi turi: yo'q;
   chegara: 0;
   to'ldirish: 0;
}

li {
   displey: inline;
}
</style>
</head>
<tana>

<ul>
   <li><a href="#home">Uy</a></li>
   <li><a href="#news">Yangiliklar</a></li>
   <li><a href="#contact">Aloqa</a></li>
   <li><a href="#about">Haqida</a></li>
</ul>

</body>
</html>





Suzuvchi roʻyxat elementlari:::

<li> elementlarini chapga surib, navigatsiya havolasi tartibini belgilash gorizontal hosil qiladi.

navigatsiya paneli. Overflow: yashirin; <ul> elementiga qo'shilganda <li> elementlarning tashqariga chiqishini oldini oladi

ro'yxati. Quyidagi rasmga qarang:

<!DOCTYPE html>
<html>
<head>
<uslub>
ul {
   ro'yxat uslubi turi: yo'q;
   chegara: 0;
   to'ldirish: 0;
   toshib ketish: yashirin;
}

li {
   float: chap;
}

li a {
   displey: blok;
   to'ldirish: 8px;
   fon rangi: #dddddd;
}
</style>
</head>
<tana>

<ul>
   <li><a href="#home">Uy</a></li>
   <li><a href="#news">Yangiliklar</a></li>
   <li><a href="#contact">Aloqa</a></li>
   <li><a href="#about">Haqida</a></li>
</ul>

<p><b>Eslatma:</b> Agar !DOCTYPE belgilanmagan bo'lsa, suzuvchi elementlar kutilmagan natijalar berishi mumkin.</p>
<p>Havola maydonini ko'rsatish uchun havolalarga fon rangi qo'shiladi. Butun havola maydonini bosish mumkin, emas

faqat matn.</p>
<p><b>Eslatma:</b> overflow:hidden ul elementiga li elementlarning tashqariga chiqishini oldini olish uchun qo'shiladi.

roʻyxati.</p>

</body>
</html>


Yuqoridagi misolda float:left; bir-birining yonida suzuvchi blok elementlarini olish uchun floatdan foydalanadi.
displey: blok; bizga to'ldirishni belgilash imkonini beradi (va agar xohlasangiz, balandlik, kenglik, chekka va hokazo)
     to'ldirish: 8px; - Har bir <a> elementi o'rtasida yaxshi ko'rinishga ega bo'lish uchun biroz to'ldirishni belgilang
     fon rangi: #dddddd; - Har bir <a> elementiga kulrang fon rangi qo'shing


Maslahat: Toʻliq kenglikdagi fon rangini istasangiz, har bir <a> elementi oʻrniga <ul> ga fon rangini qoʻshing:


<!DOCTYPE html>
<html>
<head>
<uslub>
ul {
   ro'yxat uslubi turi: yo'q;
   chegara: 0;
   to'ldirish: 0;
   toshib ketish: yashirin;
   fon rangi: #dddddd;
}

li {
   float: chap;
}

li a {
   displey: blok;
   to'ldirish: 8px;
}
</style>
</head>
<tana>

<ul>
   <li><a href="#home">Uy</a></li>
   <li><a href="#news">Yangiliklar</a></li>
   <li><a href="#contact">Aloqa</a></li>
   <li><a href="#about">Haqida</a></li>
</ul>

<p>Toʻliq kenglikdagi fon rangini yaratish uchun har bir havola oʻrniga roʻyxatga fon rangi qoʻshiladi.</p>
<p><b>Eslatma:</b> overflow:hidden ul elementiga li elementlarning tashqariga chiqishini oldini olish uchun qo'shiladi.

roʻyxati.</p>

</body>
</html>




Gorizontal navigatsiya paneliga misollar

Qorong'i fon rangi bilan asosiy gorizontal navigatsiya panelini yaratish va fon rangini o'zgartirish uchun

foydalanuvchi sichqonchani ularning ustiga siljitganda havolalar:


<!DOCTYPE html>
<html>
<head>
<uslub>
ul {
   ro'yxat uslubi turi: yo'q;
   chegara: 0;
   to'ldirish: 0;
   toshib ketish: yashirin;
   fon rangi: #333;
}

li {
   float: chap;
}

li a {
   displey: blok;
   rang: oq;
   matnni tekislash: markaz;
   to'ldirish: 14px 16px;
   matn-bezak: yo'q;
}

li a: suring {
   fon rangi: #111;
}
</style>
</head>
<tana>

<ul>
   <li><a class="active" href="#home">Uy</a></li>
   <li><a href="#news">Yangiliklar</a></li>
   <li><a href="#contact">Aloqa</a></li>
   <li><a href="#about">Haqida</a></li>
</ul>

</body>
</html>



Faol/joriy navigatsiya havolasi

Joriy havolaga “faol” sinf qo‘shing va foydalanuvchi qaysi sahifada ekanligini bilishi mumkin:


<!DOCTYPE html>
<html>
<head>
<uslub>
ul {
   ro'yxat uslubi turi: yo'q;
   chegara: 0;
   to'ldirish: 0;
   toshib ketish: yashirin;
   fon rangi: #333;
}

li {
   float: chap;
}

li a {
   displey: blok;
   rang: oq;
   matnni tekislash: markaz;
   to'ldirish: 14px 16px;
   matn-bezak: yo'q;
}

li a:hover:not(.active) {
   fon rangi: #111;
}

.faol {
   fon rangi: #04AA6D;
}
</style>
</head>
<tana>

<ul>
   <li><a class="active" href="#home">Uy</a></li>
   <li><a href="#news">Yangiliklar</a></li>
   <li><a href="#contact">Aloqa</a></li>
   <li><a href="#about">Haqida</a></li>
</ul>

</body>
</html>



O'ngga tekislash havolalari

Roʻyxat elementlarini oʻngga surish orqali havolalarni oʻngga tekislang (float:right;):

<!DOCTYPE html>
<html>
<head>
<uslub>
ul {
   ro'yxat uslubi turi: yo'q;
   chegara: 0;
   to'ldirish: 0;
   toshib ketish: yashirin;
   fon rangi: #333;
}

li {
   float: chap;
}

li a {
   displey: blok;
   rang: oq;
   matnni tekislash: markaz;
   to'ldirish: 14px 16px;
   matn-bezak: yo'q;
}

li a:hover:not(.active) {
   fon rangi: #111;
}

.faol {
   fon rangi: #04AA6D;
}
</style>
</head>
<tana>

<ul>
   <li><a href="#home">Uy</a></li>
   <li><a href="#news">Yangiliklar</a></li>
   <li><a href="#contact">Aloqa</a></li>
   <li style="float:right"><a class="active" href="#about">Haqida</a></li>
</ul>

</body>
</html>



Chegara bo'linuvchilari

Havola ajratgichlarini yaratish uchun chegara huquqi xususiyatini <li> ga qo'shing:


<!DOCTYPE html>
<html>
<head>
<uslub>
ul {
   ro'yxat uslubi turi: yo'q;
   chegara: 0;
   to'ldirish: 0;
   toshib ketish: yashirin;
   fon rangi: #333;
}

li {
   float: chap;
   chegara o'ng: 1px qattiq #bbb;
}

li: oxirgi bola {
   chegara o'ng: yo'q;
}

li a {
   displey: blok;
   rang: oq;
   matnni tekislash: markaz;
   to'ldirish: 14px 16px;
   matn-bezak: yo'q;
}

li a:hover:not(.active) {
   fon rangi: #111;
}

.faol {
   fon rangi: #04AA6D;
}
</style>
</head>
<tana>

<ul>
   <li><a class="active" href="#home">Uy</a></li>
   <li><a href="#news">Yangiliklar</a></li>
   <li><a href="#contact">Aloqa</a></li>
   <li style="float:right"><a href="#about">Haqida</a></li>
</ul>

</body>
</html>

Ruxsat etilgan navigatsiya paneli

Foydalanuvchi sahifani aylantirganda ham navigatsiya paneli sahifaning yuqori yoki pastki qismida qolsin:



Ruxsat etilgan yuqori navbat paneli:

<!DOCTYPE html>
<html>
<head>
<uslub>
tana (chegara: 0;}

ul {
   ro'yxat uslubi turi: yo'q;
   chegara: 0;
   to'ldirish: 0;
   toshib ketish: yashirin;
   fon rangi: #333;
   pozitsiyasi: qattiq;
   yuqori: 0;
   kengligi: 100%;
}

li {
   float: chap;
}

li a {
   displey: blok;
   rang: oq;
   matnni tekislash: markaz;
   to'ldirish: 14px 16px;
   matn-bezak: yo'q;
}

li a:hover:not(.active) {
   fon rangi: #111;
}

.faol {
   fon rangi: #04AA6D;
}
</style>
</head>
<tana>

<ul>
   <li><a class="active" href="#home">Uy</a></li>
   <li><a href="#news">Yangiliklar</a></li>
   <li><a href="#contact">Aloqa</a></li>
   <li><a href="#about">Haqida</a></li>
</ul>

<div style="padding:20px;margin-top:30px;background-color:#1abc9c;height:1500px;">
   <h1>Ruxsat etilgan yuqori navigatsiya paneli</h1>
   <h2>Effektni ko'rish uchun ushbu sahifani aylantiring</h2>
   <h2>O'tish paytida navigatsiya paneli sahifaning yuqori qismida qoladi</h2>

   <p>Ba'zi matnlar ba'zi matnlar, ba'zilari matnlar...</p>
   <p>Ba'zi matnlar ba'zi matnlar, ba'zilari matnlar...</p>
   <p>Ba'zi matnlar ba'zi matnlar, ba'zilari matnlar...</p>
   <p>Ba'zi matnlar ba'zi matnlar, ba'zilari matnlar...</p>
   <p>Ba'zi matnlar ba'zi matnlar, ba'zilari matnlar...</p>
   <p>Ba'zi matnlar ba'zi matnlar, ba'zilari matnlar...</p>
   <p>Ba'zi matnlar ba'zi matnlar, ba'zilari matnlar...</p>
   <p>Ba'zi matnlar ba'zi matnlar, ba'zilari matnlar...</p>
   <p>Ba'zi matnlar ba'zi matnlar, ba'zilari matnlar...</p>
   <p>Ba'zi matnlar ba'zi matnlar, ba'zilari matnlar...</p>
   <p>Ba'zi matnlar ba'zi matnlar, ba'zilari matnlar...</p>
   <p>Ba'zi matnlar ba'zi matnlar, ba'zilari matnlar...</p>
   <p>Ba'zi matnlar ba'zi matnlar, ba'zilari matnlar...</p>
   <p>Ba'zi matnlar ba'zi matnlar, ba'zilari matnlar...</p>
   <p>Ba'zi matnlar ba'zi matnlar, ba'zilari matnlar...</p>
   <p>Ba'zi matnlar ba'zi matnlar, ba'zilari matnlar...</p>
   <p>Ba'zi matnlar ba'zi matnlar, ba'zilari matnlar...</p>
   <p>Ba'zi matnlar ba'zi matnlar, ba'zilari matnlar...</p>
   <p>Ba'zi matnlar ba'zi matnlar, ba'zilari matnlar...</p>
   <p>Ba'zi matnlar ba'zi matnlar, ba'zilari matnlar...</p>
</div>

</body>
</html>



Ruxsat etilgan pastki navigatsiya paneli:

<!DOCTYPE html>
<html>
<head>
<uslub>
tana (chegara: 0;}

ul {
   ro'yxat uslubi turi: yo'q;
   chegara: 0;
   to'ldirish: 0;
   toshib ketish: yashirin;
   fon rangi: #333;
   pozitsiyasi: qattiq;
   pastki: 0;
   kengligi: 100%;
}

li {
   float: chap;
}

li a {
   displey: blok;
   rang: oq;
   matnni tekislash: markaz;
   to'ldirish: 14px 16px;
   matn-bezak: yo'q;
}

li a:hover:not(.active) {
   fon rangi: #111;
}

.faol {
   fon rangi: #04AA6D;
}
</style>
</head>
<tana>

<ul>
   <li><a class="active" href="#home">Uy</a></li>
   <li><a href="#news">Yangiliklar</a></li>
   <li><a href="#contact">Aloqa</a></li>
   <li><a href="#about">Haqida</a></li>
</ul>

<div style="padding:20px;background-color:#1abc9c;height:1500px;">
   <h1> Ruxsat etilgan pastki navigatsiya paneli</h1>
   <h2>Effektni ko'rish uchun ushbu sahifani aylantiring</h2>
   <h2>O'tish paytida navigatsiya paneli sahifaning pastki qismida qoladi</h2>

   <p>Ba'zi matnlar ba'zi matnlar, ba'zilari matnlar...</p>
   <p>Ba'zi matnlar ba'zi matnlar, ba'zilari matnlar...</p>
   <p>Ba'zi matnlar ba'zi matnlar, ba'zilari matnlar...</p>
   <p>Ba'zi matnlar ba'zi matnlar, ba'zilari matnlar...</p>
   <p>Ba'zi matnlar ba'zi matnlar, ba'zilari matnlar...</p>
   <p>Ba'zi matnlar ba'zi matnlar, ba'zilari matnlar...</p>
   <p>Ba'zi matnlar ba'zi matnlar, ba'zilari matnlar...</p>
   <p>Ba'zi matnlar ba'zi matnlar, ba'zilari matnlar...</p>
   <p>Ba'zi matnlar ba'zi matnlar, ba'zilari matnlar...</p>
   <p>Ba'zi matnlar ba'zi matnlar, ba'zilari matnlar...</p>
   <p>Ba'zi matnlar ba'zi matnlar, ba'zilari matnlar...</p>
   <p>Ba'zi matnlar ba'zi matnlar, ba'zilari matnlar...</p>
   <p>Ba'zi matnlar ba'zi matnlar, ba'zilari matnlar...</p>
   <p>Ba'zi matnlar ba'zi matnlar, ba'zilari matnlar...</p>
   <p>Ba'zi matnlar ba'zi matnlar, ba'zilari matnlar...</p>
   <p>Ba'zi matnlar ba'zi matnlar, ba'zilari matnlar...</p>
   <p>Ba'zi matnlar ba'zi matnlar, ba'zilari matnlar...</p>
   <p>Ba'zi matnlar ba'zi matnlar, ba'zilari matnlar...</p>
   <p>Ba'zi matnlar ba'zi matnlar, ba'zilari matnlar...</p>
   <p>Ba'zi matnlar ba'zi matnlar, ba'zilari matnlar...</p>
</div>

</body>
</html>


Kulrang gorizontal Navbar

Yupqa kulrang hoshiyali kulrang gorizontal chiziq quyida ko'rsatilganidek yaratilgan:

<!DOCTYPE html>
<html>
<head>
<uslub>
ul {
   ro'yxat uslubi turi: yo'q;
   chegara: 0;
   to'ldirish: 0;
   toshib ketish: yashirin;
   chegara: 1px qattiq #e7e7e7;
   fon rangi: #f3f3f3;
}

li {
   float: chap;
}

li a {
   displey: blok;
   rang: #666;
   matnni tekislash: markaz;
   to'ldirish: 14px 16px;
   matn-bezak: yo'q;
}

li a:hover:not(.active) {
   fon rangi: #ddd;
}

li a.faol {
   rang: oq;
   fon rangi: #04AA6D;
}
</style>
</head>
<tana>

<ul>
   <li><a class="active" href="#home">Uy</a></li>
   <li><a href="#news">Yangiliklar</a></li>
   <li><a href="#contact">Aloqa</a></li>
   <li><a href="#about">Haqida</a></li>
</ul>

</body>
</html>


<!DOCTYPE html>
<html>
<head>
<uslub>
ul {
   ro'yxat uslubi turi: yo'q;
   chegara: 0;
   to'ldirish: 0;
   toshib ketish: yashirin;
   chegara: 1px qattiq #e7e7e7;
   fon rangi: #f3f3f3;
}

li {
   float: chap;
}

li a {
   displey: blok;
   rang: #666;
   matnni tekislash: markaz;
   to'ldirish: 14px 16px;
   matn-bezak: yo'q;
}

li a:hover:not(.active) {
   fon rangi: #ddd;
}

li a.faol {
   rang: oq;
   fon rangi: #04AA6D;
}
</style>
</head>
<tana>

<ul>
   <li><a class="active" href="#home">Uy</a></li>
   <li><a href="#news">Yangiliklar</a></li>
   <li><a href="#contact">Aloqa</a></li>
   <li><a href="#about">Haqida</a></li>
</ul>

</body>
</html>



Yopishqoq Navbar

Lavozim qo'shing: yopishqoq; yopishqoq navbar yaratish uchun <ul> ga.

Yopishqoq element aylantirish holatiga qarab nisbiy va qattiq o'rtasida almashinadi. U joylashtirilgan

ko'rish oynasida ma'lum bir ofset pozitsiyasi bajarilmaguncha nisbiy - keyin u joyida "yopishadi" (masalan

pozitsiyasi: belgilangan). E'tibor bering, Internet Explorer yopishqoq joylashuvni qo'llab-quvvatlamaydi. Safari uchun -webkit- kerak

prefiks (yuqoridagi misolga qarang). Yopishqoqlik uchun yuqori, o'ng, pastki yoki chapdan kamida bittasini belgilashingiz kerak

ishlash uchun joylashishni aniqlash. Yopishqoq l ning yaratilishi tasviriga qarang


<!DOCTYPE html>
<html>
<head>
<uslub>
tana {
   shrift o'lchami: 28px;
}

ul {
   ro'yxat uslubi turi: yo'q;
   chegara: 0;
   to'ldirish: 0;
   toshib ketish: yashirin;
   fon rangi: #333;
   pozitsiyasi: -webkit-yopishqoq; /* Safari */
   pozitsiyasi: yopishqoq;
   yuqori: 0;
}

li {
   float: chap;
}

li a {
   displey: blok;
   rang: oq;
   matnni tekislash: markaz;
   to'ldirish: 14px 16px;
   matn-bezak: yo'q;
}

li a: suring {
   fon rangi: #111;
}

.faol {
   fon rangi: #4CAF50;
}
</style>
</head>
<tana>

<div class="header">
   <h2>Pastga aylantiring</h2>
   <p>Yopishqoq effektni ko‘rish uchun pastga aylantiring.</p>
</div>

<ul>
   <li><a class="active" href="#home">Uy</a></li>
   <li><a href="#news">Yangiliklar</a></li>
   <li><a href="#contact">Aloqa</a></li>
</ul>

<h3>Yopishqoq navigatsiya paneliga misol</h3>
<p>O'tish joyiga yetganingizda, navigatsiya paneli tepaga <strong>yopishadi</strong>.</p>
<p><strong>Eslatma:</strong> Internet Explorer yopishqoq joylashuvni qo'llab-quvvatlamaydi va Safari -webkit-ni talab qiladi.

prefiks.</p>
<p>O'tkazishni yoqish uchun bir nechta matn. Lorem ipsum dolor sit amet, illum definitiones no quo, maluisset

concludaturque et eum, altera fabulas ut quo. Atqui causae gloriatur ius te, id agam omnis evertitur eum.

Affert laboramus repudiandae nec et. Inciderint uning reklamasi samarali. Eum no molestiae voluptatibus.</p>
<p>O'tkazishni yoqish uchun bir nechta matn. Lorem ipsum dolor sit amet, illum definitiones no quo, maluisset

concludaturque et eum, altera fabulas ut quo. Atqui causae gloriatur ius te, id agam omnis evertitur eum.

Affert laboramus repudiandae nec et. Inciderint uning reklamasi samarali. Eum no molestiae voluptatibus.</p><p>Some text to enable scrolling. Lorem ipsum dolor sit amet, illum definitiones no quo, maluisset 

concludaturque et eum, altera fabulas ut quo. Atqui causae gloriatur ius te, id agam omnis evertitur eum. 

Affert laboramus repudiandae nec et. Inciderint efficiantur his ad. Eum no molestiae voluptatibus.</p>
<p>Some text to enable scrolling. Lorem ipsum dolor sit amet, illum definitiones no quo, maluisset 

concludaturque et eum, altera fabulas ut quo. Atqui causae gloriatur ius te, id agam omnis evertitur eum. 

Affert laboramus repudiandae nec et. Inciderint efficiantur his ad. Eum no molestiae voluptatibus.</p>
<p>Some text to enable scrolling. Lorem ipsum dolor sit amet, illum definitiones no quo, maluisset 

concludaturque et eum, altera fabulas ut quo. Atqui causae gloriatur ius te, id agam omnis evertitur eum. 

Affert laboramus repudiandae nec et. Inciderint efficiantur his ad. Eum no molestiae voluptatibus.</p>
<p>Some text to enable scrolling. Lorem ipsum dolor sit amet, illum definitiones no quo, maluisset 

concludaturque et eum, altera fabulas ut quo. Atqui causae gloriatur ius te, id agam omnis evertitur eum. 

Affert laboramus repudiandae nec et. Inciderint efficiantur his ad. Eum no molestiae voluptatibus.</p>
<p>Some text to enable scrolling. Lorem ipsum dolor sit amet, illum definitiones no quo, maluisset 

concludaturque et eum, altera fabulas ut quo. Atqui causae gloriatur ius te, id agam omnis evertitur eum. 

Affert laboramus repudiandae nec et. Inciderint efficiantur his ad. Eum no molestiae voluptatibus.</p>

</body>
</html>




Responsive Topnav

How to use CSS media queries to create a responsive top navigation is shown below:



<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<style>
body {margin: 0;}

ul.topnav {
  list-style-type: none;
  margin: 0;
  padding: 0;
  overflow: hidden;
  background-color: #333;
}

ul.topnav li {float: left;}

ul.topnav li a {
  display: block;
  color: white;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
}

ul.topnav li a:hover:not(.active) {background-color: #111;}

ul.topnav li a.active {background-color: #04AA6D;}

ul.topnav li.right {float: right;}

@media screen and (max-width: 600px) {
  ul.topnav li.right, 
  ul.topnav li {float: none;}
}
</style>
</head>
<body>

<ul class="topnav">
  <li><a class="active" href="#home">Home</a></li>
  <li><a href="#news">News</a></li>
  <li><a href="#contact">Contact</a></li>
  <li class="right"><a href="#about">About</a></li>
</ul>

<div style="padding:0 16px;">
  <h2>Responsive Topnav Example</h2>
  <p>This example use media queries to stack the topnav vertically when the screen size is 600px or 

less.</p>
  <p>You will learn more about media queries and responsive web design later in our CSS Tutorial.</p>
  <h4>Resize the browser window to see the effect.</h4>
</div>

</body>
</html>




Javob beruvchi Sidenav

Javob beruvchi yon navigatsiyani yaratish uchun CSS media so'rovlaridan qanday foydalanish kerak.


<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<uslub>
tana (chegara: 0;}

ul.sidenav {
   ro'yxat uslubi turi: yo'q;
   chegara: 0;
   to'ldirish: 0;
   kengligi: 25%;
   fon rangi: #f1f1f1;
   pozitsiyasi: qattiq;
   balandligi: 100%;
   toshib ketish: avtomatik;
}

ul.sidenav li a {
   displey: blok;
   rang: #000;
   to'ldirish: 8px 16px;
   matn-bezak: yo'q;
}
 
ul.sidenav li a.faol {
   fon rangi: #4CAF50;
   rang: oq;
}

ul.sidenav li a:hover:not(.active) {
   fon rangi: #555;
   rang: oq;
}

div.content {
   chap chekka: 25%;
   to'ldirish: 1px 16px;
   balandligi: 1000px;
}

@media ekrani va (maksimal kenglik: 900px) {
   ul.sidenav {
     kengligi: 100%;
     balandligi: avtomatik;
     pozitsiya: nisbiy;
   }
  
   ul.sidenav li a {
     float: chap;
     to'ldirish: 15px;
   }
  
   div.content {chap cheti: 0;}
}

@media ekrani va (maksimal kenglik: 400px) {
   ul.sidenav li a {
     matnni tekislash: markaz;
     float: yo'q;
   }
}
</style>
</head>
<tana>

<ul class="sidenav">
   <li><a class="active" href="#home">Uy</a></li>
   <li><a href="#news">Yangiliklar</a></li>
   <li><a href="#contact">Aloqa</a></li>
   <li><a href="#about">Haqida</a></li>
</ul>

<div class="content">
   <h2>Javob beruvchi Sidenav misoli</h2>
   <p>Bu misolda ekran oʻlchami katta boʻlganda sidenavni yuqori navigatsiya paneliga aylantirish uchun media soʻrovlaridan foydalaniladi.

900px yoki undan kamroq.</p>
   <p>Shuningdek, biz 400px yoki undan kichik ekranlar uchun media soʻrovni qoʻshdik, ular vertikal ravishda joylashadi va

navigatsiya havolalarini markazlashtiring.</p>
   <p>Media so'rovlari va sezgir veb-dizayn haqida batafsil ma'lumotni keyinroq CSS qo'llanmamizdan bilib olasiz.</p>
   <h3>Effektni ko'rish uchun brauzer oynasining o'lchamini o'zgartiring.</h3>
</div>

</body>
</html>




Ochiladigan Navbar

Navigatsiya paneliga ochiladigan menyuni qanday qo'shish mumkin.


<!DOCTYPE html>
<html>
<head>
<uslub>
ul {
   ro'yxat uslubi turi: yo'q;
   chegara: 0;
   to'ldirish: 0;
   toshib ketish: yashirin;
   fon rangi: #333;
}

li {
   float: chap;
}

li a, .dropbtn {
   displey: inline-block;
   rang: oq;
   matnni tekislash: markaz;
   to'ldirish: 14px 16px;
   matn-bezak: yo'q;
}

li a:hover, .dropdown:hover .dropbtn {
   fon rangi: qizil;
}

li.ochiladigan pastga {
   displey: inline-block;
}

.ochiladigan tarkib {
   ko'rsatish: yo'q;
   pozitsiyasi: mutlaq;
   fon rangi: #f9f9f9;
   min-kengligi: 160px;
   quti soyasi: 0px 8px 16px 0px rgba(0,0,0,0.2);
   z-indeks: 1;
}

.dropdown-content a {
   rang: qora;
   to'ldirish: 12px 16px;
   matn-bezak: yo'q;
   displey: blok;
   matnni tekislash: chapga;
}

.ochiladigan tarkib a: hover {fon rangi: #f1f1f1;}

.dropdown: hover .dropdown-content {
   displey: blok;
}
</style>
</head>
<tana>

<ul>
   <li><a href="#home">Uy</a></li>
   <li><a href="#news">Yangiliklar</a></li>
   <li class="ochiladigan">
     <a href="javascript:void(0)" class="dropbtn">Ochiladigan menyu</a>
     <div class="dropdown-content">
       <a href="#">1-havola</a>
       <a href="#">2-havola</a>
       <a href="#">3-havola</a>
     </div>
   </li>
</ul>

<h3>Navigatsiya paneli ichidagi ochiladigan menyu</h3>
<p>Ochiladigan menyuni koʻrish uchun kursorni “Ochiladigan” havolasi ustiga olib boring.</p>

</body>
</html>

  
<kbd>qaytish</kbd>[Mundarijaga qaytish](#homepage)

--------


## CSS ochiladi

Ushbu bo'limda CSS yordamida ochiladigan ro'yxatni qanday qo'shish mumkinligi ko'rsatilgan:

Asosiy ochiladigan menyu:::
Quyida ko'rsatilganidek, foydalanuvchi sichqonchani element ustida harakatlantirganda paydo bo'ladigan ochiladigan oynani yarating:

<!DOCTYPE html>
<html>
<head>
<uslub>
.ochiladigan ro'yxat {
   pozitsiya: nisbiy;
   displey: inline-block;
}

.ochiladigan tarkib {
   ko'rsatish: yo'q;
   pozitsiyasi: mutlaq;
   fon rangi: #f9f9f9;
   min-kengligi: 160px;
   quti soyasi: 0px 8px 16px 0px rgba(0,0,0,0.2);
   to'ldirish: 12px 16px;
   z-indeks: 1;
}

.dropdown: hover .dropdown-content {
   displey: blok;
}
</style>
</head>
<tana>

<h2>Hoverable ochiladigan menyu</h2>
<p>Ochiladigan tarkibni ochish uchun sichqonchani quyidagi matn ustiga olib boring.</p>

<div class="ochiladigan">
   <span>Sichqoncha ustimda</span>
   <div class="dropdown-content">
   <p>Salom dunyo!</p>
   </div>
</div>

</body>
</html>


Yuqoridagi misolda:

HTML:

Ochiladigan menyuni ochish uchun <span> elementidan foydalaning. Siz <button> elementidan ham foydalanishingiz mumkin

Ochiladigan menyu tarkibini yaratish va qo'shmoqchi bo'lgan narsalarni qo'shish uchun <div> kabi konteyner elementidan foydalaning

uning ichida.

CSS bilan ochiladigan menyuni to'g'ri joylashtirish uchun <div> elementini elementlar atrofiga o'rang


css:

.dropdown klassi position:relative dan foydalanadi, bu biz ochiladigan tarkibni joylashtirishni xohlaganimizda kerak bo'ladi

ochiladigan tugmaning o'ng ostidagi (pozitsiyadan foydalanish: mutlaq).

.dropdown-content sinfi haqiqiy ochiladigan tarkibga ega. U sukut bo'yicha yashiringan va shunday bo'ladi

hoverda ko'rsatiladi (pastga qarang).

Eslatma: Bu erda biz min-kenglikni 160px ga o'rnatdik. Siz uni didingizga qarab o'zgartirishingiz mumkin.

Maslahat: Ochiladigan kontentning kengligi ochiladigan tugma kabi keng bo'lishi uchun kenglikni 100% ga o'rnating (va

toshib ketish:avto; kichik ekranlarda aylantirishni yoqish uchun)

Ochiladigan menyuni chegaraga emas, balki kartaga o'xshatish uchun biz CSS box-shadow xususiyatini emas, balki o'rnatdik

chegara.


:hover selektori foydalanuvchi sichqonchani ochiladigan menyu ustida harakatlantirganda ochiladigan menyuni ko'rsatish uchun ishlatiladi

tugmasi.



Ochiladigan menyu

Quyida ko'rsatilgandek, foydalanuvchiga ro'yxatdagi variantni tanlash imkonini beruvchi ochiladigan menyu yarating:

<!DOCTYPE html>
<html>
<head>
<uslub>
.dropbtn {
   fon rangi: #4CAF50;
   rang: oq;
   to'ldirish: 16px;
   shrift o'lchami: 16px;
   chegara: yo'q;
   kursor: ko'rsatgich;
}

.ochiladigan ro'yxat {
   pozitsiya: nisbiy;
   displey: inline-block;
}

.ochiladigan tarkib {
   ko'rsatish: yo'q;
   pozitsiyasi: mutlaq;
   fon rangi: #f9f9f9;
   min-kengligi: 160px;
   quti soyasi: 0px 8px 16px 0px rgba(0,0,0,0.2);
   z-indeks: 1;
}

.dropdown-content a {
   rang: qora;
   to'ldirish: 12px 16px;
   matn-bezak: yo'q;
   displey: blok;
}

.dropdown-content a: hover {fon rangi: #f1f1f1}

.dropdown: hover .dropdown-content {
   displey: blok;
}

.dropdown: hover .dropbtn {
   fon rangi: #3e8e41;
}
</style>
</head>
<tana>

<h2>Ochiladigan menyu</h2>
<p>Ochiladigan menyuni ochish uchun sichqonchani tugma ustiga olib boring.</p>

<div class="ochiladigan">
   <button class="dropbtn">ochiladigan pastga</button>
   <div class="dropdown-content">
   <a href="#">1-havola</a>
   <a href="#">2-havola</a>
   <a href="#">3-havola</a>
   </div>
</div>

<p><strong>Eslatma:</strong> Biz sinov havolalari uchun href="#" dan foydalanamiz. Haqiqiy veb-saytda bu URL manzillar bo'ladi.</p>

</body>
</html>





O'ng tomonga tekislangan ochiladigan tarkib


Ochiladigan menyuni chapdan o'ngga emas, o'ngdan chapga o'tkazish uchun o'ngga qo'shing: 0; ko'rsatilgandek uslubda

quyida:

<!DOCTYPE html>
<html>
<head>
<uslub>
.dropbtn {
   fon rangi: #4CAF50;
   rang: oq;
   to'ldirish: 16px;
   shrift o'lchami: 16px;
   chegara: yo'q;
   kursor: ko'rsatgich;
}

.ochiladigan ro'yxat {
   pozitsiya: nisbiy;
   displey: inline-block;
}

.ochiladigan tarkib {
   ko'rsatish: yo'q;
   pozitsiyasi: mutlaq;
   o'ng: 0;
   fon rangi: #f9f9f9;
   min-kengligi: 160px;
   quti soyasi: 0px 8px 16px 0px rgba(0,0,0,0.2);
   z-indeks: 1;
}

.dropdown-content a {
   rang: qora;
   to'ldirish: 12px 16px;
   matn-bezak: yo'q;
   displey: blok;
}

.ochiladigan tarkib a: hover {fon rangi: #f1f1f1;}

.dropdown: hover .dropdown-content {
   displey: blok;
}

.dropdown: hover .dropbtn {
   fon rangi: #3e8e41;
}
</style>
</head>
<tana>

<h2>Tezlangan ochiladigan tarkib</h2>
<p>Ochiladigan tarkib chapdan o'ngga yoki o'ngdan chapga chapga va chapga o'tishini aniqlang

to'g'ri xususiyatlar.</p>

<div class="dropdown" style="float:left;">
   <button class="dropbtn">Chapga</button>
   <div class="dropdown-content" style="left:0;">
   <a href="#">1-havola</a>
   <a href="#">2-havola</a>
   <a href="#">3-havola</a>
   </div>
</div>

<div class="dropdown" style="float:right;">
   <button class="dropbtn">O'ng</button>
   <div class="dropdown-content">
   <a href="#">1-havola</a>
   <a href="#">2-havola</a>
   <a href="#">3-havola</a>
   </div>
</div>

</body>
</html>


Ochiladigan rasm

Ochiladigan oynaga rasm va boshqa tarkibni qanday qo'shish mumkin.


<!DOCTYPE html>
<html>
<head>
<uslub>
.ochiladigan ro'yxat {
   pozitsiya: nisbiy;
   displey: inline-block;
}

.ochiladigan tarkib {
   ko'rsatish: yo'q;
   pozitsiyasi: mutlaq;
   fon rangi: #f9f9f9;
   min-kengligi: 160px;
   quti soyasi: 0px 8px 16px 0px rgba(0,0,0,0.2);
   z-indeks: 1;
}

.dropdown: hover .dropdown-content {
   displey: blok;
}

.desc {
   to'ldirish: 15px;
   matnni tekislash: markaz;
}
</style>
</head>
<tana>

<h2>Ochiladigan rasm</h2>
<p>Ochiladigan tarkibni ochish uchun sichqonchani quyidagi rasm ustiga olib boring.</p>

<div class="ochiladigan">
   <img src="img_5terre.jpg" alt="Cinque Terre" kengligi="100" balandligi="50">
   <div class="dropdown-content">
   <img src="img_5terre.jpg" alt="Cinque Terre" kengligi="300" balandligi="200">
   <div class="desc">Chiroyli Cinque Terre</div>
   </div>
</div>

</body>
</html>




Ochiladigan Navbar

Navigatsiya paneliga ochiladigan menyuni qanday qo'shish mumkin:


<!DOCTYPE html>
<html>
<head>
<uslub>
ul {
   ro'yxat uslubi turi: yo'q;
   chegara: 0;
   to'ldirish: 0;
   toshib ketish: yashirin;
   fon rangi: #333;
}

li {
   float: chap;
}

li a, .dropbtn {
   displey: inline-block;
   rang: oq;
   matnni tekislash: markaz;
   to'ldirish: 14px 16px;
   matn-bezak: yo'q;
}

li a:hover, .dropdown:hover .dropbtn {
   fon rangi: qizil;
}

li.ochiladigan pastga {
   displey: inline-block;
}

.ochiladigan tarkib {
   ko'rsatish: yo'q;
   pozitsiyasi: mutlaq;
   fon rangi: #f9f9f9;
   min-kengligi: 160px;
   quti soyasi: 0px 8px 16px 0px rgba(0,0,0,0.2);
   z-indeks: 1;
}

.dropdown-content a {
   rang: qora;
   to'ldirish: 12px 16px;
   matn-bezak: yo'q;
   displey: blok;
   matnni tekislash: chapga;
}

.ochiladigan tarkib a: hover {fon rangi: #f1f1f1;}

.dropdown: hover .dropdown-content {
   displey: blok;
}
</style>
</head>
<tana>

<ul>
   <li><a href="#home">Uy</a></li>
   <li><a href="#news">Yangiliklar</a></li>
   <li class="ochiladigan">
     <a href="javascript:void(0)" class="dropbtn">Ochiladigan menyu</a>
     <div class="dropdown-content">
       <a href="#">1-havola</a>
       <a href="#">2-havola</a>
       <a href="#">3-havola</a>
     </div>
   </li>
</ul>

<h3>Navigatsiya paneli ichidagi ochiladigan menyu</h3>
<p>Ochiladigan menyuni koʻrish uchun kursorni “Ochiladigan” havolasi ustiga olib boring.</p>

</body>
</html>


<kbd>qaytish</kbd>[Mundarijaga qaytish](#homepage)


--------


## CSS rasmlar galereyasi


Quyida tasvirlanganidek CSS yordamida rasm galereyasini yaratishingiz mumkin:

<!DOCTYPE html>
<html>
<head>
<uslub>
div.gallery {
   chegara: 5px;
   chegara: 1px qattiq #ccc;
   float: chap;
   kengligi: 180px;
}

div.gallery: hover {
   chegara: 1px qattiq #777;
}

div.gallery img {
   kengligi: 100%;
   balandligi: avtomatik;
}

div.desc {
   to'ldirish: 15px;
   matnni tekislash: markaz;
}
</style>
</head>
<tana>

<div class="galereya">
   <a target="_blank" href="img_5terre.jpg">
     <img src="img_5terre.jpg" alt="Cinque Terre" kengligi="600" balandligi="400">
   </a>
   <div class="desc">Rasm tavsifini shu yerga qo'shing</div>
</div>

<div class="galereya">
   <a target="_blank" href="img_forest.jpg">
     <img src="img_forest.jpg" alt="O'rmon" kengligi="600" balandligi="400">
   </a>
   <div class="desc">Rasm tavsifini shu yerga qo'shing</div>
</div>

<div class="gallery">
   <a target="_blank" href="img_lights.jpg">
     <img src="img_lights.jpg" alt="Shimoliy chiroqlar" kengligi="600" balandligi="400">
   </a>
   <div class="desc">Rasm tavsifini shu yerga qo'shing</div>
</div>

<div class="gallery">
   <a target="_blank" href="img_mountains.jpg">
     <img src="img_mountains.jpg" alt="Tog'lar" kengligi="600" balandligi="400">
   </a>
   <div class="desc">Rasm tavsifini shu yerga qo'shing</div>
</div>

</body>
</html>


Javob beruvchi tasvirlar galereyasi

Ish stollarida, planshetlarda yaxshi ko'rinadigan sezgir tasvirlar galereyasini yaratish uchun CSS media so'rovlaridan qanday foydalanish kerak

va aqlli telefonlar.


<!DOCTYPE html>
<html>
<head>
<uslub>
div.gallery {
   chegara: 1px qattiq #ccc;
}

div.gallery: hover {
   chegara: 1px qattiq #777;
}

div.gallery img {
   kengligi: 100%;
   balandligi: avtomatik;
}

div.desc {
   to'ldirish: 15px;
   matnni tekislash: markaz;
}

* {
   quti o'lchami: chegara qutisi;
}

.responsive {
   to'ldirish: 0 6px;
   float: chap;
   kengligi: 24,99999%;
}

@media faqat ekran va (maksimal kenglik: 700px) {
   .responsive {
     kengligi: 49,99999%;
     chegara: 6px 0;
   }
}

@media faqat ekran va (maksimal kenglik: 500px) {
   .responsive {
     kengligi: 100%;
   }
}

.clearfix:keyin {
   tarkib: "";
   ko'rsatish: jadval;
   aniq: ikkalasi ham;
}
</style>
</head>
<tana>

<h2>Responsive rasmlar galereyasi</h2>

<h4>Effektni ko'rish uchun brauzer oynasining o'lchamini o'zgartiring.</h4>

<div class="responsive">
   <div class="gallery">
     <a target="_blank" href="img_5terre.jpg">
       <img src="img_5terre.jpg" alt="Cinque Terre" kengligi="600" balandligi="400">
     </a>
     <div class="desc">Rasm tavsifini shu yerga qo'shing</div>
   </div>
</div>


<div class="responsive">
   <div class="gallery">
     <a target="_blank" href="img_forest.jpg">
       <img src="img_forest.jpg" alt="O'rmon" kengligi="600" balandligi="400">
     </a>
     <div class="desc">Rasm tavsifini shu yerga qo'shing</div>
   </div>
</div>

<div class="responsive">
   <div class="gallery">
     <a target="_blank" href="img_lights.jpg">
       <img src="img_lights.jpg" alt="Shimoliy chiroqlar" kengligi="600" balandligi="400">
     </a>
     <div class="desc">Rasm tavsifini shu yerga qo'shing</div>
   </div>
</div>

<div class="responsive">
   <div class="gallery">
     <a target="_blank" href="img_mountains.jpg">
       <img src="img_mountains.jpg" alt="Tog'lar" kengligi="600" balandligi="400">
     </a>
     <div class="desc">Rasm tavsifini shu yerga qo'shing</div>
   </div>
</div>

<div class="clearfix"></div>

<div style="padding:6px;">
   <p>Ushbu misol turli ekran o'lchamlaridagi tasvirlarni qayta joylashtirish uchun media so'rovlaridan foydalanadi: kattaroq ekranlar uchun

kengligi 700px dan katta bo'lsa, u to'rtta tasvirni yonma-yon ko'rsatadi, 700px dan kichik ekranlar uchun ikkitasini ko'rsatadi.

tasvirlar yonma-yon. 500px dan kichikroq ekranlar uchun tasvirlar vertikal ravishda joylashadi (100%).</p>
   <p>Media so'rovlari va sezgir veb-dizayn haqida batafsil ma'lumotni keyinroq CSS qo'llanmamizdan bilib olasiz.</p>
</div>

</body>
</html>

<kbd>qaytish</kbd>[Mundarijaga qaytish](#homepage)



--------



## CSS tasvir spritlari


Tasvir sprite - bu server so'rovlari sonini kamaytirish uchun bitta rasmga joylashtirilgan rasmlar to'plami,

tarmoqli kengligini tejash va bir nechta server so'rovlaridan kelib chiqqan sahifani yuklash vaqtini qisqartirish.



Oddiy misol: Rasm spritlari:::

Rasm spritlari bizga rasmning kerakli qismini ko'rsatishga imkon beradi. Bir nechta tasvirlar kompozitsiyasi ichida.

Quyidagi rasmga qarang:

<!DOCTYPE html>
<html>
<head>
<uslub>
#uy {
   kengligi: 46px;
   balandligi: 44px;
   fon: url (img_navsprites.gif) 0 0;
}

#Keyingisi {
   kengligi: 43px;
   balandligi: 44px;
   fon: url (img_navsprites.gif) -91px 0;
}
</style>
</head>
<tana>

<img id="home" src="img_trans.gif" width="1" height="1">
<img id="keyingi" src="img_trans.gif" kengligi="1" balandligi="1">

</body>
</html>


Yuqoridagi misolda,


     <img id="home" src="img_trans.gif"> - Faqat kichik shaffof tasvirni belgilaydi, chunki src atributi

bo'sh bo'lishi mumkin emas. Ko'rsatilgan rasm biz CSS-da belgilagan fon tasviri bo'ladi
     kengligi: 46px; balandligi: 44px; - Rasmning biz foydalanmoqchi bo'lgan qismini belgilaydi
     fon: url (img_navsprites.gif) 0 0; - Fon rasmi va uning o'rnini belgilaydi (chapda 0px, tepada

0px)





Image Sprites - Navigatsiya ro'yxatini yarating

Quyidagi rasmda sprite tasvir ("img_navsprites.gif") yordamida navigatsiya ro'yxatini yaratish ko'rsatilgan. An

Bu yerda HTML roʻyxati ishlatiladi, chunki u roʻyxat boʻlishi mumkin va fon tasvirini ham qoʻllab-quvvatlaydi. Rasmga qarang

hozir quyida:


<!DOCTYPE html>
<html>
<head>
<uslub>
#navlist {
   pozitsiya: nisbiy;
}

#navlist li {
   chegara: 0;
   to'ldirish: 0;
   ro'yxat uslubi: yo'q;
   pozitsiyasi: mutlaq;
   yuqori: 0;
}

#navlist li, #navlist a {
   balandligi: 44px;
   displey: blok;
}

#uy {
   chap: 0px;
   kengligi: 46px;
   fon: url('img_navsprites.gif') 0 0;
}

#oldingi {
   chap: 63px;
   kengligi: 43px;
   fon: url('img_navsprites.gif') -47px 0;
}

#Keyingisi {
   chap: 129px;
   kengligi: 43px;
   fon: url('img_navsprites.gif') -91px 0;
}
</style>
</head>
<tana>

<ul id="navlist">
   <li id="home"><a href="default.asp"></a></li>
   <li id="prev"><a href="css_intro.asp"></a></li>
   <li id="next"><a href="css_syntax.asp"></a></li>
</ul>

</body>
</html>


Yuqoridagi misol uchun tushuntirish:


     #navlist {pozitsiya: nisbiy;} - uning ichida mutlaq joylashishni ta'minlash uchun pozitsiya nisbatan o'rnatiladi
     #navlist li {margin:0;padding:0;list-style:none;position:absolute;top:0;} - chekka va to'ldirish o'rnatiladi

0 ga, ro'yxat uslubi o'chiriladi va barcha ro'yxat elementlari mutlaq joylashadi
     #navlist li, #navlist a {height:44px;display:block;} - barcha tasvirlarning balandligi 44px.


Har bir alohida qismni joylashtirish va uslublash:


     #home {left:0px;width:46px;} - Toʻliq chap tomonga joylashtirilgan va tasvirning kengligi 46px.
     #home {background:url(img_navsprites.gif) 0 0;} - Fon rasmi va uning oʻrnini belgilaydi (chapda)

0px, yuqori 0px)
     #prev {chap:63px;width:43px;} - 63px oʻngga joylashtirilgan (#uy kengligi 46px + biroz qoʻshimcha joy)

elementlar orasida) va kengligi 43px.
     #prev {background:url('img_navsprites.gif') -47px 0;} - Fon rasmini 47px oʻngga belgilaydi

(#uy kengligi 46px + 1px chiziq ajratuvchi)
     #keyingi {chap:129px;width:43px;}- 129px oʻngga joylashtirilgan (#oldingi 63px + #oldingi kengligi 43px)

+ qo'shimcha joy) va kengligi 43px.
     #next {background:url('img_navsprites.gif') -91px 0;} - Fon rasmini 91px oʻngga belgilaydi

(#uy kengligi 46px + 1px chiziqni ajratuvchi + #oldingi kengligi 43px + 1px chiziq boʻluvchisi )



Rasm spritlari - Hover effekti:::

Bu erda biz navigatsiya ro'yxatiga hover effektini qo'shamiz. E'tibor bering, :hover selektori hamma uchun ishlatilishi mumkin

elementlar, shu jumladan, lekin ular bilan cheklanmagan, havolalar.


<!DOCTYPE html>
<html>
<head>
<uslub>
#navlist {
   pozitsiya: nisbiy;
}

#navlist li {
   chegara: 0;
   to'ldirish: 0;
   ro'yxat uslubi: yo'q;
   pozitsiyasi: mutlaq;
   yuqori: 0;
}

#navlist li, #navlist a {
   balandligi: 44px;
   displey: blok;
}

#uy {
   chap: 0px;
   kengligi: 46px;
   fon: url('img_navsprites_hover.gif') 0 0;
}

#oldingi {
   chap: 63px;
   kengligi: 43px;
   fon: url('img_navsprites_hover.gif') -47px 0;
}

#Keyingisi {
   chap: 129px;
   kengligi: 43px;
   fon: url('img_navsprites_hover.gif') -91px 0;
}

#uy a: suring {
   fon: url('img_navsprites_hover.gif') 0 -45px;
}

#oldingi a: suring {
   fon: url('img_navsprites_hover.gif') -47px -45px;
}

#keyingi a: suring {
   fon: url('img_navsprites_hover.gif') -91px -45px;
}
</style>
</head>
<tana>

<ul id="navlist">
   <li id="home"><a href="default.asp"></a></li>
   <li id="prev"><a href="css_intro.asp"></a></li>
   <li id="next"><a href="css_syntax.asp"></a></li>
</ul>

</body>
</html>


Yuqoridagi misolning tushuntirishi:

     #home a:hover {background: url('img_navsprites_hover.gif') 0 -45px;} - Barcha uchta hover tasvir uchun biz

bir xil fon holatini belgilang, faqat 45px pastga


<kbd>qaytish</kbd>[Mundarijaga qaytish](#homepage)


------



## CSS Attr selektorlari
  
CSS atribut selektorlari


Muayyan atributlarga ega uslub HTML elementlari

Siz HTML elementlarini maxsus atributlar yoki atribut qiymatlari bilan uslublashingiz mumkin.



[atribut] selektori belgilangan atributga ega elementlarni tanlash uchun ishlatiladi.

Quyidagi misol maqsad atributiga ega barcha <a> elementlarni tanlaydi:


<!DOCTYPE html>
<html>
<head>
<uslub>
a[maqsad] {
   fon rangi: sariq;
}
</style>
</head>
<tana>

<h2>CSS [atribut] selektori</h2>
<p>Maqsadli atributli havolalar sariq fonga ega bo'ladi:</p>

<a href="https://www.w3schools.com">w3schools.com</a>
<a href="http://www.disney.com" target="_blank">disney.com</a>
<a href="http://www.wikipedia.org" target="_top">wikipedia.org</a>

</body>
</html>



CSS [attribute="value"] selektori

[attribute="value"] selektori belgilangan atribut va qiymatga ega elementlarni tanlash uchun ishlatiladi.

Quyidagi misol target="_blank" atributiga ega barcha <a> elementlarni tanlaydi:


<!DOCTYPE html>
<html>
<head>
<uslub>
a[target=_blank] {
   fon rangi: sariq;
}
</style>
</head>
<tana>

<h2>CSS [attribute="value"] Selektor</h2>
<p>Target="_blank" havolasi sariq fonga ega:</p>

<a href="https://www.w3schools.com">w3schools.com</a>
<a href="http://www.disney.com" target="_blank">disney.com</a>
<a href="http://www.wikipedia.org" target="_top">wikipedia.org</a>

</body>
</html>



CSS [atribut~="qiymat"] selektori


[atribut~="value"] selektori ko'rsatilgan atribut qiymatiga ega elementlarni tanlash uchun ishlatiladi

so'z.

Quyidagi misol bo'sh joy bilan ajratilgan ro'yxatini o'z ichiga olgan sarlavha atributiga ega barcha elementlarni tanlaydi

so'zlar, ulardan biri "gul":


<!DOCTYPE html>
<html>
<head>
<uslub>
[title~=gul] {
   chegara: 5px qattiq sariq;
}
</style>
</head>
<tana>

<h2>CSS [atribut~="value"] Selektor</h2>
<p>"Gul" so'zini o'z ichiga olgan sarlavha atributiga ega barcha rasmlar sariq hoshiyaga ega bo'ladi.</p>

<img src="klematis.jpg" title="klematis gul" kengligi="150" balandligi="113">
<img src="img_flwr.gif" title="gul" kengligi="224" balandligi="162">
<img src="img_tree.gif" title="daraxt" kengligi="200" balandligi="358">

</body>
</html>


Yuqoridagi misolda title="flower", title="yozgi gul" va title="gul new" bilan elementlar mos keladi.

lekin unvon = "mening gulim" yoki "gullar" emas.



CSS [atribut|="value"] selektori

[atribut|="value"] selektori belgilangan atribut bilan boshlanadigan elementlarni tanlash uchun ishlatiladi

belgilangan qiymat.

Quyidagi misol "yuqori" bilan boshlanadigan sinf atributi qiymatiga ega barcha elementlarni tanlaydi.

Eslatma: Qiymat yaxlit so'z bo'lishi kerak, masalan, class="top" yoki keyin chiziqcha( - ), kabi

class="top-matn"!


Quyidagi misolga qarang:

<!DOCTYPE html>
<html>
<head>
<uslub>
[sinf|=yuqori] {
   fon: sariq;
}
</style>
</head>
<tana>

<h2>CSS [atribut|="value"] Selektor</h2>

<h1 class="top-header">Xush kelibsiz</h1>
<p class="top-text">Salom dunyo!</p>
<p class="topcontent">CSS-ni o'rganyapsizmi?</p>

</body>
</html>



CSS [atribut^="value"] selektori

[atribut^="value"] selektori atribut qiymati belgilangan qiymatdan boshlanadigan elementlarni tanlash uchun ishlatiladi.

qiymat.

Quyidagi misol "yuqori" bilan boshlanadigan sinf atributi qiymatiga ega barcha elementlarni tanlaydi:

Eslatma: Qiymat butun so'z bo'lishi shart emas! Bu holda yuqori tarkib va yuqori tarkib tanlanadi.


<!DOCTYPE html>
<html>
<head>
<uslub>
[sinf ^ = "yuqori"] {
   fon: sariq;
}
</style>
</head>
<tana>

<h2>CSS [atribut^="value"] Selektor</h2>

<h1 class="top-header">Xush kelibsiz</h1>
<p class="top-text">Salom dunyo!</p>
<p class="topcontent">CSS-ni o'rganyapsizmi?</p>

</body>
</html>



CSS [attribute$="value"] selektori

[attribute$="value"] selektori atribut qiymati belgilangan qiymat bilan tugaydigan elementlarni tanlash uchun ishlatiladi.

qiymat.

Quyidagi misol "test" bilan tugaydigan sinf atributi qiymatiga ega barcha elementlarni tanlaydi:

Eslatma: Qiymat butun so'z bo'lishi shart emas!

<!DOCTYPE html>
<html>
<head>
<uslub>
[sinf $ = "test"] {
   fon: sariq;
}
</style>
</head>
<tana>

<h2>CSS [attribute$="value"] selektori</h2>

<div class="first_test">Birinchi div elementi.</div>
<div class="second">Ikkinchi div elementi.</div>
<div class="my-test">Uchinchi div elementi.</div>
<p class="mytest">Bu paragrafdagi matn.</p>

</body>
</html>


CSS [attribute*="value"] selektori

[atribut*="value"] selektori atribut qiymati ko'rsatilgan elementlarni tanlash uchun ishlatiladi

qiymat.

Quyidagi misol "te" ni o'z ichiga olgan sinf atributi qiymatiga ega barcha elementlarni tanlaydi:

Eslatma: Qiymat butun so'z bo'lishi shart emas!


<!DOCTYPE html>
<html>
<head>
<uslub>
[sinf*="te"] {
   fon: sariq;
}
</style>
</head>
<tana>

<h2>CSS [attribute*="value"] Selektor</h2>

<div class="first_test">Birinchi div elementi.</div>
<div class="second">Ikkinchi div elementi.</div>
<div class="my-test">Uchinchi div elementi.</div>
<p class="mytest">Bu paragrafdagi matn.</p>

</body>
</html>


Styling shakllari

Atribut selektorlari sinf yoki identifikatorsiz shakllarni shakllantirish uchun foydali bo'lishi mumkin:


<!DOCTYPE html>
<html>
<head>
<uslub>
kiritish[type=matn] {
   kengligi: 150px;
   displey: blok;
   pastki chet: 10px;
   fon rangi: sariq;
}

kiritish[type=tugma] {
   kengligi: 120px;
   chap chekka: 35px;
   displey: blok;
}
</style>
</head>
<tana>

<h2>Uslublar shakllari</h2>

<form name="input" action="" method="get">
   Ism:<input type="text" name="Name" value="Piter" size="20">
   Familiya:<input type="text" name="Name" value="Griffin" size="20">
   <input type="tugma" qiymati="Misol tugmasi">
</form>

</body>
</html>




Barcha CSS atribut selektorlari
Selektor misoli Misol tavsifi
[atribut] [maqsad] Maqsad atributiga ega barcha elementlarni tanlaydi
[atribut=value] [target=_blank] target="_blank" bilan barcha elementlarni tanlaydi
[atribut~=qiymat] [title~=gul] Sarlavha atributiga ega barcha elementlarni tanlaydi.

"gul" so'zi
[atribut|=value] [lang|=en] “en” bilan boshlanadigan lang atribut qiymatiga ega barcha elementlarni tanlaydi
[atribut^=value] a[href^="https"] href atribut qiymati boshlanadigan har bir <a> elementni tanlaydi

"https" bilan
[attribute$=value] a[href$=".pdf"] href atribut qiymati tugaydigan har bir <a> elementni tanlaydi

".pdf" bilan
[atribut*=value] a[href*="w3schools"] href atribut qiymatiga ega har bir <a> elementni tanlaydi

"w3schools" pastki qatorini o'z ichiga oladi

<kbd>qaytish</kbd>[Mundarijaga qaytish](#homepage)



------


## CSS hisoblagichlari


Ular CSS-qo'llab-quvvatlanadigan o'zgaruvchilar bo'lib, ularning qiymatlari CSS qoidalari bo'yicha qo'shimcha bo'lishi mumkin (marta sonini kuzatish uchun)

ular ishlatiladi). Kontentning ko'rinishini uning joylashuviga qarab sozlash uchun hisoblagichlardan ham foydalanishingiz mumkin

hujjat.


Hisoblagichlar bilan avtomatik raqamlash

CSS hisoblagichlari "o'zgaruvchilar" ga o'xshaydi. O'zgaruvchi qiymatlari CSS qoidalari bilan oshirilishi mumkin (bu qanday qilib kuzatilishini kuzatib boradi

ko'p marta ishlatiladi).

CSS hisoblagichlari bilan ishlash uchun biz quyidagi xususiyatlardan foydalanamiz:

     counter-reset - hisoblagichni yaratadi yoki qayta o'rnatadi
     counter-increment - hisoblagich qiymatini oshiradi
     kontent - Yaratilgan tarkibni kiritadi
     counter() yoki counters() funksiyasi - elementga hisoblagich qiymatini qo'shadi

CSS hisoblagichidan foydalanish uchun avval uni qayta tiklash bilan yaratish kerak.


Tasavvur qilish uchun quyidagi misol sahifa uchun hisoblagich yaratadi (tana selektorida), ni oshiradi

Har bir <h2> elementi uchun hisoblagich qiymati va har bir <h2> elementining boshiga “<hisoblagich qiymati>:” boʻlimi qoʻshiladi.

element:

<!DOCTYPE html>
<html>
<head>
<uslub>
tana {
   qarshi qayta o'rnatish: bo'lim;
}

h2 :: oldin {
   qarama-qarshi o'sish: bo'lim;
   tarkib: "Bo'lim " counter(bo'lim) ": ";
}
</style>
</head>
<tana>

<h1>CSS hisoblagichlaridan foydalanish</h1>

<h2>HTML darsligi</h2>
<h2>CSS darsligi</h2>
<h2>JavaScript darsligi</h2>
<h2>Python darsligi</h2>
<h2>SQL darsligi</h2>

</body>
</html>


Yuqoridagi misolda natija shunday ko'rinadi:


CSS hisoblagichlaridan foydalanish

1-bo'lim: HTML qo'llanmasi
2-bo'lim: CSS qo'llanmasi
3-bo'lim: JavaScript qo'llanmasi
4-bo'lim: Python qo'llanmasi
5-bo'lim: SQL qo'llanmasi

Va siz ta'kidlaganingizda, "1-dan 5-gachasi bo'lim" ajratilmaydi, chunki u avtomatik ravishda yaratiladi.

CSS.





Yuvalash hisoblagichlari

Quyidagi misol sahifa (bo'lim) uchun bitta hisoblagich va har bir <h1> elementi uchun bitta hisoblagich yaratadi

(kichik bo'lim). "Bo'lim" hisoblagichi har bir <h1> element uchun "bo'lim <qiymati" bilan hisoblanadi

bo'lim hisoblagichi>.", va "kichik bo'lim" hisoblagichi har bir <h2> element uchun "<qiymati" bilan hisoblanadi.

bo'lim hisoblagichi>.<kichik bo'lim hisoblagichining qiymati>":


<!DOCTYPE html>
<html>
<head>
<uslub>
tana {
   qarshi qayta o'rnatish: bo'lim;
}

h1 {
   qarshi qayta o'rnatish: kichik bo'lim;
}

h1 :: oldin {
   qarama-qarshi o'sish: bo'lim;
   mazmuni: "Bo'lim" hisoblagich(bo'lim) ". ";
}

h2 :: oldin {
   qarama-qarshi o'sish: kichik bo'lim;
   tarkib: hisoblagich (bo'lim) "." hisoblagich (kichik bo'lim) " ";
}
</style>
</head>
<tana>


<h1>HTML/CSS darsliklari</h1>
<h2>HTML</h2>
<h2>CSS</h2>
<h2>Bootstrap</h2>
<h2>W3.CSS</h2>

<h1>Skript yaratish boʻyicha qoʻllanmalar</h1>
<h2>JavaScript</h2>
<h2>jQuery</h2>
<h2>Reaksiya</h2>

<h1>Dasturlash bo'yicha qo'llanmalar</h1>
<h2>Python</h2>
<h2>Java</h2>
<h2>C++</h2>

</body>
</html>


Yuqoridagi ichki hisoblagichlar quyidagicha ko'rsatiladi:

1-bo'lim. HTML/CSS darsliklari

1.1 HTML
1.2 CSS
1.3 Bootstrap
1.4 W3.CSS

2-bo'lim. Skript yaratish bo'yicha qo'llanmalar

2.1 JavaScript
2.2 jQuery
2.3 Reaksiya

3-bo'lim. Dasturlash bo'yicha qo'llanmalar

3.1 Python
3.2 Java
3.3 C++



Hisoblagich belgilangan ro'yxatlarni yaratish uchun ham foydali bo'lishi mumkin, chunki hisoblagichning yangi nusxasi avtomatik ravishda paydo bo'ladi

bola elementlarda yaratilgan. Bu yerda biz counters() funksiyasidan turli darajalar orasiga qator kiritish uchun foydalanamiz

o'rnatilgan hisoblagichlar:

<!DOCTYPE html>
<html>
<head>
<uslub>
ol {
   qarshi qayta o'rnatish: bo'lim;
   ro'yxat uslubi turi: yo'q;
}

li :: oldin {
   qarama-qarshi o'sish: bo'lim;
   tarkib: hisoblagichlar(bo'lim,".") " ";
}
</style>
</head>
<tana>

<ol>
   <li>element</li>
   <li>element
   <ol>
     <li>element</li>
     <li>element</li>
     <li>element
     <ol>
       <li>element</li>
       <li>element</li>
       <li>element</li>
     </ol>
     </li>
     <li>element</li>
   </ol>
   </li>
   <li>element</li>
   <li>element</li>
</ol>

<ol>
   <li>element</li>
   <li>element</li>
</ol>

</body>
</html>


Yuqoridagi hisoblagich quyida ko'rsatilgandek ko'rsatilgan:


     1 ta element
     2 ta element
         2.1 band
         2.2-band
         2.3-band
             2.3.1-band
             2.3.2-band
             2.3.3-band
         2.4-band
     3 ta element
     4 ta element

     1 ta element
     2 ta element


CSS hisoblagich xususiyatlari
Mulk tavsifi
kontent Yaratilgan tarkibni kiritish uchun ::oldin va ::pseudo-elementlar bilan ishlatiladi
counter-increment Bir yoki bir nechta hisoblagich qiymatlarini oshiradi
counter-reset Bir yoki bir nechta hisoblagichlarni yaratadi yoki qayta o'rnatadi
counter() Nomlangan hisoblagichning joriy qiymatini qaytaradi


<kbd>qaytish</kbd>[Mundarijaga qaytish](#homepage)


--------


## CSS veb-sayt tartibi

Veb-sayt tartibi

Veb-sayt ko'pincha sarlavhalar, menyular, kontent va altbilgiga bo'linadi:

Tanlash uchun juda ko'p turli xil dizayn dizaynlari mavjud. Biroq, yuqoridagi tuzilma eng ko'p biridir

keng tarqalgan va biz buni ushbu qo'llanmada batafsil ko'rib chiqamiz.


Sarlavha

Sarlavha odatda veb-saytning yuqori qismida (yoki yuqori navigatsiya menyusi ostida) joylashgan. Tez-tez

logotip yoki veb-sayt nomini o'z ichiga oladi:


<!DOCTYPE html>
<html lang="en">
<head>
<title>CSS veb-sayt tartibi</title>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<uslub>
tana {
   chegara: 0;
}

/* Sarlavhani uslublash */
.sarlavha {
   fon rangi: #f1f1f1;
   to'ldirish: 20px;
   matnni tekislash: markaz;
}
</style>
</head>
<tana>

<div class="header">
   <h1>Sarlavha</h1>
</div>

</body>
</html>



Navigatsiya paneli


Navigatsiya paneli tashrif buyuruvchilarga veb-saytingizda harakat qilishiga yordam beradigan havolalar ro'yxatini o'z ichiga oladi:


<!DOCTYPE html>
<html lang="en">
<head>
<title>CSS veb-sayt tartibi</title>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<uslub>
* {
   quti o'lchami: chegara qutisi;
}

tana {
   chegara: 0;
}

/* Sarlavhani uslublash */
.sarlavha {
   fon rangi: #f1f1f1;
   to'ldirish: 20px;
   matnni tekislash: markaz;
}

/* Yuqori navigatsiya panelini uslublash */
.topnav {
   toshib ketish: yashirin;
   fon rangi: #333;
}

/* Topnav havolalarini uslublash */
.topnav a {
   float: chap;
   displey: blok;
   rang: #f2f2f2;
   matnni tekislash: markaz;
   to'ldirish: 14px 16px;
   matn-bezak: yo'q;
}

/* sichqonchani ko'targanda rangni o'zgartiring */
.topnav a: hover {
   fon rangi: #ddd;
   rang: qora;
}
</style>
</head>
<tana>

<div class="header">
   <h1>Sarlavha</h1>
</div>

<div class="topnav">
   <a href="#">Havola</a>
   <a href="#">Havola</a>
   <a href="#">Havola</a>
</div>

</body>
</html>


Tarkib

Ushbu bo'limdagi tartib ko'pincha maqsadli foydalanuvchilarga bog'liq. Eng keng tarqalgan tartib - bitta (yoki birlashtiruvchi

ular) quyidagilardan:

     1-ustun (ko'pincha mobil brauzerlar uchun ishlatiladi)
     2 ustunli (ko'pincha planshetlar va noutbuklar uchun ishlatiladi)
     3 ustunli tartib (faqat ish stoli uchun ishlatiladi)

Biz 3 ustunli tartibni yaratamiz va uni kichikroq ekranlarda 1 ustunli tartibga o'zgartiramiz:


<!DOCTYPE html>
<html lang="en">
<head>
<title>CSS veb-sayt tartibi</title>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<uslub>
* {
   quti o'lchami: chegara qutisi;
}

tana {
   chegara: 0;
}

/* Sarlavhani uslublash */
.sarlavha {
   fon rangi: #f1f1f1;
   to'ldirish: 20px;
   matnni tekislash: markaz;
}

/* Yuqori navigatsiya panelini uslublash */
.topnav {
   toshib ketish: yashirin;
   fon rangi: #333;
}

/* Topnav havolalarini uslublash */
.topnav a {
   float: chap;
   displey: blok;
   rang: #f2f2f2;
   matnni tekislash: markaz;
   to'ldirish: 14px 16px;
   matn-bezak: yo'q;
}

/* sichqonchani ko'targanda rangni o'zgartiring */
.topnav a: hover {
   fon rangi: #ddd;
   rang: qora;
}

/* Bir-birining yonida suzuvchi uchta teng ustun yarating */
.ustun {
   float: chap;
   kengligi: 33,33%;
   to'ldirish: 15px;
}

/* Ustunlardan keyingi floatlarni tozalash */
.qator:keyin {
   tarkib: "";
   ko'rsatish: jadval;
   aniq: ikkalasi ham;
}

/* Ta’sirchan tartib – uchta ustunni yonma-yon emas, bir-birining ustiga qo‘yadi */
@media ekrani va (maksimal kenglik: 600px) {
   .ustun {
     kengligi: 100%;
   }
}
</style>
</head>
<tana>

<div class="header">
   <h1>Sarlavha</h1>
   <p>Ta'sirchan effektni ko'rish uchun brauzer oynasining o'lchamini o'zgartiring.</p>
</div>

<div class="topnav">
   <a href="#">Havola</a>
   <a href="#">Havola</a>
   <a href="#">Havola</a>
</div>

<div class="satr">
   <div class="ustun">
     <h2>Ustun</h2>
     <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Mesenatlar amet pretium urna o'tirishadi. Vivamus

venenatis velit nec neque ultricies, eget elementum magna tristique. Quisque Vehicula, Risus Eget Aliquam

placerat, purus leo tincidunt eros, eget luctus quam orci in velit. Praesent sclerisque tortor sed accumsan

convallis.</p>
   </div>
  
   <div class="ustun">
     <h2>Ustun</h2>
     <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Mesenatlar amet pretium urna o'tirishadi. Vivamus

venenatis velit nec neque ultricies, eget elementum magna tristique. Quisque Vehicula, Risus Eget Aliquam

placerat, purus leo tincidunt eros, eget luctus quam orci in velit. Praesent sclerisque tortor sed accumsan

convallis.</p>
   </div>
  
   <div class="ustun">
     <h2>Ustun</h2>
     <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Mesenatlar amet pretium urna o'tirishadi. Vivamus

venenatis velit nec neque ultricies, eget elementum magna tristique. Quisque Vehicula, Risus Eget Aliquam

placerat, purus leo tincidunt eros, eget luctus quam orci in velit. Praesent sclerisque tortor sed accumsan

convallis.</p>
   </div>
</div>

</body>
</html>


Maslahat: 2 ustunli tartib yaratish uchun kenglikni 50% ga o'zgartiring. 4 ustunli tartibni yaratish uchun 25% va hokazolardan foydalaning.
Maslahat: @media qoidasi qanday ishlashini bilish uchun CSS Media so'rovlari bo'limiga qarang

Maslahat: Ustun maketlarini yaratishning zamonaviy usuli bu CSS Flexbox-dan foydalanishdir. Biroq, u qo'llab-quvvatlanmaydi

Internet Explorer 10 va undan oldingi versiyalari. Agar sizga IE6-10 yordami kerak bo'lsa, floatlardan foydalaning (yuqorida ko'rsatilganidek).



Teng bo'lmagan ustunlar

Asosiy tarkib saytingizning eng katta va eng muhim qismidir.

Bu teng bo'lmagan ustunlar kengligi bilan keng tarqalgan, shuning uchun bo'sh joyning katta qismi asosiy tarkib uchun ajratilgan. The

yon kontent (agar mavjud bo'lsa) ko'pincha muqobil navigatsiya sifatida yoki tegishli ma'lumotlarni ko'rsatish uchun ishlatiladi

asosiy tarkib. Kengliklarni xohlaganingizcha o'zgartiring, faqat jami 100% gacha qo'shilishi kerakligini yodda tuting:

<!DOCTYPE html>
<html lang="en">
<head>
<title>CSS veb-sayt tartibi</title>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<uslub>
* {
   quti o'lchami: chegara qutisi;
}

tana {
   chegara: 0;
}

/* Sarlavhani uslublash */
.sarlavha {
   fon rangi: #f1f1f1;
   to'ldirish: 20px;
   matnni tekislash: markaz;
}

/* Yuqori navigatsiya panelini uslublash */
.topnav {
   toshib ketish: yashirin;
   fon rangi: #333;
}

/* Topnav havolalarini uslublash */
.topnav a {
   float: chap;
   displey: blok;
   rang: #f2f2f2;
   matnni tekislash: markaz;
   to'ldirish: 14px 16px;
   matn-bezak: yo'q;
}

/* sichqonchani ko'targanda rangni o'zgartiring */
.topnav a: hover {
   fon rangi: #ddd;
   rang: qora;
}

/* Bir-birining yonida suzuvchi uchta teng bo'lmagan ustunlar yarating */
.ustun {
   float: chap;
   to'ldirish: 10px;
}

/* Chap va o'ng ustun */
.ustun.tomoni {
   kengligi: 25%;
}

/* o'rta ustun */
.ustun.middle {
   kengligi: 50%;
}

/* Ustunlardan keyingi floatlarni tozalash */
.qator:keyin {
   tarkib: "";
   ko'rsatish: jadval;
   aniq: ikkalasi ham;
}

/* Ta’sirchan tartib – uchta ustunni yonma-yon emas, bir-birining ustiga qo‘yadi */
@media ekrani va (maksimal kenglik: 600px) {
   .ustun.yon, .ustun.oʻrta {
     kengligi: 100%;
   }
}
</style>
</head>
<tana>

<div class="header">
   <h1>Sarlavha</h1>
   <p>Ta'sirchan effektni ko'rish uchun brauzer oynasining o'lchamini o'zgartiring.</p>
</div>

<div class="topnav">
   <a href="#">Havola</a>
   <a href="#">Havola</a>
   <a href="#">Havola</a>
</div>

<div class="satr">
   <div class="ustun tomoni">
     <h2>Yon</h2>
     <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit..</p>
   </div>
  
   <div class="ustun o'rtasi">
     <h2>Asosiy tarkib</h2>
     <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Mesenatlar amet pretium urna o'tirishadi. Vivamus

venenatis velit nec neque ultricies, eget elementum magna tristique. Quisque Vehicula, Risus Eget Aliquam

placerat, purus leo tincidunt eros, eget luctus quam orci in velit. Praesent sclerisque tortor sed accumsan

convallis.</p>
     <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Mesenatlar amet pretium urna o'tirishadi. Vivamus

venenatis velit nec neque ultricies, eget elementum magna tristique. Quisque Vehicula, Risus Eget Aliquam

placerat, purus leo tincidunt eros, eget luctus quam orci in velit. Praesent sclerisque tortor sed accumsan

convallis.</p>
   </div>
  
   <div class="ustun tomoni">
     <h2>Yon</h2>
     <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit..</p>
   </div>
</div>
  
</body>
</html>


Altbilgi

Altbilgi sahifangizning pastki qismida joylashgan. U ko'pincha mualliflik huquqi va aloqa kabi ma'lumotlarni o'z ichiga oladi

ma'lumot:



<!DOCTYPE html>
<html lang="en">
<head>
<title>CSS veb-sayt tartibi</title>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<uslub>
* {
   quti o'lchami: chegara qutisi;
}

tana {
   chegara: 0;
}

/* Sarlavhani uslublash */
.sarlavha {
   fon rangi: #f1f1f1;
   to'ldirish: 20px;
   matnni tekislash: markaz;
}

/* Yuqori navigatsiya panelini uslublash */
.topnav {
   toshib ketish: yashirin;
   fon rangi: #333;
}

/* Topnav havolalarini uslublash */
.topnav a {
   float: chap;
   displey: blok;
   rang: #f2f2f2;
   matnni tekislash: markaz;
   to'ldirish: 14px 16px;
   matn-bezak: yo'q;
}

/* sichqonchani ko'targanda rangni o'zgartiring */
.topnav a: hover {
   fon rangi: #ddd;
   rang: qora;
}

/* Bir-birining yonida suzuvchi uchta teng bo'lmagan ustunlar yarating */
.ustun {
   float: chap;
   to'ldirish: 10px;
}

/* Chap va o'ng ustun */
.ustun.tomoni {
   kengligi: 25%;
}

/* o'rta ustun */
.ustun.middle {
   kengligi: 50%;
}

/* Ustunlardan keyingi floatlarni tozalash */
.qator:keyin {
   tarkib: "";
   ko'rsatish: jadval;
   aniq: ikkalasi ham;
}

/* Ta’sirchan tartib – uchta ustunni yonma-yon emas, bir-birining ustiga qo‘yadi */
@media ekrani va (maksimal kenglik: 600px) {
   .ustun.yon, .ustun.oʻrta {
     kengligi: 100%;
   }
}

/* Altbilgiga uslub */
.footer {
   fon rangi: #f1f1f1;
   to'ldirish: 10px;
   matnni tekislash: markaz;
}
</style>
</head>
<tana>

<div class="header">
   <h1>Sarlavha</h1>
   <p>Ta'sirchan effektni ko'rish uchun brauzer oynasining o'lchamini o'zgartiring.</p>
</div>

<div class="topnav">
   <a href="#">Havola</a>
   <a href="#">Havola</a>
   <a href="#">Havola</a>
</div>

<div class="satr">
   <div class="ustun tomoni">
     <h2>Yon</h2>
     <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit..</p>
   </div>
  
   <div class="ustun o'rtasi">
     <h2>Asosiy tarkib</h2>
     <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Mesenatlar amet pretium urna o'tirishadi. Vivamus

venenatis velit nec neque ultricies, eget elementum magna tristique. Quisque Vehicula, Risus Eget Aliquam

placerat, purus leo tincidunt eros, eget luctus quam orci in velit. Praesent sclerisque tortor sed accumsan

convallis.</p>
     <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Mesenatlar amet pretium urna o'tirishadi. Vivamus

venenatis velit nec neque ultricies, eget elementum magna tristique. Quisque Vehicula, Risus Eget Aliquam

placerat, purus leo tincidunt eros, eget luctus quam orci in velit. Praesent sclerisque tortor sed accumsan

convallis.</p>
   </div>
  
   <div class="ustun tomoni">
     <h2>Yon</h2>
     <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit..</p>
   </div>
</div>

<div class="footer">
   <p>Alt-bilgi</p>
</div>
  
</body>
</html>

Javob beruvchi veb-sayt tartibi

Yuqoridagi ba'zi CSS kodlaridan foydalanib, biz javob beruvchi veb-sayt tartibini yaratdik, u ikkitadan farq qiladi.

ekran kengligiga qarab ustunlar va to'liq kenglikdagi ustunlar:


<!DOCTYPE html>
<html>
<head>
<uslub>
* {
   quti o'lchami: chegara qutisi;
}

tana {
   shrift oilasi: Arial;
   to'ldirish: 10px;
   fon: #f1f1f1;
}

/* Sarlavha/Blog sarlavhasi */
.sarlavha {
   to'ldirish: 30px;
   matnni tekislash: markaz;
   fon: oq;
}

.header h1 {
   shrift o'lchami: 50px;
}

/* Yuqori navigatsiya panelini uslublash */
.topnav {
   toshib ketish: yashirin;
   fon rangi: #333;
}

/* Topnav havolalarini uslublash */
.topnav a {
   float: chap;
   displey: blok;
   rang: #f2f2f2;
   matnni tekislash: markaz;
   to'ldirish: 14px 16px;
   matn-bezak: yo'q;
}

/* sichqonchani ko'targanda rangni o'zgartiring */
.topnav a: hover {
   fon rangi: #ddd;
   rang: qora;
}

/* Bir-birining yonida suzuvchi ikkita teng bo'lmagan ustunlar yarating */
/* Chap ustun */
.chap ustun {
   float: chap;
   kengligi: 75%;
}

/* o'ng ustun */
.o'ng ustun {
   float: chap;
   kengligi: 25%;
   fon rangi: #f1f1f1;
   padding-chap: 20px;
}

/* Soxta rasm */
.fakeimg {
   fon rangi: #aaa;
   kengligi: 100%;
   to'ldirish: 20px;
}

/* Maqolalar uchun karta effektini qo'shing */
.karta {
   fon rangi: oq;
   to'ldirish: 20px;
   yuqori chegara: 20px;
}

/* Ustunlardan keyingi floatlarni tozalash */
.qator:keyin {
   tarkib: "";
   ko'rsatish: jadval;
   aniq: ikkalasi ham;
}

/* Altbilgi */
.footer {
   to'ldirish: 20px;
   matnni tekislash: markaz;
   fon: #ddd;
   yuqori chegara: 20px;
}

/* Javob beruvchi tartib - ekran kengligi 800px dan kam bo'lsa, ikkita ustunni har birining ustiga qo'ying.

bir-birining o'rniga boshqa */
@media ekrani va (maksimal kenglik: 800px) {
   .leftcolumn, .rightcolumn {
     kengligi: 100%;
     to'ldirish: 0;
   }
}

/* Javob beruvchi tartib - ekran kengligi 400px dan kam bo'lsa, navigatsiya havolalarini tepaga joylashtiring.

bir-birining o'rniga bir-birlari */
@media ekrani va (maksimal kenglik: 400px) {
   .topnav a {
     float: yo'q;
     kengligi: 100%;
   }
}
</style>
</head>
<tana>

<div class="header">
   <h1>Mening veb-saytim</h1>
   <p>Effektni ko'rish uchun brauzer oynasining o'lchamini o'zgartiring.</p>
</div>

<div class="topnav">
   <a href="#">Havola</a>
   <a href="#">Havola</a>
   <a href="#">Havola</a>
   <a href="#" style="float:right">Havola</a>
</div>

<div class="satr">
   <div class="leftcolumn">
     <div class="card">
       <h2>SARLI SAVOL</h2>
       <h5>Sarlavha tavsifi, 2017-yil 7-dekabr</h5>
       <div class="fakeimg" style="height:200px;">Rasm</div>
       <p>Ba'zi matn..</p>
       <p>Unt in culpa qui officia deserunt mollit anim id est laborum consectetur adipiscing elit, sed do

eiusmod tempor incididunt ut labore va doore magna aliqua. Ut enim ad minim veniam, quis nostrud

mashqlar ullamco.</p>
     </div>
     <div class="card">
       <h2>SARLI SAVOL</h2>
       <h5>Sarlavha tavsifi, 2017-yil, 2-sentabr</h5>
       <div class="fakeimg" style="height:200px;">Rasm</div>
       <p>Ba'zi matn..</p>
       <p>Unt in culpa qui officia deserunt mollit anim id est laborum consectetur adipiscing elit, sed do

eiusmod tempor incididunt ut labore va doore magna aliqua. Ut enim ad minim veniam, quis nostrud

mashqlar ullamco.</p>
     </div>
   </div>
   <div class="rightcolumn">
     <div class="card">
       <h2>Men haqimda</h2>
       <div class="fakeimg" style="height:100px;">Rasm</div>
       <p>Men haqimda ba'zi matn culpa qui officia deserunt mollit anim..</p>
     </div>
     <div class="card">
       <h3>Mashhur post</h3>
       <div class="fakeimg"><p>Rasm</p></div>
       <div class="fakeimg"><p>Rasm</p></div>
       <div class="fakeimg"><p>Rasm</p></div>
     </div>
     <div class="card">
       <h3>Meni kuzatib boring</h3>
       <p>Ba'zi matn..</p>
     </div>
   </div>
</div>

<div class="footer">
   <h2>Alt-bilgi</h2>
</div>

</body>
</html>


<kbd>qaytish</kbd>[Mundarijaga qaytish](#homepage)


------