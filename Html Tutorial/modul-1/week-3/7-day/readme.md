## HTML LAYOUT
HTML LAYOUT--Layout elementlari va texnikasi

HTMLda semantik elementlar mavjud
```
<header> - Hujjat yoki bo'lim uchun sarlavhani belgilaydi
<nav> - navigatsiya havolalari to'plamini belgilaydi
<bo'lim> - Hujjatdagi bo'limni belgilaydi
<maqola> - mustaqil, mustaqil tarkibni belgilaydi
<chekka> - kontentdan tashqari tarkibni belgilaydi (yon panel kabi)
<footer> - Hujjat yoki bo'lim uchun pastki ko'rsatkichni belgilaydi
<etails> - foydalanuvchi talabiga ko'ra ochishi va yopishi mumkin bo'lgan qo'shimcha tafsilotlarni belgilaydi
<xulosa> - <details> elementi uchun sarlavhani belgilaydi
```

HTML maketlarini yaratish texnikasi
CSS ramkasi
CSS float xususiyati
CSS flexbox
CSS tarmog'i

* CSS Frameworks: Tezda maketingizni yaratishga imkon beradi: W3.CSS va Boostrap misollardir

CSS Float layout: Veb-layout qilish uchun CSS float xususiyatidan foydalaning. Buni ishlatish uchun faqat float va aniq xususiyatlarni eslab qolishingiz kerak. Uning asosiy kamchiligi - bu moslashuvchanlikka zarar etkazishi mumkin bo'lgan hujjat oqimiga bog'langan.

CSS Flexbox layout::Foydalanuvchi ekranining bir nechta o'lchamlari saytni yaxshi ko'rsatishi kerak bo'lganda elementlarning taxminiy tarzda harakat qilishini ta'minlaydi.


CSS Gridlayout: Veb-sahifalarni floatsiz va joylashishni aniqlashsiz loyihalash va bunga erishish uchun qatorlar va ustunlardan foydalanishni osonlashtiradigan gridga asoslangan tartib tizimini taklif qiladi.

<kbd>qaytish</kbd>[Mundarijaga qaytish](#homepage)


------

## HTML RESPONSIVE

HTML RESPONSIVE - javob beruvchi veb-dizayn;

Qurilmadan qat'i nazar, sezgir veb-sayt yaxshi ko'rinadi va u avtomatik ravishda turli o'lchamlar va ko'rish oynalariga moslashadi.

Bu yerda HTML va CSS barcha qurilmalarda (ish stollari, planshetlar va telefonlar) yaxshi ko‘rinishi uchun sayt o‘lchamini avtomatik ravishda o‘zgartiradi, yashiradi, kichraytiradi yoki kattalashtiradi.

Javob beruvchi sayt yaratish uchun barcha veb-sahifalaringizga quyidagi <meta> tegini qo'shing:
```

  <meta name="viewport" content="width=device-width, initial-scale=1.0">
```
* Ta'sirchan tasvirlar: brauzerning istalgan o'lchamiga mos keladigan darajada o'lchab ko'ring. Tasvirni sezgir qilish uchun CSS kengligi xususiyatini 100% ga o'rnating va tasvir ehtiyojlarga qarab javob beradi.
Javob beruvchi tasvir uchun quyidagi kodga qarang.
```
  <img src="img_girl.jpg" style="width:100%;">
```
Tasvirning asl hajmidan oshib ketishining oldini olish uchun width:100% oʻrniga max-width xususiyatidan foydalaning. Masalan:
```
  <img src="img_girl.jpg" style="max-width:100%;height:auto;">
```

** Brauzer kengligiga qarab turli xil tasvirlarni ko'rsatish uchun <rasm> elementidan foydalaning.

```
<rasm>
   <source srcset="img_smallflower.jpg" media="(maksimal kenglik: 600px)">
   <source srcset="img_flowers.jpg" media="(maksimal kenglik: 1500px)">
   <source srcset="flowers.jpg">
   <img src="img_smallflower.jpg" alt="Gullar">
</rasm>
```

** Javob beruvchi matn hajmi.

Matn o'lchamini ```"vw"``` birligi bilan o'rnatish mumkin, ya'ni ```"ko'rish maydoni kengligi"``` matn o'lchamini brauzer oynasi o'lchamiga mos kelishini bildiradi.

* Quyidagi kod javob beruvchi matn hajmini ta'minlaydi
```
<h1 style="font-size:10vw">Salom dunyo</h1>
```
* Viewport - bu brauzer oynasining o'lchami. 1vw = ko'rish maydoni kengligining 1%. Agar ko'rish maydoni 50 sm kengligida bo'lsa, 1vw 0,5 sm.


* Media so'rovlari: Turli xil brauzer o'lchamlari uchun mutlaqo boshqa uslublarni aniqlash imkonini beradi.

```
<uslub>
.chap, o'ng {
   float: chap;
   kengligi: 20%; /* Kengligi sukut bo'yicha 20% */
}

.asosiy {
   float: chap;
   kengligi: 60%; /* Kengligi sukut bo'yicha 60% */
}

/* 800px da toʻxtash nuqtasini qoʻshish uchun media soʻrovidan foydalaning: */
@media ekrani va (maksimal kenglik: 800px) {
   .chap, .asosiy, .oʻng {
     kengligi: 100%; /* Ko‘rish oynasi 800px yoki undan kichikroq bo‘lsa, kengligi 100% */
   }
}
</style>
```

* W3.CSS

W3.CSS ish stoli, planshet va mobil dizaynni sukut bo'yicha qo'llab-quvvatlaydigan zamonaviy CSS ramkasidir.

W3.CSS shunga o'xshash CSS ramkalariga qaraganda kichikroq va tezroq.

W3.CSS Bootstrap-ga yuqori sifatli muqobil sifatida ishlab chiqilgan.

W3.CSS jQuery yoki boshqa JavaScript kutubxonasidan mustaqil bo'lishi uchun yaratilgan.


** To'liq javob beruvchi vebga misol
```
<!DOCTYPE html>
<html>
<meta name="viewport" content="width=device-width, initial-scale=1">
<link rel="stylesheet" href="https://www.w3schools.com/w3css/4/w3.css">
<tana>

<div class="w3-konteyner w3-yashil">
   <h1>W3Schools demosi</h1>
   <p>Ushbu javob beruvchi sahifa hajmini o'zgartiring!</p>
</div>

<div class="w3-row-padding">
   <div class="w3-third">
     <h2>London</h2>
     <p>London - Angliyaning poytaxti.</p>
     <p>Bu Buyuk Britaniyadagi eng gavjum shahar,
     13 milliondan ortiq aholiga ega poytaxt hududi.</p>
   </div>

   <div class="w3-third">
     <h2>Parij</h2>
     <p>Parij - Fransiyaning poytaxti.</p>
     <p>Parij hududi Yevropadagi eng yirik aholi markazlaridan biri,
     12 milliondan ortiq aholiga ega.</p>
   </div>

   <div class="w3-third">
     <h2>Tokio</h2>
     <p>Tokio - Yaponiya poytaxti.</p>
     <p>Bu Katta Tokio hududining markazi,
     va dunyodagi eng gavjum metropolitan hudud.</p>
   </div>
</div>

</body>
</html>
```


** Bootstrap: veb-sahifalarni yaratish uchun HTML, CSS va JQuery-dan foydalanadigan boshqa ramka:
```
<!DOCTYPE html>
<html lang="en">
<head>
<title>Bootstrap misoli</title>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.4.1/css/bootstrap.min.css">
<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
<script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.4.1/js/bootstrap.min.js"></script>
</head>
<tana>

<div class="container">
   <div class="jumbotron">
     <h1>Mening birinchi yuklash sahifam</h1>
   </div>
   <div class="satr">
     <div class="col-sm-4">
       ...
     </div>
     <div class="col-sm-4">
       ...
     </div>
     <div class="col-sm-4">
     ...
     </div>
   </div>
</div>

</body>
</html>
```
<kbd>qaytish</kbd>[Mundarijaga qaytish](#homepage)


------


## HTML SEMANTIKA

HTML semantik elementlari

Semantik elementlar ma'noga ega bo'lgan elementlardir va bu ma'no brauzer va ishlab chiquvchi uchun tarkibni tavsiflaydi.

Semantik bo'lmagan element: ```<div>``` va ```<span>``` kontent haqida hech narsa aytmaydi

Semantik elementlar: ```<form>, <jadval> va <maqola>``` tarkibni belgilaydi
Saytlar odatda elementlarni belgilaydi:```<div id="nav"> <div class="header"> <div id="footer">``` navigatsiya, sarlavha va altbilgini ko'rsatish uchun.

* HTMLdagi emantik elementlar
```
<maqola>
<chetga>
<batafsil>
<figcaption>
<rasm>
<footer>
<sarlavha>
<asosiy>
<belgi>
<nav>
<bo'lim>
<xulosa>
<vaqt>
```

HTML ```<bo`lim>``` Element: Odatda sarlavhaga ega bo`lgan kontentni tematik guruhlash. Siz veb-sahifani kirish, tarkib va aloqa ma'lumotlari uchun bo'limlarga bo'lishingiz mumkin.
```
<bo'lim>
<h1>WWF</h1>
<p>Butunjahon tabiatni muhofaza qilish jamg'armasi (WWF) atrof-muhitni muhofaza qilish, tadqiq qilish va qayta tiklash masalalari bilan shug'ullanuvchi xalqaro tashkilot bo'lib, ilgari Jahon yovvoyi tabiat jamg'armasi deb nomlangan. WWF 1961 yilda tashkil etilgan.</p>
</bo'lim>

<bo'lim>
<h1>WWFning Panda belgisi</h1>
<p>Panda WWF ramziga aylandi. WWFning taniqli panda logotipi WWF tashkil etilgan yili Pekin hayvonot bog'idan London hayvonot bog'iga ko'chirilgan Chi Chi ismli pandadan kelib chiqqan.</p>
</bo'lim>
```


HTML ```<maqola>``` elementi

```<article>``` elementi mustaqil mustaqil tarkibni belgilaydi. Maqola mantiqiy bo'lishi va saytning qolgan qismidan mustaqil ravishda tarqatilishi kerak. Maqola elementi quyidagilarda ishlatilishi mumkin: Forum posti, Blog posti, Gazeta maqolasi.

* Maqola elementlaridan foydalanishga misol
```
<maqola>
<h2>Google Chrome</h2>
<p>Google Chrome — Google tomonidan ishlab chiqilgan, 2008 yilda chiqarilgan veb-brauzer. Chrome — bugungi kunda dunyodagi eng mashhur veb-brauzer!</p>
</maqola>

<maqola>
<h2>Mozilla Firefox</h2>
<p>Mozilla Firefox — Mozilla tomonidan ishlab chiqilgan ochiq manbali veb-brauzer. Firefox 2018-yil yanvar oyidan beri eng mashhur ikkinchi veb-brauzer bo‘ldi.</p>
</maqola>

<maqola>
<h2>Microsoft Edge</h2>
<p>Microsoft Edge — Microsoft tomonidan ishlab chiqilgan, 2015-yilda chiqarilgan veb-brauzer. Microsoft Edge Internet Explorer oʻrnini egalladi.</p>
</maqola>
```
* Maqola elementlarini uslublash uchun CSS-dan foydalanish:
```
<html>
<head>
<uslub>
.all-brauzerlar {
   chegara: 0;
   to'ldirish: 5px;
   fon rangi: och kulrang;
}

.all-brauzerlar > h1, .browser {
   chegara: 10px;
   to'ldirish: 5px;
}

.brauzer {
   fon: oq;
}

.brauzer > h2, p {
   chegara: 4px;
   shrift hajmi: 90%;
}
</style>
</head>
<tana>

<article class="barcha brauzerlar">
   <h1>Eng mashhur brauzerlar</h1>
   <article class="brauzer">
     <h2>Google Chrome</h2>
     <p>Google Chrome — Google tomonidan ishlab chiqilgan, 2008 yilda chiqarilgan veb-brauzer. Chrome — bugungi kunda dunyodagi eng mashhur veb-brauzer!</p>
   </maqola>
   <article class="brauzer">
     <h2>Mozilla Firefox</h2>
     <p>Mozilla Firefox — Mozilla tomonidan ishlab chiqilgan ochiq manbali veb-brauzer. Firefox 2018-yil yanvar oyidan beri eng mashhur ikkinchi veb-brauzer bo‘ldi.</p>
   </maqola>
   <article class="brauzer">
     <h2>Microsoft Edge</h2>
     <p>Microsoft Edge — Microsoft tomonidan ishlab chiqilgan, 2015-yilda chiqarilgan veb-brauzer. Microsoft Edge Internet Explorer oʻrnini egalladi.</p>
   </maqola>
</maqola>

</body>
</html>
```

```<maqola>``` ```<bo`lim>``` ichiga joylashtirish yoki aksincha.

```<article>``` elementi mustaqil mustaqil tarkibni, <section> elementi esa hujjatdagi bo`limni belgilaydi.

Siz ```<bo'lim>``` elementlarni o'z ichiga olgan ```<maqola>``` elementi va ```<article>``` elementlarni o`z ichiga olgan HTML sahifalarini topasiz.

```
<bo'lim>
```

HTML ```<header>``` elementi

```<header>```element kirish mazmuni yoki navigatsiya havolalari to`plami uchun konteynerni ifodalaydi va odatda bir yoki bir nechta ```<h1> -<h6>```, logotip yoki belgi, mualliflik ma`lumotlari va boshqalarni o`z ichiga oladi.

* Eslatma: Bitta HTML hujjatida bir nechta ```<header>``` elementlar bo`lishi mumkin. Biroq, ```<header>``` ```<footer>```, ```<adres>``` yoki boshqa ```<header>``` elementiga joylashtirilishi mumkin emas.

Sarlavhaga misol:
```
<maqola>
   <sarlavha>
     <h1>WWF nima qiladi?</h1>
     <p>WWF missiyasi:</p>
   </header>
   <p>WWF missiyasi - sayyoramizning tabiiy muhiti degradatsiyasini to'xtatish,
   va odamlar tabiat bilan uyg'unlikda yashaydigan kelajakni qurish.</p>
</maqola>
```


* HTML ```<footer>``` elementi

Ushbu element odatda o'z ichiga oladi
mualliflik ma'lumotlari
mualliflik huquqi haqida ma'lumot
bog'lanish uchun ma'lumot
sayt xaritasi
yuqori havolalarga qaytish
tegishli hujjatlar
* Bitta hujjatda bir nechta ```<footer>``` element bo`lishi mumkin


* Hujjatdagi kolontiter bo'limiga misollar
```
<footer>
   <p>Muallif: Xege Refsnes</p>
   <p><a href="mailto:hege@example.com">hege@example.com</a></p>
</footer>
```

HTML ```<nav>``` Element: Navigatsiya havolalari to`plamini belgilaydi.

```<nav>``` elementi navigatsiya havolalarining asosiy bloklari bo`lgan navigatsiya havolalari to`plamini belgilaydi. Shunday qilib, barcha havolalar uchun <nav> dan foydalanmasligingiz kerak.

Brauzerlar, masalan, nogiron foydalanuvchilar uchun ekranni o'qiydiganlar, ushbu elementdan ushbu kontentning dastlabki ko'rsatilishini o'tkazib yuborishni aniqlash uchun foydalanishi mumkin.

** Navigatsiya havolalari to'plami
```
<nav>
   <a href="/html/">HTML</a> |
   <a href="/css/">CSS</a> |
   <a href="/js/">JavaScript</a> |
   <a href="/jquery/">jQuery</a>
</nav>
```


HTML ```<chekka>``` elementi
Yon panel kabi joylashtirilgan kontentdan tashqari ba'zi tarkiblarni belgilaydi. <side> mazmuni atrofdagi tarkib bilan bilvosita bog'liq bo'lishi kerak.

```
<p>Men va oilam shu yozda The Epcot markaziga tashrif buyurdik. Ob-havo yaxshi edi va Epcot ajoyib edi! Men oilam bilan yozni ajoyib o'tkazdim!</p>

<chetga>
<h4>Epcot markazi</h4>
<p>Epcot - bu Walt Disney World Resortdagi qiziqarli attraksionlar, xalqaro pavilonlar, mukofotga sazovor bo'lgan otashinlar va mavsumiy maxsus tadbirlarni o'z ichiga olgan mavzuli park.</p>
</chetga>
```

* Yon elementni uslublash uchun CSS-dan foydalanish.
```
<html>
<head>
<uslub>
chetga {
   kengligi: 30%;
   padding-chap: 15px;
   chap chekka: 15px;
   suzuvchi: o'ng;
   shrift uslubi: kursiv;
   fon rangi: och kulrang;
}
</style>
</head>
<tana>

<p>Men va oilam shu yozda The Epcot markaziga tashrif buyurdik. Ob-havo yaxshi edi va Epcot ajoyib edi! Men oilam bilan yozni ajoyib o'tkazdim!</p>

<chetga>
<p>Epcot markazi - bu Walt Disney World Resortdagi qiziqarli attraksionlar, xalqaro pavilyonlar, mukofotga sazovor bo'lgan otashinlar va mavsumiy maxsus tadbirlarni o'z ichiga olgan mavzuli park.</p>
</chetga>

<p>Men va oilam shu yozda The Epcot markaziga tashrif buyurdik. Ob-havo yaxshi edi va Epcot ajoyib edi! Men oilam bilan yozni ajoyib o'tkazdim!</p>
<p>Men va oilam shu yozda The Epcot markaziga tashrif buyurdik. Ob-havo yaxshi edi va Epcot ajoyib edi! Men oilam bilan yozni ajoyib o'tkazdim!</p>

</body>
</html>

```

HTML ```<figure>``` va ```<figcaption>``` elementlari

```<figure>``` yorlig`i rasmlar, diagrammalar, fotosuratlar, kodlar ro`yxati va boshqalar kabi o`z-o`zidan tarkib topgan tarkibni belgilaydi.

```<figcaption>``` tegi ```<figure>``` elementi uchun sarlavhani belgilaydi. ```<figcaption>``` elementi ```<figure>``` elementining birinchi yoki oxirgi bolasi sifatida joylashtirilishi mumkin.

```<img>``` elementi haqiqiy tasvirni/illyustratsiyani belgilaydi.

* Rasm va rasm sarlavhasi uchun kod namunasi
```
<rasm>
   <img src="pic_trulli.jpg" alt="Trulli">
   <figcaption>1-rasm. - Trulli, Puglia, Italiya.</figcaption>
</figure>
```

* Semantik elementlarning mohiyati
W3C ga ko'ra: "Semantik Internet ma'lumotlarni ilovalar, korxonalar va jamoalar bo'ylab almashish va qayta foydalanish imkonini beradi."


HTMLdagi semantik elementlar

Quyida HTML tilidagi ba'zi semantik elementlarning ro'yxati keltirilgan.
```
Teg tavsifi
<maqola> Mustaqil, mustaqil tarkibni belgilaydi
<aside> Sahifa mazmunidan tashqari tarkibni belgilaydi
<details> Foydalanuvchi ko'rishi yoki yashirishi mumkin bo'lgan qo'shimcha ma'lumotlarni belgilaydi
<figcaption> <figure> elementi uchun sarlavhani belgilaydi
<figure> Illyustratsiyalar, diagrammalar, fotosuratlar, kodlar roʻyxati va h.k. kabi mustaqil tarkibni belgilaydi.
<footer> Hujjat yoki bo'lim uchun pastki ko'rsatkichni belgilaydi
<header> Hujjat yoki bo'lim uchun sarlavhani belgilaydi
<main> Hujjatning asosiy mazmunini belgilaydi
<belgi> Belgilangan/ta'kidlangan matnni belgilaydi
<nav> Navigatsiya havolalarini belgilaydi
<bo'lim> Hujjatdagi bo'limni belgilaydi
<xulosa> <details> elementi uchun ko'rinadigan sarlavhani belgilaydi
<time> Sana/vaqtni belgilaydi
```
<kbd>qaytish</kbd>[Mundarijaga qaytish](#homepage)


--------

## HTML EMOJIS

* HTMLda kulgichlardan foydalanish

Emojilar UTF-8 belgilar to‘plamidagi belgilar:

Ular tasvirlar yoki piktogrammalarga o'xshaydi, lekin unday emas. va ular UTF-8 (Unicode) belgilar to'plamidagi harflar (belgilar).

UTF-8 deyarli barcha mavjud belgilar va belgilarni qamrab oladi

<kbd>qaytish</kbd>[Mundarijaga qaytish](#homepage)


------


## CSS havolalari


CSS-dan foydalangan holda va CSS rang, shrift-familiya va shrift-familiya yordamida havolalarni shakllantirishning bir necha usullari mavjud.

fon xususiyatlari. Quyidagi misolga qarang:


<!DOCTYPE html>
<html>
<head>
<uslub>
a {
   rang: issiq pushti;
}
</style>
</head>
<tana>

<h2>CSS havolalari</h2>
<p><b><a href="default.asp" target="_blank">Bu havola</a></b></p>

</body>
</html>



Bundan tashqari, havolalar qaysi holatda ekanligiga qarab turlicha uslubda bo'lishi mumkin.

To'rtta havola holati quyidagilardir:

     a:link - oddiy, tashrif buyurilmagan havola
     a: tashrif buyurdi - foydalanuvchi tashrif buyurgan havola
     a: hover - foydalanuvchi ustiga sichqonchani bosganda havola
     a:faol - bosilgan paytdagi havola


Bir nechta havola holatlari uchun uslubni o'rnatishda ba'zi tartib qoidalari mavjud:

     a:hover a:link va a:visited dan keyin kelishi SHART
     a:active a:hoverdan keyin kelishi KERAK

<!DOCTYPE html>
<html>
<head>
<uslub>
/* tashrif buyurilmagan havola */
a: havola {
   rang: qizil;
}

/* tashrif buyurilgan havola */
a: tashrif buyurgan {
   rang: yashil;
}

/* sichqonchani havola ustiga bosing */
a: suring {
   rang: issiq pushti;
}

/* tanlangan havola */
a: faol {
   rang: ko'k;
}
</style>
</head>
<tana>

<h2>CSS havolalari</h2>
<p><b><a href="default.asp" target="_blank">Bu havola</a></b></p>
<p><b>Eslatma:</b> a:hover CSS taʼrifida a:link va a:visiteddan keyin kelishi KERAK boʻlishi uchun

samarali.</p>
<p><b>Eslatma:</b> a:active samarali bo'lishi uchun CSS ta'rifida a: kursordan keyin kelishi KERAK.</p>

</body>
</html>



Matnni bezatish:::
Bu ko'pincha havolalardan pastki chiziqni olib tashlash uchun ishlatiladi. Quyidagi misolga qarang:

<!DOCTYPE html>
<html>
<head>
<uslub>
a: havola {
   matn-bezak: yo'q;
}

a: tashrif buyurgan {
   matn-bezak: yo'q;
}

a: suring {
   matnni bezash: tagiga chizish;
}

a: faol {
   matnni bezash: tagiga chizish;
}
</style>
</head>
<tana>

<h2>CSS havolalari</h2>
<p><b><a href="default.asp" target="_blank">Bu havola</a></b></p>
<p><b>Eslatma:</b> a:hover CSS taʼrifida a:link va a:visiteddan keyin kelishi KERAK boʻlishi uchun

samarali.</p>
<p><b>Eslatma:</b> a:active samarali bo'lishi uchun CSS ta'rifida a: kursordan keyin kelishi KERAK.</p>

</body>
</html>




Fon rangi:::

Fon rangi xususiyati havolalar uchun fon rangini belgilash uchun ishlatilishi mumkin:

<!DOCTYPE html>
<html>
<head>
<uslub>
a: havola {
   fon rangi: sariq;
}

a: tashrif buyurgan {
   fon rangi: zangori;
}

a: suring {
   fon rangi: och yashil;
}

a: faol {
   fon rangi: issiq pushti;
}
</style>
</head>
<tana>

<h2>CSS havolalari</h2>
<p><b><a href="default.asp" target="_blank">Bu havola</a></b></p>
<p><b>Eslatma:</b> a:hover CSS taʼrifida a:link va a:visiteddan keyin kelishi KERAK boʻlishi uchun

samarali.</p>
<p><b>Eslatma:</b> a:active samarali bo'lishi uchun CSS ta'rifida a: kursordan keyin kelishi KERAK.</p>

</body>
</html>



Bog'lanish tugmalari:::

Quyidagi misollar yanada rivojlangan, chunki ular havolalarni qutilar shaklida ko'rsatish uchun turli CSS xususiyatlarini birlashtiradi.

tugmalar. Quyidagi misolga qarang:


<!DOCTYPE html>
<html>
<head>
<uslub>
a: havola, a: tashrif buyurgan {
   fon rangi: #f44336;
   rang: oq;
   to'ldirish: 14px 25px;
   matnni tekislash: markaz;
   matn-bezak: yo'q;
   displey: inline-block;
}

a: suring, a: faol {
   fon rangi: qizil;
}
</style>
</head>
<tana>

<h2>Ulanish tugmasi</h2>
<p>Tugma sifatida yaratilgan havola:</p>
<a href="default.asp" target="_blank">Bu havola</a>

</body>
</html>

CSS havolalarini uslublashning boshqa misollari

<!DOCTYPE html>
<html>
<head>
<uslub>
a.one: havola {rang:#ff0000;}
a.one:ziyorat qilingan {rang:#0000ff;}
a.one: hover {rang:#ffcc00;}

a.ikki: havola {rang:#ff0000;}
a.ikki:ziyorat qilingan {rang:#0000ff;}
a.ikki: hover {shrift o'lchami: 150%;}

a.uch: havola {rang:#ff0000;}
a.three:ziyorat qilingan {rang:#0000ff;}
a.uch: suring {fon:#66ff66;}

a.four:link {rang:#ff0000;}
a.four:ziyorat qilingan {rang:#0000ff;}
a.four: hover {font-family: monospace;}

a.five:link {rang:#ff0000;matn-bezatish:yo'q;}
a.besh: tashrif buyurilgan {rang:#0000ff;matn-bezatish:yo'q;}
a.five: suring {matn-bezatish: ostiga chizish;}
</style>
</head>
<tana>

<p>Sichqonchani havolalar ustiga bosing va ularning tartibini oʻzgartirishini tomosha qiling:</p>

<p><b><a class="one" href="default.asp" target="_blank">Ushbu havola rangini o'zgartiradi</a></b></p>
<p><b><a class="two" href="default.asp" target="_blank">Ushbu havola shrift hajmini o'zgartiradi</a></b></p>
<p><b><a class="three" href="default.asp" target="_blank">Bu havola fon rangini o'zgartiradi</a></b></p>
<p><b><a class="four" href="default.asp" target="_blank">Ushbu havola font-family-ni o'zgartiradi</a></b></p>
<p><b><a class="five" href="default.asp" target="_blank">Ushbu havola matn bezaklarini o'zgartiradi</a></b></p>

</body>
</html>


Yana bir misol

<!DOCTYPE html>
<html>
<head>
<uslub>
a: havola, a: tashrif buyurgan {
   fon rangi: oq;
   rang: qora;
   chegara: 2px qattiq yashil;
   to'ldirish: 10px 20px;
   matnni tekislash: markaz;
   matn-bezak: yo'q;
   displey: inline-block;
}

a: suring, a: faol {
   fon rangi: yashil;
   rang: oq;
}
</style>
</head>
<tana>

<a href="default.asp" target="_blank">Bu havola</a>

</body>
</html>





Havolalar uchun ishlatilishi mumkin bo'lgan turli xil kursorlar

<!DOCTYPE html>
<html>
<tana>

<p>Kursorni oʻzgartirish uchun sichqonchani soʻzlar ustiga bosing.</p>
<span style="cursor:auto">avtomatik</span><br>
<span style="cursor:crosshair">krossshair</span><br>
<span style="cursor:default">standart</span><br>
<span style="cursor:e-resize">e-resize</span><br>
<span style="cursor:help">yordam</span><br>
<span style="cursor:move">ko'chirish</span><br>
<span style="cursor:n-resize">n-resize</span><br>
<span style="cursor:ne-resize">ne-resize</span><br>
<span style="cursor:nw-resize">nw-resize</span><br>
<span style="cursor:pointer">ko'rsatkich</span><br>
<span style="cursor:progress">progress</span><br>
<span style="cursor:s-resize">s-resize</span><br>
<span style="cursor:se-resize">se-resize</span><br>
<span style="cursor:sw-resize">sw-resize</span><br>
<span style="cursor:text">matn</span><br>
<span style="cursor:w-resize">w-resize</span><br>
<span style="cursor:wait">kuting</span><br>

</body>
</html>

<kbd>qaytish</kbd>[Mundarijaga qaytish](#homepage)


---------


## CSS ro'yxatlari

HTML ro'yxatlari va CSS ro'yxati xususiyatlari


Tartibsiz ro'yxatlar (<ul>) va tartiblangan (<ol>) ro'yxatlar HTMLda ro'yxatlarning ikkita asosiy turidir. Tartibsiz ro'yxatlar

o'q bilan belgilanadi, tartiblangan ro'yxatlar esa raqamlar yoki harflar bilan belgilanadi.


CSS ro'yxati xususiyatlari sizga quyidagilarga imkon beradi:

     Buyurtma qilingan ro'yxatlar uchun turli xil ro'yxat element belgilarini o'rnating
     Tartibsiz ro'yxatlar uchun turli xil ro'yxat element belgilarini o'rnating
     Rasmni ro'yxat elementi belgisi sifatida o'rnating
     Ro'yxatlar va ro'yxat elementlariga fon ranglarini qo'shing



Turli xil ro'yxat elementi belgilari

Ro'yxat uslubi turi xususiyati ishlatiladigan ro'yxat elementi markerining turini belgilash uchun ishlatiladi. Masalan,

<!DOCTYPE html>
<html>
<head>
<uslub>
ul.a {
   ro'yxat uslubi turi: doira;
}

ul.b {
   ro'yxat uslubi turi: kvadrat;
}

ol.c {
   ro'yxat uslubi turi: yuqori rim;
}

eski {
   ro'yxat uslubi turi: pastki alfa;
}
</style>
</head>
<tana>

<h2>Roʻyxatlar</h2>
<p>Tartibsiz ro'yxatlarga misol:</p>
<ul class="a">
   <li>Qahva</li>
   <li>Choy</li>
   <li>Coca Cola</li>
</ul>

<ul class="b">
   <li>Qahva</li>
   <li>Choy</li>
   <li>Coca Cola</li>
</ul>

<p>Tartiblangan roʻyxatlarga misol:</p>
<ol class="c">
   <li>Qahva</li>
   <li>Choy</li>
   <li>Coca Cola</li>
</ol>

<ol class="d">
   <li>Qahva</li>
   <li>Choy</li>
   <li>Coca Cola</li>
</ol>

</body>
</html>


Eslatma: Ba'zi qiymatlar tartibsiz ro'yxatlar uchun, ba'zilari esa tartiblangan ro'yxatlar uchun.



Roʻyxat elementi belgisi sifatida tasvir

Ro'yxat uslubidagi rasm xususiyati tasvirni element ro'yxati belgisi sifatida tezlashtirish uchun ishlatiladi. Masalan; misol uchun,


<!DOCTYPE html>
<html>
<head>
<uslub>
ul {
   ro'yxat uslubidagi rasm: url('sqpurple.gif');
}
</style>
</head>
<tana>

<h2>CSS ro'yxatlari</h2>
<p>List-style-image xususiyati rasmni roʻyxat elementi belgisi sifatida belgilaydi:</p>

<ul>
   <li>Qahva</li>
   <li>Choy</li>
   <li>Coca Cola</li>
</ul>

</body>
</html>



Ro'yxat elementi belgilarini joylashtiring

Ro'yxat-modda belgilarining (o'q nuqtalari) joylashuvi list-style-position yordamida aniqlanadi.


"list-style-position: outside;" o'q nuqtalari ro'yxat elementidan tashqarida bo'lishini anglatadi. ning boshlanishi

ro'yxat elementining har bir satri vertikal ravishda tekislanadi. Bu standart:


"list-style-position: inside;" o'q nuqtalari ro'yxat elementi ichida bo'lishini anglatadi. Bir qismi sifatida

ro'yxat elementi, u matnning bir qismi bo'ladi va matnni boshida surish:



<!DOCTYPE html>
<html>
<head>
<uslub>
ul.a {
   ro'yxat uslubidagi pozitsiya: tashqarida;
}

ul.b {
   ro'yxat uslubidagi pozitsiya: ichkarida;
}
</style>
</head>
<tana>

<h1>Ro'yxat uslubidagi joylashuv xususiyati</h1>

<h2>list-style-position: tashqarida (standart):</h2>
<ul class="a">
   <li>Qahva - qovurilgan kofe donalaridan tayyorlanadigan qaynatilgan ichimlik.

Kofe o'simligi</li>
   <li>Choy - odatda o't barglari ustiga issiq yoki qaynoq suv quyib tayyorlanadigan xushbo'y ichimlik.

Camellia sinensis , vatani Osiyo</li>dan doimiy yashil buta (buta).
   <li>Coca-Cola - The Coca-Cola kompaniyasi tomonidan ishlab chiqarilgan gazlangan alkogolsiz ichimlik. Ichimlikning nomi ikkitaga ishora qiladi

kola yong'og'i (kofein manbai) va koka barglari bo'lgan asl ingredientlardan</li>
</ul>

<h2>ro'yxat uslubidagi pozitsiya: ichida:</h2>
<ul class="b">
   <li>Qahva - qovurilgan kofe donalaridan tayyorlanadigan qaynatilgan ichimlik.

Kofe o'simligi</li>
   <li>Choy - odatda o't barglari ustiga issiq yoki qaynoq suv quyib tayyorlanadigan xushbo'y ichimlik.

Camellia sinensis , vatani Osiyo</li>dan doimiy yashil buta (buta).
   <li>Coca-Cola - The Coca-Cola kompaniyasi tomonidan ishlab chiqarilgan gazlangan alkogolsiz ichimlik. Ichimlikning nomi ikkitaga ishora qiladi

kola yong'og'i (kofein manbai) va koka barglari bo'lgan asl ingredientlardan</li>
</ul>

</body>
</html>




Eslatma: Ro'yxat uslubidagi joylashuv uchun tashqi tekislash sukut bo'yicha hisoblanadi va bu holda ikkinchi harfdagi birinchi harf

Har bir o'q tarkibining satri to'g'ridan-to'g'ri birinchi qatordagi birinchi harf ostida. Biroq, ro'yxat qachon -

style-position ichkariga o'rnatiladi, ro'yxat elementidagi ikkinchi qatorning birinchi harfi to'g'ridan-to'g'ri ostidadir

birinchi qatordagi o'q belgisi.



Standart sozlamalarni olib tashlang

List-style-type:none xususiyatidan markerlarni/markerlarni olib tashlash uchun ham foydalanish mumkin. Ro'yxatni ham unutmang

standart chekka va toʻldirishga ega. Buni olib tashlash uchun <ul> yoki <ol> ga margin:0 va padding:0 qo'shing:

<!DOCTYPE html>
<html>
<head>
<uslub>
ul.demo {
   ro'yxat uslubi turi: yo'q;
   chegara: 0;
   to'ldirish: 0;
}
</style>
</head>
<tana>

<p>Birlamchi roʻyxat:</p>
<ul>
   <li>Qahva</li>
   <li>Choy</li>
   <li>Coca Cola</li>
</ul>

<p>Markalar, chekka va toʻldirishni olib tashlang:</p>
<ul class="demo">
   <li>Qahva</li>
   <li>Choy</li>
   <li>Coca Cola</li>
</ul>

</body>
</html>



Ro'yxat - Stenografiya xususiyati

Ro'yxat uslubidagi xususiyat stenografiya xususiyatidir. U barcha ro'yxat xususiyatlarini birida o'rnatish uchun ishlatiladi

deklaratsiya:


<!DOCTYPE html>
<html>
<head>
<uslub>
ul {
   ro'yxat uslubi: url ichida kvadrat ("sqpurple.gif");
}
</style>
</head>
<tana>

<h2>CSS ro'yxatlari</h2>
<p>Ro'yxat uslubidagi xususiyat stenografiya xususiyati bo'lib, u barcha ro'yxat xususiyatlarini bittada o'rnatish uchun ishlatiladi

deklaratsiya.</p>

<ul>
   <li>Qahva</li>
   <li>Choy</li>
   <li>Coca Cola</li>
</ul>

</body>
</html>



Qisqartirilgan xususiyatdan foydalanganda, xususiyat qiymatlarining tartibi quyidagicha:

1. roʻyxat uslubi turi (agar roʻyxat uslubi tasviri koʻrsatilgan boʻlsa, ushbu xususiyat qiymati koʻrsatiladi, agar

Ba'zi sabablarga ko'ra tasvirni ko'rsatib bo'lmaydi)
2. roʻyxat uslubidagi joylashuv (roʻyxat elementi belgilarining kontent ichida yoki tashqarisida koʻrinishini belgilaydi.

oqim)
3. roʻyxat uslubidagi tasvir (roʻyxat elementi belgisi sifatida tasvirni belgilaydi)

Yuqoridagi xususiyat qiymatlaridan biri etishmayotgan bo'lsa, etishmayotgan xususiyat uchun standart qiymat bo'ladi

agar mavjud bo'lsa, kiritilgan.


Ranglar bilan uslublar ro'yxati

Shuningdek, biz ro'yxatlarni biroz qiziqarliroq qilish uchun ranglar bilan bezashimiz mumkin.

<ol> yoki <ul> tegiga qo'shilgan har qanday narsa butun ro'yxatga ta'sir qiladi, <li> tegiga qo'shilgan xususiyatlar esa

alohida ro'yxat elementlariga ta'sir qiladi:

<!DOCTYPE html>
<html>
<head>
<uslub>
ol {
   fon: #ff9999;
   to'ldirish: 20px;
}

ul {
   fon: #3399ff;
   to'ldirish: 20px;
}

ol li {
   fon: #ffe5e5;
   to'ldirish: 5px;
   chap chekka: 35px;
}

ul li {
   fon: #cce5ff;
   chegara: 5px;
}
</style>
</head>
<tana>

<h1>Ranglar bilan uslublar roʻyxati:</h1>

<ol>
   <li>Qahva</li>
   <li>Choy</li>
   <li>Coca Cola</li>
</ol>

<ul>
   <li>Qahva</li>
   <li>Choy</li>
   <li>Coca Cola</li>
</ul>

</body>
</html>



Ko'proq misollar:

Chap qizil chegara bilan moslashtirilgan ro'yxat:


<!DOCTYPE html>
<html>
<head>
<uslub>
ul {
   chegara-chap: 5px qattiq qizil;
   fon rangi: #f1f1f1;
   ro'yxat uslubi turi: yo'q;
   to'ldirish: 10px 20px;
}
</style>
</head>
<tana>

<p>Chapdagi qizil hoshiyali roʻyxat:</p>
<ul>
   <li>Qahva</li>
   <li>Choy</li>
   <li>Coca Cola</li>
</ul>

</body>
</html>


To'liq kenglikdagi chegaralangan ro'yxat:

<!DOCTYPE html>
<html>
<head>
<uslub>
ul {
   ro'yxat uslubi turi: yo'q;
   to'ldirish: 0;
   chegara: 1px qattiq #ddd;
}

ul li {
   to'ldirish: 8px 16px;
   chegara-pastki: 1px qattiq #ddd;
}

ul li:oxirgi bola {
   chegara-pastki: yo'q
}
</style>
</head>
<tana>

<p>Toʻliq kenglikdagi chegaralangan roʻyxat:</p>
<ul>
   <li>Qahva</li>
   <li>Choy</li>
   <li>Coca Cola</li>
</ul>

</body>
</html>



Ro'yxatlar uchun barcha turli xil ro'yxat elementlari:


<!DOCTYPE html>
<html>
<head>
<uslub>
ul.a {ro'yxat uslubi turi: doira;}
ul.b {ro'yxat uslubi turi: disk;}
ul.c {ro'yxat uslubi turi: kvadrat;}

ol.d {ro'yxat uslubi turi: arman;}
ol.e {ro'yxat uslubi turi: cjk-ideografik;}
ol.f {ro'yxat uslubi turi: kasr;}
ol.g {ro'yxat uslubi turi: o'nlik bosh nol;}
ol.h {ro'yxat uslubi turi: gruzin;}
ol.i {ro'yxat uslubi turi: ibroniycha;}
ol.j {ro'yxat uslubi turi: hiragana;}
ol.k {ro'yxat uslubi turi: hiragana-iroha;}
ol.l {ro'yxat uslubi turi: katakana;}
ol.m {ro'yxat uslubi turi: katakana-iroha;}
ol.n {ro'yxat uslubi turi: pastki alfa;}
ol.o {ro'yxat uslubi turi: pastki yunoncha;}
ol.p {ro'yxat uslubi turi: pastki lotin;}
ol.q {ro'yxat uslubi turi: pastki roman;}
ol.r {ro'yxat uslubi turi: yuqori alfa;}
ol.s {ro'yxat uslubi turi: yuqori lotin;}
ol.t {ro'yxat uslubi turi: yuqori rim;}
ol.u {ro'yxat uslubi turi: yo'q;}
ol.v {ro'yxat uslubi turi: meros;}
</style>
</head>
<tana>

<ul class="a">
   <li>Dira turi</li>
   <li>Choy</li>
   <li>Coca Cola</li>
</ul>

<ul class="b">
   <li>Disk turi</li>
   <li>Choy</li>
   <li>Coca Cola</li>
</ul>

<ul class="c">
   <li>Kvadrat turi</li>
   <li>Choy</li>
   <li>Coca Cola</li>
</ul>

<ol class="d">
   <li>Armancha turi</li>
   <li>Choy</li>
   <li>Coca Cola</li>
</ol>

<ol class="e">
   <li>Cjk-ideografik turi</li>
   <li>Choy</li>
   <li>Coca Cola</li>
</ol>

<ol class="f">
   <li>O'nlik sanoq turi</li>
   <li>Choy</li>
   <li>Coca Cola</li>
</ol>

<ol class="g">
   <li>O'nlik-boshlovchi-nol turi</li>
   <li>Choy</li>
   <li>Coca Cola</li>
</ol>

<ol class="h">
   <li>Gruziya turi</li>
   <li>Choy</li>
   <li>Coca Cola</li>
</ol>

<ol class="i">
   <li>Ibroniycha turi</li>
   <li>Choy</li>
   <li>Coca Cola</li>
</ol>

<ol class="j">
   <li>Hiragana turi</li>
   <li>Choy</li>
   <li>Coca Cola</li>
</ol>

<ol class="k">
   <li>Hiragana-iroha turi</li>
   <li>Choy</li>
   <li>Coca Cola</li>
</ol>

<ol class="l">
   <li>Katakana turi</li>
   <li>Choy</li>
   <li>Coca Cola</li>
</ol>

<ol class="m">
   <li>Katakana-iroha turi</li>
   <li>Choy</li>
   <li>Coca Cola</li>
</ol>

<ol class="n">
   <li>Quyi alfa turi</li>
   <li>Choy</li>
   <li>Coca Cola</li>
</ol>

<ol class="o">
   <li>Quyi yunoncha turi</li>
   <li>Choy</li>
   <li>Coca Cola</li>
</ol>

<ol class="p">
   <li>Quyi lotincha turi</li>
   <li>Choy</li>
   <li>Coca Cola</li>
</ol>

<ol class="q">
   <li>Quyi rim turi</li>
   <li>Choy</li>
   <li>Coca Cola</li>
</ol>

<ol class="r">
   <li>Yuqori alfa turi</li>
   <li>Choy</li>
   <li>Coca Cola</li>
</ol>

<ol class="s">
   <li>Yuqori lotincha turi</li>
   <li>Choy</li>
   <li>Coca Cola</li>
</ol>

<ol class="t">
   <li>Yuqori rim turi</li>
   <li>Choy</li>
   <li>Coca Cola</li>
</ol>

<ol class="u">
   <li>Hech qanday tur</li>
   <li>Choy</li>
   <li>Coca Cola</li>
</ol>

<ol class="v">
   <li>turni meros qilib olish</li>
   <li>Choy</li>
   <li>Coca Cola</li>
</ol>

</body>
</html>

<kbd>qaytish</kbd>[Mundarijaga qaytish](#homepage)


-------



## CSS jadvallari

CSS HTML jadvallarining ko'rinishini yaxshilashga yordam beradi


Jadvalning namunasi quyida ko'rsatilgan:

<!DOCTYPE html>
<html>
<head>
<uslub>
#xaridorlar {
   shrift oilasi: Arial, Helvetica, sans-serif;
   chegara-burilish: qulash;
   kengligi: 100%;
}

#mijozlar td, #mijozlar th {
   chegara: 1px qattiq #ddd;
   to'ldirish: 8px;
}

#mijozlar tr:n-child(hatto){fon rangi: #f2f2f2;}

#customers tr:hover {fon rangi: #ddd;}

#mijozlar th {
   to'ldirish tepasi: 12px;
   to'ldirish-pastki: 12px;
   matnni tekislash: chapga;
   fon rangi: #04AA6D;
   rang: oq;
}
</style>
</head>
<tana>

<table id="mijozlar">
   <tr>
     <th>Kompaniya</th>
     <th>Aloqa</th>
     <th>Mamlakat</th>
   </tr>
   <tr>
     <td>Alfreds Futterkiste</td>
     <td>Mariya Anders</td>
     <td>Germaniya</td>
   </tr>
   <tr>
     <td>Berglunds snabbköp</td>
     <td>Kristina Berglund</td>
     <td>Shvetsiya</td>
   </tr>
   <tr>
     <td>Markaziy tijorat Moctezuma</td>
     <td>Fransisko Chang</td>
     <td>Meksika</td>
   </tr>
   <tr>
     <td>Ernst Handel</td>
     <td>Roland Mendel</td>
     <td>Avstriya</td>
   </tr>
   <tr>
     <td>Orol savdosi</td>
     <td>Xelen Bennet</td>
     <td>Buyuk Britaniya</td>
   </tr>
   <tr>
     <td>Königlich Essen</td>
     <td>Filip Kramer</td>
     <td>Germaniya</td>
   </tr>
   <tr>
     <td>Kulayotgan Bacchus vinocellars</td>
     <td>Yoshi Tannamuri</td>
     <td>Kanada</td>
   </tr>
   <tr>
     <td>Magazzini Alimentari Riuniti</td>
     <td>Jiovanni Rovelli</td>
     <td>Italiya</td>
   </tr>
   <tr>
     <td>Shimoliy/Janubiy</td>
     <td>Simon Krouter</td>
     <td>Buyuk Britaniya</td>
   </tr>
   <tr>
     <td>Paris spécialités</td>
     <td>Mari Bertran</td>
     <td>Frantsiya</td>
   </tr>
</jadval>

</body>
</html>




Jadval chegaralari


Jadval chegaralari

CSS-da jadval chegaralarini belgilash uchun border xususiyatidan foydalaning.

Quyidagi misol <table>, <th> va <td> elementlari uchun qora chegarani belgilaydi:


<!DOCTYPE html>
<html>
<head>
<uslub>
jadval, th, td {
   chegara: 1px qattiq qora;
}
</style>
</head>
<tana>

<h2>Jadvalga chegara qo'shish:</h2>

<jadval>
   <tr>
     <th>Ism</th>
     <th>Familiya</th>
   </tr>
   <tr>
     <td>Piter</td>
     <td>Griffin</td>
   </tr>
   <tr>
     <td>Lois</td>
     <td>Griffin</td>
   </tr>
</jadval>

</body>
</html>



To'liq kenglik jadvali:


Agar siz butun ekranni qamrab oladigan jadval yaratmoqchi bo'lsangiz (to'liq kenglik), <jadval> ga kenglik:100% qo'shing.
  element quyida ko'rsatilganidek:



<!DOCTYPE html>
<html>
<head>
<uslub>
jadval, th, td {
   chegara: 1px qattiq qora;
}

stol {
   kengligi: 100%;
}
</style>
</head>
<tana>

<h2>To'liq kenglikdagi jadval</h2>

<jadval>
   <tr>
     <th>Ism</th>
     <th>Familiya</th>
   </tr>
   <tr>
     <td>Piter</td>
     <td>Griffin</td>
   </tr>
   <tr>
     <td>Lois</td>
     <td>Griffin</td>
   </tr>
</jadval>

</body>
</html>




Ikki tomonlama chegaralar

E'tibor bering, yuqoridagi misollardagi jadval ikkita chegaraga ega. Buning sababi ham jadval, ham <th>

va <td> elementlari alohida chegaralarga ega.

Ikki tomonlama chegaralarni olib tashlash uchun quyidagi misolni ko'rib chiqing.




<!DOCTYPE html>
<html>
<head>
<uslub>
jadval, td, th {
   chegara: 1px qattiq qora;
}

stol {
   kengligi: 100%;
   chegara-burilish: qulash;
}
</style>
</head>
<tana>

<h2>Chegaralar siqilsin</h2>

<jadval>
   <tr>
     <th>Ism</th>
     <th>Familiya</th>
   </tr>
   <tr>
     <td>Piter</td>
     <td>Griffin</td>
   </tr>
   <tr>
     <td>Lois</td>
     <td>Griffin</td>
   </tr>
</jadval>

</body>
</html>



Jadval atrofida faqat chegarasi bo'lgan jadval yaratish uchun faqat <table> uchun chegara xususiyatini belgilang


<!DOCTYPE html>
<html>
<head>
<uslub>
stol {
   kengligi: 100%;
   chegara-burilish: qulash;
   chegara: 1px qattiq qora;
}
</style>
</head>
<tana>

<h2>Stol atrofidagi yagona chegara</h2>

<jadval>
   <tr>
     <th>Ism</th>
     <th>Familiya</th>
   </tr>
   <tr>
     <td>Piter</td>
     <td>Griffin</td>
   </tr>
   <tr>
     <td>Lois</td>
     <td>Griffin</td>
   </tr>
</jadval>

</body>
</html>



Jadval hajmi

Jadvalning kengligi va balandligi

Jadvalning kengligi va balandligi kenglik va balandlik xususiyatlari bilan belgilanadi.

Quyidagi misol jadvalning kengligini 100% va <th> elementlarning balandligini 70px ga o'rnatadi:



<!DOCTYPE html>
<html>
<head>
<uslub>
jadval, td, th {
   chegara: 1px qattiq qora;
}

stol {
   chegara-burilish: qulash;
   kengligi: 100%;
}

n {
   balandligi: 70px;
}
</style>
</head>
<tana>

<h2>Keniklik va balandlik xususiyatlari</h2>
<p>Jadvalning kengligi va sarlavha satrining balandligini belgilang:</p>

<jadval>
   <tr>
     <th>Ism</th>
     <th>Familiya</th>
     <th>Tejamkorlik</th>
   </tr>
   <tr>
     <td>Piter</td>
     <td>Griffin</td>
     <td>$100</td>
   </tr>
   <tr>
     <td>Lois</td>
     <td>Griffin</td>
     <td>$150</td>
   </tr>
   <tr>
     <td>Jo</td>
     <td>Swanson</td>
     <td>300$</td>
   </tr>
   <tr>
     <td>Klivlend</td>
     <td>Jigarrang</td>
     <td>$250</td>
   </tr>
</jadval>

</body>
</html>



Sahifaning faqat yarmini qamrab oladigan jadval yaratish uchun width:50% spetsifikatsiyasidan foydalaning. Rasmga qarang

quyida:


<!DOCTYPE html>
<html>
<head>
<uslub>
jadval, td, th {
   chegara: 1px qattiq qora;
}

stol {
   chegara-burilish: qulash;
   kengligi: 50%;
}

n {
   balandligi: 70px;
}
</style>
</head>
<tana>

<h2>Keniklik va balandlik xususiyatlari</h2>
<p>Jadvalning kengligi va sarlavha satrining balandligini belgilang:</p>

<jadval>
   <tr>
     <th>Ism</th>
     <th>Familiya</th>
     <th>Tejamkorlik</th>
   </tr>
   <tr>
     <td>Piter</td>
     <td>Griffin</td>
     <td>$100</td>
   </tr>
   <tr>
     <td>Lois</td>
     <td>Griffin</td>
     <td>$150</td>
   </tr>
   <tr>
     <td>Jo</td>
     <td>Swanson</td>
     <td>300$</td>
   </tr>
   <tr>
     <td>Klivlend</td>
     <td>Jigarrang</td>
     <td>$250</td>
   </tr>
</jadval>

</body>
</html>


CSS jadvalini tekislash::

Gorizontal tekislash

Matnni tekislash xususiyati <th>-dagi kontentning gorizontal tekislanishini (masalan, chap, o'ng yoki markaz) o'rnatadi.

yoki <td>.

Odatiy bo'lib, <th> elementlarning mazmuni markazga hizalanadi va <td> elementlarning mazmuni chap-

tekislangan.

<td> elementlari tarkibini ham markazga tekislash uchun text-align: center dan foydalaning:



<!DOCTYPE html>
<html>
<head>
<uslub>
jadval, td, th {
   chegara: 1px qattiq qora;
}

stol {
   chegara-burilish: qulash;
   kengligi: 100%;
}

td {
   matnni tekislash: markaz;
}
</style>
</head>
<tana>

<h2>Matnni tekislash xususiyati</h2>
<p>Bu xususiyat th yoki td.dagi kontentning gorizontal tekislanishini (masalan, chap, oʻng yoki markaz) oʻrnatadi.</p>

<jadval>
   <tr>
     <th>Ism</th>
     <th>Familiya</th>
     <th>Tejamkorlik</th>
   </tr>
   <tr>
     <td>Piter</td>
     <td>Griffin</td>
     <td>$100</td>
   </tr>
   <tr>
     <td>Lois</td>
     <td>Griffin</td>
     <td>$150</td>
   </tr>
   <tr>
     <td>Jo</td>
     <td>Swanson</td>
     <td>300$</td>
   </tr>
   <tr>
     <td>Klivlend</td>
     <td>Jigarrang</td>
     <td>$250</td>
   </tr>
</jadval>

</body>
</html>



Kontentni chap tomonga tekislash uchun <th> elementlarni matnni tekislash bilan chapga tekislashni majburlang:

chap mulk:


<!DOCTYPE html>
<html>
<head>
<uslub>
jadval, td, th {
   chegara: 1px qattiq qora;
}

stol {
   chegara-burilish: qulash;
   kengligi: 100%;
}

n {
   matnni tekislash: chapga;
}
</style>
</head>
<tana>

<h2>Matnni tekislash xususiyati</h2>
<p>Bu xususiyat th yoki td.dagi kontentning gorizontal tekislanishini (masalan, chap, oʻng yoki markaz) oʻrnatadi.</p>

<jadval>
   <tr>
     <th>Ism</th>
     <th>Familiya</th>
     <th>Tejamkorlik</th>
   </tr>
   <tr>
     <td>Piter</td>
     <td>Griffin</td>
     <td>$100</td>
   </tr>
   <tr>
     <td>Lois</td>
     <td>Griffin</td>
     <td>$150</td>
   </tr>
   <tr>
     <td>Jo</td>
     <td>Swanson</td>
     <td>300$</td>
   </tr>
   <tr>
     <td>Klivlend</td>
     <td>Jigarrang</td>
     <td>$250</td>
   </tr>
</jadval>

</body>
</html>



Vertikal tekislash


Vertical-align xususiyati <th>-dagi kontentning vertikal tekislanishini (masalan, yuqori, pastki yoki o'rta) o'rnatadi.

yoki <td>. Odatiy bo'lib, jadvaldagi tarkibning vertikal hizalanishi o'rtada (<th> va <td> uchun).

elementlar).

Quyidagi misol <td> elementlari uchun vertikal matnni pastga tekislashni o'rnatadi:

<!DOCTYPE html>
<html>
<head>
<uslub>
jadval, td, th {
   chegara: 1px qattiq qora;
}

stol {
   chegara-burilish: qulash;
   kengligi: 100%;
}

td {
   balandligi: 50px;
   vertikal tekislash: pastki;
}
</style>
</head>
<tana>

<h2>Vertikal tekislash xususiyati</h2>
<p>Bu xususiyat th yoki td.dagi kontentning vertikal tekislanishini (masalan, yuqori, pastki yoki oʻrta) oʻrnatadi.</p>
<jadval>
   <tr>
     <th>Ism</th>
     <th>Familiya</th>
     <th>Tejamkorlik</th>
   </tr>
   <tr>
     <td>Piter</td>
     <td>Griffin</td>
     <td>$100</td>
   </tr>
   <tr>
     <td>Lois</td>
     <td>Griffin</td>
     <td>$150</td>
   </tr>
   <tr>
     <td>Jo</td>
     <td>Swanson</td>
     <td>300$</td>
   </tr>
   <tr>
     <td>Klivlend</td>
     <td>Jigarrang</td>
     <td>$250</td>
   </tr>
</jadval>

</body>
</html>


CSS jadval uslubi

Jadvalni to'ldirish

Jadvaldagi chegara va tarkib o'rtasidagi bo'shliqni boshqarish uchun <td> va padding xususiyatidan foydalaning

<th> elementlar:

<!DOCTYPE html>
<html>
<head>
<uslub>
jadval, td, th {
   chegara: 1px qattiq #ddd;
   matnni tekislash: chapga;
}

stol {
   chegara-burilish: qulash;
   kengligi: 100%;
}

th, td {
   to'ldirish: 15px;
}
</style>
</head>
<tana>

<h2>To'ldirish xususiyati</h2>
<p>Bu xususiyat chegara va jadval tarkibi oʻrtasida boʻsh joy qoʻshadi.</p>

<jadval>
   <tr>
     <th>Ism</th>
     <th>Familiya</th>
     <th>Tejamkorlik</th>
   </tr>
   <tr>
     <td>Piter</td>
     <td>Griffin</td>
     <td>$100</td>
   </tr>
   <tr>
     <td>Lois</td>
     <td>Griffin</td>
     <td>$150</td>
   </tr>
   <tr>
     <td>Jo</td>
     <td>Swanson</td>
     <td>300$</td>
   </tr>
   <tr>
     <td>Klivlend</td>
     <td>Jigarrang</td>
     <td>$250</td>
   </tr>
</jadval>

</body>
</html>



Gorizontal ajratgichlar

Gorizontal bo'linishlar uchun border-bottom xususiyatini <th> va <td> ga qo'shing:


<!DOCTYPE html>
<html>
<head>
<uslub>
stol {
   chegara-burilish: qulash;
   kengligi: 100%;
}

th, td {
   to'ldirish: 8px;
   matnni tekislash: chapga;
   chegara-pastki: 1px qattiq #ddd;
}
</style>
</head>
<tana>

<h2>Chegaralangan jadval bo'linuvchilari</h2>
<p>Gorizontal ajratuvchilar uchun th va td ga border-bottom xususiyatini qo'shing:</p>

<jadval>
   <tr>
     <th>Ism</th>
     <th>Familiya</th>
   <th>Tejamkorlik</th>
   </tr>
   <tr>
     <td>Piter</td>
     <td>Griffin</td>
     <td>$100</td>
   </tr>
   <tr>
     <td>Lois</td>
     <td>Griffin</td>
     <td>$150</td>
   </tr>
   <tr>
     <td>Jo</td>
     <td>Swanson</td>
     <td>300$</td>
   </tr>
   <tr>
     <td>Klivlend</td>
     <td>Jigarrang</td>
     <td>$250</td>
   </tr>
</jadval>

</body>
</html>





Harakatlanuvchi stol

Sichqoncha ustidagi jadval qatorlarini ajratib ko'rsatish uchun <tr> da :hover selektoridan foydalaning:



<!DOCTYPE html>
<html>
<head>
<uslub>
stol {
   chegara-burilish: qulash;
   kengligi: 100%;
}

th, td {
   to'ldirish: 8px;
   matnni tekislash: chapga;
   chegara-pastki: 1px qattiq #ddd;
}

tr: hover {fon rangi: sariq;}
</style>
</head>
<tana>

<h2>Ko'chma jadval</h2>
<p>Effektni ko'rish uchun sichqonchani jadval qatorlari ustiga olib boring.</p>

<jadval>
   <tr>
     <th>Ism</th>
     <th>Familiya</th>
     <th>Bollar</th>
   </tr>
   <tr>
     <td>Piter</td>
     <td>Griffin</td>
     <td>$100</td>
   </tr>
   <tr>
     <td>Lois</td>
     <td>Griffin</td>
     <td>$150</td>
   </tr>
   <tr>
     <td>Jo</td>
     <td>Swanson</td>
     <td>300$</td>
   </tr>
   <tr>
     <td>Klivlend</td>
     <td>Jigarrang</td>
     <td>$250</td>
   </tr>
</jadval>

</body>
</html>



Chiziqli stollar

Zebra chiziqli jadvallar uchun nth-child() selektoridan foydalaning va barcha juft (yoki toq) jadvalga fon rangini qo'shing.

qatorlar:

birinchi qator sarlavha (<th> bilan toq boshlanuvchi)



<!DOCTYPE html>
<html>
<head>
<uslub>
stol {
   chegara-burilish: qulash;
   kengligi: 100%;
}

th, td {
   matnni tekislash: chapga;
   to'ldirish: 8px;
}

tr:nth-child(juft) {fon rangi: #f2f2f2;}
</style>
</head>
<tana>

<h2>Chiziqli stol</h2>
<p>Zebra chiziqli jadvallar uchun nth-child() selektoridan foydalaning va barcha juft (yoki toq) uchun fon rangini qo'shing.

jadval qatorlari:</p>

<jadval>
   <tr>
   <th>Ism</th>
   <th>Familiya</th>
   <th>Bollar</th>
   </tr>
   <tr>
   <td>Piter</td>
   <td>Griffin</td>
   <td>$100</td>
   </tr>
   <tr>
   <td>Lois</td>
   <td>Griffin</td>
   <td>$150</td>
   </tr>
   <tr>
   <td>Jo</td>
   <td>Swanson</td>
   <td>300$</td>
   </tr>
   <tr>
   <td>Klivlend</td>
   <td>Jigarrang</td>
   <td>$250</td>
   </tr>
</jadval>

</body>
</html>




Jadval rangi

Quyidagi misol <th> elementlarning fon rangi va matn rangini belgilaydi:

<!DOCTYPE html>
<html>
<head>
<uslub>
stol {
   chegara-burilish: qulash;
   kengligi: 100%;
}

th, td {
   matnni tekislash: chapga;
   to'ldirish: 8px;
}

tr:nth-child(juft){fon rangi: #f2f2f2}

n {
   fon rangi: #04AA6D;
   rang: oq;
}
</style>
</head>
<tana>

<h2>Rangli jadval sarlavhasi</h2>

<jadval>
   <tr>
     <th>Ism</th>
     <th>Familiya</th>
     <th>Tejamkorlik</th>
   </tr>
   <tr>
     <td>Piter</td>
     <td>Griffin</td>
     <td>$100</td>
   </tr>
   <tr>
     <td>Lois</td>
     <td>Griffin</td>
     <td>$150</td>
   </tr>
   <tr>
     <td>Jo</td>
     <td>Swanson</td>
     <td>300$</td>
   </tr>
   <tr>
     <td>Klivlend</td>
     <td>Jigarrang</td>
     <td>$250</td>
</tr>
</jadval>

</body>
</html>




CSS javob beruvchi jadvali

Javob beruvchi jadval

Agar ekran to'liq ko'rsatish uchun juda kichik bo'lsa, sezgir jadval gorizontal aylantirish panelini ko'rsatadi

tarkibi:

Konteyner elementini (masalan, <div>) sezgir qilish uchun <table> elementi atrofida overflow-x:auto bilan qo'shing:


Eslatma: OS X Lion-da (Mac-da) aylantirish panellari sukut bo'yicha yashiriladi va faqat foydalanilganda ko'rsatiladi (garchi bo'lsa ham)

"overflow: scroll" o'rnatilgan).

<!DOCTYPE html>
<html>
<head>
<uslub>
stol {
   chegara-burilish: qulash;
   kengligi: 100%;
}

th, td {
   matnni tekislash: chapga;
   to'ldirish: 8px;
}

tr:nth-child(juft) {fon rangi: #f2f2f2;}
</style>
</head>
<tana>

<h2>Javob beruvchi jadval</h2>
<p>Agar ekran ham bo'lsa, javob beruvchi jadval gorizontal aylantirish panelini ko'rsatadi
to'liq tarkibni ko'rsatish uchun kichik. Effektni ko'rish uchun brauzer oynasining o'lchamini o'zgartiring:</p>
<p>Restiv jadval yaratish uchun <strong>overflow-x:auto</strong> bilan konteyner elementini (masalan, div) qo‘shing.

jadval elementi atrofida:</p>

<div style="overflow-x:auto;">
   <jadval>
     <tr>
       <th>Ism</th>
       <th>Familiya</th>
       <th>Bollar</th>
       <th>Bollar</th>
       <th>Bollar</th>
       <th>Bollar</th>
       <th>Bollar</th>
       <th>Bollar</th>
       <th>Bollar</th>
       <th>Bollar</th>
       <th>Bollar</th>
       <th>Bollar</th>
     </tr>
     <tr>
       <td>Jill</td>
       <td>Smit</td>
       <td>50</td>
       <td>50</td>
       <td>50</td>
       <td>50</td>
       <td>50</td>
       <td>50</td>
       <td>50</td>
       <td>50</td>
       <td>50</td>
       <td>50</td>
     </tr>
     <tr>
       <td>Havo</td>
       <td>Jekson</td>
       <td>94</td>
       <td>94</td>
       <td>94</td>
       <td>94</td>
       <td>94</td>
       <td>94</td>
       <td>94</td>
       <td>94</td>
       <td>94</td>
       <td>94</td>
     </tr>
     <tr>
       <td>Odam</td>
       <td>Jonson</td>
       <td>67</td>
       <td>67</td>
       <td>67</td>
       <td>67</td>
       <td>67</td>
       <td>67</td>
       <td>67</td>
       <td>67</td>
       <td>67</td>
       <td>67</td>
     </tr>
   </jadval>
</div>

</body>
</html>



Ko'proq jadval misollari:


Chiroyli stol yasash uchun


<!DOCTYPE html>
<html>
<head>
<uslub>
#xaridorlar {
   shrift oilasi: Arial, Helvetica, sans-serif;
   chegara-burilish: qulash;
   kengligi: 100%;
}

#mijozlar td, #mijozlar th {
   chegara: 1px qattiq #ddd;
   to'ldirish: 8px;
}

#mijozlar tr:n-child(hatto){fon rangi: #f2f2f2;}

#customers tr:hover {fon rangi: #ddd;}

#mijozlar th {
   to'ldirish tepasi: 12px;
   to'ldirish-pastki: 12px;
   matnni tekislash: chapga;
   fon rangi: #04AA6D;
   rang: oq;
}
</style>
</head>
<tana>

<table id="mijozlar">
   <tr>
     <th>Kompaniya</th>
     <th>Aloqa</th>
     <th>Mamlakat</th>
   </tr>
   <tr>
     <td>Alfreds Futterkiste</td>
     <td>Mariya Anders</td>
     <td>Germaniya</td>
   </tr>
   <tr>
     <td>Berglunds snabbköp</td>
     <td>Kristina Berglund</td>
     <td>Shvetsiya</td>
   </tr>
   <tr>
     <td>Markaziy tijorat Moctezuma</td>
     <td>Fransisko Chang</td>
     <td>Meksika</td>
   </tr>
   <tr>
     <td>Ernst Handel</td>
     <td>Roland Mendel</td>
     <td>Avstriya</td>
   </tr>
   <tr>
     <td>Orol savdosi</td>
     <td>Xelen Bennet</td>
     <td>Buyuk Britaniya</td>
   </tr>
   <tr>
     <td>Königlich Essen</td>
     <td>Filip Kramer</td>
     <td>Germaniya</td>
   </tr>
   <tr>
     <td>Kulayotgan Bacchus vinocellars</td>
     <td>Yoshi Tannamuri</td>
     <td>Kanada</td>
   </tr>
   <tr>
     <td>Magazzini Alimentari Riuniti</td>
     <td>Jiovanni Rovelli</td>
     <td>Italiya</td>
   </tr>
   <tr>
     <td>Shimoliy/Janubiy</td>
     <td>Simon Krouter</td>
     <td>Buyuk Britaniya</td>
   </tr>
   <tr>
     <td>Paris spécialités</td>
     <td>Mari Bertran</td>
     <td>Frantsiya</td>
   </tr>
</jadval>

</body>
</html>




Jadval sarlavhasi o'rnini o'rnatish uchun

<!DOCTYPE html>
<html>
<head>
<uslub>
jadval, td, th {
   chegara: 1px qattiq qora;
}

sarlavha {
   sarlavha tomoni: pastki;
}
</style>
</head>
<tana>

<jadval>
<caption>1.1-jadval mijozlar</caption>
   <tr>
     <th>Kompaniya</th>
     <th>Aloqa</th>
     <th>Mamlakat</th>
   </tr>
   <tr>
     <td>Alfreds Futterkiste</td>
     <td>Mariya Anders</td>
     <td>Germaniya</td>
   </tr>
   <tr class="alt">
     <td>Berglunds snabbköp</td>
     <td>Kristina Berglund</td>
     <td>Shvetsiya</td>
   </tr>
   <tr>
     <td>Markaziy tijorat Moctezuma</td>
     <td>Fransisko Chang</td>
     <td>Meksika</td>
   </tr>
   <tr class="alt">
     <td>Ernst Handel</td>
     <td>Roland Mendel</td>
     <td>Avstriya</td>
   </tr>
   <tr>
     <td>Orol savdosi</td>
     <td>Xelen Bennet</td>
     <td>Buyuk Britaniya</td>
   </tr>
</jadval>

</body>
</html>

<kbd>qaytish</kbd>[Mundarijaga qaytish](#homepage)


--------





## CSS pozitsiyasi

CSS Layout - joylashuv xususiyati

Pozitsiya xususiyati elementning joylashuvi statik, nisbiy, sobit,

mutlaq yoki yopishqoq. Keyin elementlar yuqori, pastki, chap va o'ng xususiyatlaridan foydalangan holda joylashtiriladi (bular

xususiyatlar faqat pozitsiya xususiyati birinchi marta o'rnatilgandan keyin ishlaydi). Bu xususiyatlar qarab har xil ishlaydi

CSS pozitsiyasi o'rnatilgan.



pozitsiyasi: statik; ::

Statik joylashuv barcha HTML elementlari uchun standart hisoblanadi. Statik joylashtirilgan element yuqoridan ta'sirlanmaydi

pastki, chap va o'ng xususiyatlari. Ular maxsus tarzda joylashtirilmaydi, balki odatdagiga amal qiladi

sahifa oqimi. Pozitsiyadan foydalanish tasviriga qarang;statik; quyida.

<!DOCTYPE html>
<html>
<head>
<uslub>
div.static {
   pozitsiyasi: statik;
   chegara: 3px qattiq #73AD21;
}
</style>
</head>
<tana>

<h2>pozitsiya: statik;</h2>

<p>Pozitsiyaga ega element: statik; hech qanday maxsus tarzda joylashtirilmaydi; bu
har doim sahifaning normal oqimiga ko'ra joylashtirilgan:</p>

<div class="statik">
   Ushbu div elementi pozitsiyasiga ega: statik;
</div>

</body>
</html>



pozitsiya: nisbiy; ::

Nisbatan joylashuv xususiyati elementni normal holatiga nisbatan joylashtirish imkonini beradi. Sozlama

joylashuvi bilan elementning yuqori, o'ng, pastki va chap xususiyatlari: nisbiy; dan bunday elementni rostlaydi

uning normal holati. Qolgan tarkib element tomonidan qoldirilgan bo'shliqni egallamaydi. Rasmga qarang

quyida:


<!DOCTYPE html>
<html>
<head>
<uslub>
div.nisbiy {
   pozitsiya: nisbiy;
   chap: 30px;
   chegara: 3px qattiq #73AD21;
}
</style>
</head>
<tana>

<h2>pozitsiya: nisbiy;</h2>

<p>Pozitsiyaga ega element: nisbiy; normal holatiga nisbatan joylashtirilgan:</p>

<div class="relative">
Ushbu div elementi pozitsiyaga ega: nisbiy;
</div>

</body>
</html>




Eslatma: chap: 30px; elementni asl joyidan 30px uzoqda joylashtiring (30px oʻngga siljiydi).




pozitsiyasi: qattiq; ::

Bu ko'rish oynasiga nisbatan elementni joylashtirish imkonini beradi; element sahifa bo'lsa ham bir joyda qoladi

aylantiriladi. Ruxsat etilgan element sahifada odatda joylashgan joyda bo'sh joy qoldirmaydi.

Yuqori, o'ng, pastki va chap xususiyatlar elementni joylashtirish uchun ishlatiladi.


Quyidagi misolga qarang:


<!DOCTYPE html>
<html>
<head>
<uslub>
div.fixed {
   pozitsiyasi: qattiq;
   pastki: 0;
   o'ng: 0;
   kengligi: 300px;
   chegara: 3px qattiq #73AD21;
}
</style>
</head>
<tana>

<h2>pozitsiya: belgilangan;</h2>

<p>Pozitsiyaga ega element: belgilangan; ko'rish oynasiga nisbatan joylashtirilgan, ya'ni u doimo ichida qoladi

sahifa aylantirilsa ham bir xil joy:</p>

<div class="tuzatildi">
Ushbu div elementi pozitsiyaga ega: fixed;
</div>

</body>
</html>

Eslatma: pastki: 0; o'ng: 0; elementning o'ng pastki burchakda aniq joylashuvini bildiradi

element chegaralari va ko'rish oynasi orasidagi bo'shliq.




pozitsiyasi: mutlaq; ::

Pozitsiyali element:mutlaq; pozitsiyasiga emas, balki eng yaqin ajdodiga nisbatan joylashtirilgan

ko'rish oynasiga nisbatan. Mutlaq joylashtirilgan element, agar u bo'lmasa, hujjat tanasidan ajdod sifatida foydalanadi

joylangan ajdod va ular sahifani aylantirish bilan birga harakatlanadi. Quyidagi misolga qarang:


Eslatma: Mutlaq joylashtirilgan elementlar oddiy oqimdan olib tashlanadi va elementlarning ustiga chiqishi mumkin.



<!DOCTYPE html>
<html>
<head>
<uslub>
div.nisbiy {
   pozitsiya: nisbiy;
   kengligi: 400px;
   balandligi: 200px;
   chegara: 3px qattiq #73AD21;
}

div.absolute {
   pozitsiyasi: mutlaq;
   yuqori: 80px;
   o'ng: 0;
   kengligi: 200px;
   balandligi: 100px;
   chegara: 3px qattiq #73AD21;
}
</style>
</head>
<tana>

<h2>pozitsiya: mutlaq;</h2>

<p>Pozitsiyaga ega element: mutlaq; eng yaqin joylashgan ajdodga nisbatan joylashtirilgan (o'rniga

ko'rish oynasiga nisbatan o'rnatilgan, mahkamlangan kabi):</p>

<div class="relative">Ushbu div elementi pozitsiyaga ega: nisbatan;
   <div class="absolute">Ushbu div elementi pozitsiyasiga ega: mutlaq;</div>
</div>

</body>
</html>



Lavozim: yopishqoq; :::

Yopishqoq sifatida joylashtirilgan element aylantirish vaqtida foydalanuvchining joylashuviga nisbatan joylashtirilgan. Tayoq

element pozitsiyasi aylantirish holatiga qarab nisbiy va sobit o'rtasida almashtiriladi. U joylashtirilgan

ko'rish oynasida ma'lum bir ofset pozitsiyasi bajarilmaguncha nisbiy - keyin u joyida "yopishadi" (masalan

pozitsiyasi: belgilangan). Yopishqoq pozitsiyaning ishlashi uchun yuqori, o'ng, pastki yoki chap pozitsiyani ham belgilashingiz kerak.


Yopishqoq element sahifaning yuqori qismiga (yuqori: 0) yopishib qolishi uchun aylantirish holatiga kelganingizda qarang.

quyida buni qanday qilish kerak:


<!DOCTYPE html>
<html>
<head>
<uslub>
div.sticky {
   pozitsiyasi: -webkit-yopishqoq;
   pozitsiyasi: yopishqoq;
   yuqori: 0;
   to'ldirish: 5px;
   fon rangi: #cae8ca;
   chegara: 2px qattiq #4CAF50;
}
</style>
</head>
<tana>

<p>Yopishqoq joylashishni aniqlash qanday ishlashini tushunish uchun ushbu ramka ichida <b>aylanishga</b> harakat qiling.</p>

<div class="sticky">Men yopishqoqman!</div>

<div style="padding-bottom:2000px">
   <p>Ushbu misolda yopishqoq element sahifaning yuqori qismiga yopishib qoladi (yuqori: 0), varaqlash nuqtasiga yetganda

pozitsiyasi.</p>
   <p>Yopishqoqlikni olib tashlash uchun yuqoriga aylantiring.</p>
   <p>O'tkazishni yoqish uchun ba'zi matn.. Lorem ipsum dolor sit amet, illum definitiones no quo, maluisset

concludaturque et eum, altera fabulas ut quo. Atqui causae gloriatur ius te, id agam omnis evertitur eum.

Affert laboramus repudiandae nec et. Inciderint uning reklamasi samarali. Eum no molestiae voluptatibus.</p>
   <p>O'tkazishni yoqish uchun ba'zi matn.. Lorem ipsum dolor sit amet, illum definitiones no quo, maluisset

concludaturque et eum, altera fabulas ut quo. Atqui causae gloriatur ius te, id agam omnis evertitur eum.

Affert laboramus repudiandae nec et. Inciderint uning reklamasi samarali. Eum no molestiae voluptatibus.</p>
</div>

</body>
</html>


Bir-biriga yopishgan elementlar::

Joylashtirilgan elementlar boshqa elementlarning ustiga chiqishi mumkin. Z-index xususiyati stacking tartibini belgilaydi

element (qaysi element oldida (z musbat) yoki orqasida (z salbiy) joylashtirilishi kerak

boshqalar). Z-indeks ijobiy yoki salbiy bo'lishi mumkin.

<!DOCTYPE html>
<html>
<head>
<uslub>
img {
   pozitsiyasi: mutlaq;
   chap: 0px;
   yuqori: 0px;
   z-indeks: -1;
}
</style>
</head>
<tana>

<h1>Bu sarlavha</h1>
<img src="w3css.gif" width="100" height="140">
<p>Rasmning z-indeksi -1 bo'lgani uchun u matn orqasiga joylashtiriladi.</p>

</body>
</html>



Kattaroq stek tartibiga ega element har doim pastroq stek tartibiga ega element oldida turadi.

Eslatma: Agar ikkita joylashtirilgan element z-indeksi ko'rsatilmagan holda bir-birining ustiga tushsa, element eng so'nggida joylashgan

Yuqorida HTML kodi ko'rsatiladi.



Rasmdagi matnni joylashtirish.


Yuqori chap:


<!DOCTYPE html>
<html>
<head>
<uslub>
.idish {
   pozitsiya: nisbiy;
}

.toleft {
   pozitsiyasi: mutlaq;
   yuqori: 8px;
   chap: 16px;
   shrift o'lchami: 18px;
}

img {
   kengligi: 100%;
   balandligi: avtomatik;
   shaffoflik: 0,3;
}
</style>
</head>
<tana>

<h2>Rasm matni</h2>
<p>Yuqori chap burchakdagi rasmga matn qo'shing:</p>

<div class="container">
   <img src="img_5terre_wide.jpg" alt="Cinque Terre" kengligi="1000" balandligi="300">
   <div class="topleft">Yuqori chap</div>
</div>

</body>
</html>


Yuqori o'ng:

<!DOCTYPE html>
<html>
<head>
<uslub>
.idish {
   pozitsiya: nisbiy;
}

.to'g'ri {
   pozitsiyasi: mutlaq;
   yuqori: 8px;
   o'ng: 16px;
   shrift o'lchami: 18px;
}

img {
   kengligi: 100%;
   balandligi: avtomatik;
   shaffoflik: 0,3;
}
</style>
</head>
<tana>

<h2>Rasm matni</h2>
<p>Yuqori oʻng burchakdagi rasmga matn qoʻshing:</p>

<div class="container">
   <img src="img_5terre_wide.jpg" alt="Cinque Terre" kengligi="1000" balandligi="300">
   <div class="topright">Yuqori o‘ng</div>
</div>

</body>
</html>




Pastki chap:

<!DOCTYPE html>
<html>
<head>
<uslub>
.idish {
   pozitsiya: nisbiy;
}

.pastki chap {
   pozitsiyasi: mutlaq;
   pastki: 8px;
   chap: 16px;
   shrift o'lchami: 18px;
}

img {
   kengligi: 100%;
   balandligi: avtomatik;
   shaffoflik: 0,3;
}
</style>
</head>
<tana>

<h2>Rasm matni</h2>
<p>pastki chap burchakdagi rasmga bir oz matn qo'shing:</p>

<div class="container">
   <img src="img_5terre_wide.jpg" alt="Cinque Terre" kengligi="1000" balandligi="300">
   <div class="bottomleft">Pastki chap</div>
</div>

</body>
</html>



Pastki o'ng:


<!DOCTYPE html>
<html>
<head>
<uslub>
.idish {
   pozitsiya: nisbiy;
}

.pastki o'ng {
   pozitsiyasi: mutlaq;
   pastki: 8px;
   o'ng: 16px;
   shrift o'lchami: 18px;
}

img {
   kengligi: 100%;
   balandligi: avtomatik;
   shaffoflik: 0,3;
}
</style>
</head>
<tana>

<h2>Rasm matni</h2>
<p>Quyi oʻng burchakdagi rasmga matn qoʻshing:</p>

<div class="container">
   <img src="img_5terre_wide.jpg" alt="Cinque Terre" kengligi="1000" balandligi="300">
   <div class="bottomright">O'ng pastki</div>
</div>

</body>
</html>




Markazlashtirilgan::

<!DOCTYPE html>
<html>
<head>
<uslub>
.idish {
   pozitsiya: nisbiy;
}

.markaz {
   pozitsiyasi: mutlaq;
   yuqori: 50%;
   kengligi: 100%;
   matnni tekislash: markaz;
   shrift o'lchami: 18px;
}

img {
   kengligi: 100%;
   balandligi: avtomatik;
   shaffoflik: 0,3;
}
</style>
</head>
<tana>

<h2>Rasm matni</h2>
<p>Rasmdagi markaziy matn:</p>

<div class="container">
   <img src="img_5terre_wide.jpg" alt="Cinque Terre" kengligi="1000" balandligi="300">
   <div class="center">Markazlangan</div>
</div>

</body>
</html>



Element shaklini o'rnatish uchun::

<!DOCTYPE html>
<html>
<head>
<uslub>
img {
   pozitsiyasi: mutlaq;
   klip: rect (0px, 60px, 200px, 0px);
}
</style>
</head>
<tana>

<img src="w3css.gif" width="100" height="140">

</body>
</html>



Barcha CSS joylashishni aniqlash xususiyatlari
Mulk tavsifi
pastki O'rnatilgan quti uchun pastki chetini o'rnatadi
clip Mutlaqo joylashtirilgan elementni qirqadi
chap Joylashtirilgan quti uchun chap chekka chekkasini o'rnatadi
pozitsiya Element uchun joylashishni aniqlash turini belgilaydi
o‘ng O‘rnatilgan quti uchun o‘ng chekka chekkasini o‘rnatadi
top Joylashtirilgan quti uchun yuqori chekka chetini o'rnatadi
z-index Elementning stek tartibini o'rnatadi


Eslatma: pozitsiya, chap: -20px; element normal holatidan 20px chapga siljiganligini bildiradi.
      
<kbd>qaytish</kbd>[Mundarijaga qaytish](#homepage)


------




## CSS Z-indeks
CSS Layout - z-index xususiyati

z-indeks xususiyati

Elementlar joylashtirilganda, ular boshqa elementlarning ustiga chiqishi mumkin.

z-index xususiyati elementning stek tartibini belgilaydi (qaysi element boshqalarning oldiga yoki orqasiga joylashtirilishi kerak). Quyidagi CSS z-index rasmiga qarang:

<!DOCTYPE html>
<html>
<head>
<uslub>
img {
   pozitsiyasi: mutlaq;
   chap: 0px;
   yuqori: 0px;
   z-indeks: -1;
}
</style>
</head>
<tana>

<h1>Bu sarlavha</h1>
<img src="w3css.gif" width="100" height="140">
<p>Rasmning z-indeksi -1 bo'lgani uchun u matn orqasiga joylashtiriladi.</p>

</body>
</html>

Eslatma: z-indeks faqat joylashtirilgan elementlarda (pozitsiya: mutlaq, pozitsiya: nisbiy, pozitsiya: qattiq yoki pozitsiya: yopishqoq) va moslashuvchan elementlarda (ekspleyning bevosita bolalari bo'lgan elementlar: moslashuvchan elementlar) ishlaydi.
      
Boshqa z-indeks misoli
Misol

Bu erda biz kattaroq stek tartibiga ega element har doim pastroq stek tartibiga ega elementdan yuqori ekanligini ko'ramiz:
<!DOCTYPE html>
<html>
<head>
<uslub>
.idish {
   pozitsiya: nisbiy;
}

.qora quti {
   pozitsiya: nisbiy;
   z-indeks: 1;
   chegara: 2px qattiq qora;
   balandligi: 100px;
   chegara: 30px;
}

.gray-box {
   pozitsiyasi: mutlaq;
   z-indeks: 3; /* kulrang quti yashil va qora qutining tepasida bo'ladi */
   fon: och kulrang;
   balandligi: 60px;
   kengligi: 70%;
   chap: 50px;
   yuqori: 50px;
}

.yashil quti {
   pozitsiyasi: mutlaq;
   z-indeks: 2; /* yashil quti qora qutining tepasida bo'ladi */
   fon: och yashil;
   kengligi: 35%;
   chap: 270px;
   yuqori: -15px;
   balandligi: 100px;
}
</style>
</head>
<tana>

<h1>Z-indeks misoli</h1>

<p>Yuqorroq stek tartibiga ega element har doim pastroq stek tartibiga ega elementning ustida turadi.</p>

<div class="container">
   <div class="black-box">Qora quti (z-index: 1)</div>
   <div class="gray-box">Kulrang quti (z-index: 3)</div>
   <div class="green-box">Yashil quti (z-index: 2)</div>
</div>

</body>
</html>

Z-indekssiz

Agar ikkita joylashtirilgan element z-indeks ko'rsatilmagan holda bir-birining ustiga tushsa, HTML kodida oxirgi belgilangan element tepada ko'rsatiladi.
Misol

Yuqoridagi misol, lekin bu erda z-indeks ko'rsatilmagan:

<!DOCTYPE html>
<html>
<head>
<uslub>
.idish {
   pozitsiya: nisbiy;
}

.qora quti {
   pozitsiya: nisbiy;
   chegara: 2px qattiq qora;
   balandligi: 100px;
   chegara: 30px;
}

.gray-box {
   pozitsiyasi: mutlaq;
   fon: och kulrang;
   balandligi: 60px;
   kengligi: 70%;
   chap: 50px;
   yuqori: 50px;
}

.yashil quti {
   pozitsiyasi: mutlaq;
   fon: och yashil;
   kengligi: 35%;
   chap: 270px;
   yuqori: -15px;
   balandligi: 100px;
}
</style>
</head>
<tana>

<h1>Bir-biriga yopishgan elementlar</h1>

<p>Agar ikkita joylashtirilgan element z-indeksi belgilanmagan holda bir-birining ustiga tushsa,
HTML kodida oxirgi belgilangan element tepada ko'rsatiladi:</p>

<div class="container">
   <div class="black-box">Qora quti</div>
   <div class="gray-box">Kulrang quti</div>
   <div class="green-box">Yashil quti</div>
</div>

</body>
</html>

CSS xususiyati
Mulk tavsifi
z-index Elementning stek tartibini o'rnatadi
      
      
<kbd>qaytish</kbd>[Mundarijaga qaytish](#homepage)




## CSS Overflow
CSS Layout - Overflow

Agar matn egallash uchun ajratilgan joydan oshsa nima bo'lishini bildiradi.

Ushbu mulkning tasviri quyida ko'rsatilgan:

<!DOCTYPE html>
<html>
<head>
<uslub>
#overflowTest {
   fon: #4CAF50;
   rang: oq;
   to'ldirish: 15px;
   kengligi: 50%;
   balandligi: 100px;
   to'lib-toshgan: aylantirish;
   chegara: 1px qattiq #ccc;
}
</style>
</head>
<tana>

<h2>CSS Overflow</h2>
<p>Toshib ketish xususiyati hududga sig‘maydigan darajada katta bo‘lgan kontentga nima bo‘lishini nazorat qiladi.</p>

<div id="overflowTest">Ushbu matn haqiqatan ham uzun va uning konteyner balandligi atigi 100 piksel.

Shuning uchun, o'quvchiga tarkibni aylantirishga yordam berish uchun aylantirish paneli qo'shiladi. Lorem ipsum dolor sit amet,

consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut laoreet dolore magna aliquam erat

volutpat. Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut

aliquip ex ea commodo consequat. Duis autem vel eum iriure dolor in hendrerit in vulputate velit esse

molestie consequat, vel illum doore eu feugiat nulla facilisis at vero eros et accumsan et iusto odio

dignissim qui blandit praesent luptatum zzril delenit augue duis dolore te feugait nulla facilisi. Nam ozod

tempor cum soluta nobis eleifend option congue nihil imperdiet doming id quod mazim placerat facer possim

faraz qilmoq. Typi non habent claritatem insitam; est usus legentis in iis qui facit eorum claritatem.</div>

</body>
</html>




CSS Overflow

Element tarkibiga o'tish satri yoki qirqish tarkibi kiritilishini belgilaydi

belgilangan hududga sig'ish uchun juda katta.


Overflow xususiyatining xususiyatlari:
ko'rinadigan: Bu sukut bo'lib, toshib ketish kesilmasligini ta'minlaydi. Kontent tashqarida paydo bo'ladi

element qutisi.

yashirin: elementning qolgan tarkibini ko'rinadigan qilib, to'ldirishni qirqadi
aylantirish: elementning qolgan qismi bo'lishi mumkin bo'lgan aylantirish panellarini qo'shib, to'lib-toshganni kesib tashlaydi

ko'rgan.
auto: aylantirishga o'xshash ishlaydi, faqat kerak bo'lganda aylantirish satrlarini qo'shadi.

Eslatma: Overflow xususiyati belgilangan balandlikdagi blok elementlari uchun ishlaydi. Shuningdek,

OS X Lion-da (Mac-da) aylantirish panellari sukut bo'yicha yashiriladi va faqat foydalanilganda ko'rsatiladi (garchi bo'lsa ham)

"overflow: scroll" o'rnatilgan).



toshib ketish: ko'rinadigan; ::

bu toshib ketish uchun standart qiymatdir. U kesilmaydi va element qutisidan tashqarida ko'rsatiladi. ga qarang

toshib ketish tasviri: quyida ko'rinadi:

<!DOCTYPE html>
<html>
<head>
<uslub>
div {
   fon rangi: #eee;
   kengligi: 200px;
   balandligi: 50px;
   chegara: 1px nuqtali qora;
   toshib ketish: ko'rinadigan;
}
</style>
</head>
<tana>

<h2>CSS Overflow</h2>
<p>Sukut bo'yicha, to'lib ketish ko'rinadi, ya'ni u kesilmaydi va elementdan tashqarida ko'rsatiladi.

quti:</p>

<div>Tuzilishni yaxshiroq boshqarishni istasangiz, overflow xususiyatidan foydalanishingiz mumkin. Toshib ketish

xususiyat, agar kontent elementning qutisiga to‘lib ketgan bo‘lsa, nima bo‘lishini belgilaydi.</div>

</body>
</html>


toshib ketish: yashirin; ::

Yashirin toshib ketish xususiyatining qiymati kesiladi (berilgan qutiga mos keladi), qolgan qismi esa

yashirin. To'lib-toshgan rasmga qarang: yashirin; quyida:


<!DOCTYPE html>
<html>
<head>
<uslub>
div {
   fon rangi: #eee;
   kengligi: 200px;
   balandligi: 50px;
   chegara: 1px nuqtali qora;
   toshib ketish: yashirin;
}
</style>
</head>
<tana>

<h2>CSS Overflow</h2>
<p>Yashirin qiymat bilan to‘lib-tosh qirqib olinadi, qolgan tarkib esa berkitiladi:</p>
<p>Uning qanday ishlashini tushunish uchun overflow xususiyatini olib tashlashga harakat qiling.</p>

<div>Tuzilishni yaxshiroq boshqarishni istasangiz, overflow xususiyatidan foydalanishingiz mumkin. Toshib ketish

xususiyat, agar kontent elementning qutisiga to‘lib ketgan bo‘lsa, nima bo‘lishini belgilaydi.</div>

</body>
</html>



to'lib-toshgan: aylantirish; ::

To'lib-tosh o'tishga o'rnatilgan bo'lsa, bunday to'lib ketish kesiladi va quti ichiga aylantirish paneli qo'shiladi. Bu

parametr, hatto kerak bo'lmagan holatlarda ham gorizontal va vertikal aylantirish chiziqlarini qo'shadi. Qarang

toshib ketishning tasviri: aylantirish; quyida:

<!DOCTYPE html>
<html>
<head>
<uslub>
div {
   fon rangi: #eee;
   kengligi: 200px;
   balandligi: 100px;
   chegara: 1px nuqtali qora;
   to'lib-toshgan: aylantirish;
}
</style>
</head>
<tana>

<h2>CSS Overflow</h2>
<p>O'tish uchun to'ldirish qiymatini o'rnatish, to'ldirish kesiladi va ichkarida aylantirish uchun aylantirish paneli qo'shiladi

quti. E'tibor bering, bu gorizontal va vertikal ravishda aylantirish paneli qo'shadi (hatto kerak bo'lmasa ham

u):</p>

<div>Tuzilishni yaxshiroq boshqarishni istasangiz, overflow xususiyatidan foydalanishingiz mumkin. Toshib ketish

xususiyat, agar kontent elementning qutisiga to‘lib ketgan bo‘lsa, nima bo‘lishini belgilaydi.</div>

</body>
</html>



toshib ketish: avtomatik; ::

Overflow: auto; aylantirishga o'xshaydi, lekin faqat kerak bo'lganda aylantirish panellarini qo'shing. Aslida, u

toshib ketganda paydo bo'ladigan foydasiz siljishlar masalalarini hal qiladi:scroll; ishlatilgan. Rasmga qarang

toshib ketish:avto; quyida:

<!DOCTYPE html>
<html>
<head>
<uslub>
div {
   fon rangi: #eee;
   kengligi: 200px;
   balandligi: 50px;
   chegara: 1px nuqtali qora;
   toshib ketish: avtomatik;
}
</style>
</head>
<tana>

<h2>CSS Overflow</h2>
<p>Avtomatik qiymat aylantirishga o'xshaydi, faqat kerak bo'lganda aylantirish panellarini qo'shadi:</p>

<div>Tuzilishni yaxshiroq boshqarishni istasangiz, overflow xususiyatidan foydalanishingiz mumkin. Toshib ketish

xususiyat, agar kontent elementning qutisiga to‘lib ketgan bo‘lsa, nima bo‘lishini belgilaydi.</div>

</body>
</html>



to'lib-toshgan-x va to'lib-toshgan-y; ::

overflow-x va overflow-y xossalari kontentning toʻlib ketishini faqat gorizontal, faqat vertikal yoki

ikkalasi ham. Bu overflow tomonidan berilgan o'xshash afzalliklarni berishi mumkin: auto: overflow: scroll;
Quyida overflow-x va overflow-y rasmlariga qarang:


<!DOCTYPE html>
<html>
<head>
<uslub>
div {
   fon rangi: #eee;
   kengligi: 200px;
   balandligi: 50px;
   chegara: 1px nuqtali qora;
   overflow-x: yashirin;
   overflow-y: aylantirish;
}
</style>
</head>
<tana>

<h2>CSS Overflow</h2>
<p>Shuningdek, kontentning toʻlib ketishini gorizontal yoki vertikal ravishda oʻzgartirishingiz mumkin.</p>
<p>overflow-x kontentning chap/o‘ng qirralari bilan nima qilish kerakligini belgilaydi.<br>
overflow-y kontentning yuqori/pastki qirralari bilan nima qilish kerakligini belgilaydi.</p>

<div>Tuzilishni yaxshiroq boshqarishni istasangiz, overflow xususiyatidan foydalanishingiz mumkin. Toshib ketish

xususiyat, agar kontent elementning qutisiga to‘lib ketgan bo‘lsa, nima bo‘lishini belgilaydi.</div>

</body>
</html>



Barcha CSS Overflow xususiyatlari
Mulk tavsifi
Overflow Agar kontent elementning qutisiga toʻlib ketgan boʻlsa, nima boʻlishini belgilaydi
overflow-x Agar kontentning chap/o'ng qirralari elementning chegarasidan oshib ketsa, nima qilish kerakligini belgilaydi.

tarkib maydoni
overflow-y Agar kontent elementning yuqori/pastki qirralari bilan nima qilish kerakligini belgilaydi.

tarkib maydoni

<kbd>qaytish</kbd>[Mundarijaga qaytish](#homepage)


------------


