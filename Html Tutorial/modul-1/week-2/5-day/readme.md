## HTML SINFLARI

** html klassi atributi html elementi uchun sinfni belgilash uchun ishlatiladi.

* Bir nechta HTML elementlari ham bir xil sinfni baham ko'rishi mumkin.
* Class atributi uslublar jadvalida birgalikda manipulyatsiya qilish uchun sinfga ishora qilish uchun ishlatiladi. Javascript bir sinfdagi elementlarni birgalikda boshqarishi mumkin.

** Quyidagi misolda, shahar sinfiga ega bo'lgan uchta div elementi sarlavhadagi .city uslubi ta'rifiga ko'ra bir xil tarzda bir xil uslubda.
```
<!DOCTYPE html>
<html>
<head>
<uslub>
.shahar {
   fon rangi: pomidor;
   rang: oq;
   chegara: 2px qattiq qora;
   chegara: 20px;
   to'ldirish: 20px;
}
</style>
</head>
<tana>

<div class="shahar">
   <h2>London</h2>
   <p>London - Angliya poytaxti.</p>
</div>

<div class="shahar">
   <h2>Parij</h2>
   <p>Parij - Fransiyaning poytaxti.</p>
</div>

<div class="shahar">
   <h2>Tokio</h2>
   <p>Tokio - Yaponiya poytaxti.</p>
</div>

</body>
</html>
```



** Bu yerda biz ```<span>``` elementlaridagi eslatma sinfini .note uslubi ta'rifi bilan ham uslublashimiz mumkin

```
<!DOCTYPE html>
<html>
<head>
<uslub>
.Eslatma {
   shrift hajmi: 120%;
   rang: qizil;
}
</style>
</head>
<tana>

<h1>Mening <span class="note">Muhim</span> sarlavham</h1>
<p>Bu <span class="note">muhim</span> matn.</p>

</body>
</html>
```
NB

Maslahat: Class atributidan istalgan HTML elementida foydalanish mumkin.

Eslatma: sinf nomi katta-kichik harflarga sezgir!


* Sintaksis sintaksisi.

Sinf yaratish uchun; nuqta (.) belgisini, undan keyin sinf nomini yozing. Keyin, jingalak qavslar ichida CSS xususiyatlarini aniqlang {}

```
<!DOCTYPE html>
<html>
<head>
<uslub>
.shahar {
   fon rangi: pomidor;
   rang: oq;
   to'ldirish: 10px;
}
</style>
</head>
<tana>

<h2 class="city">London</h2>
<p>London - Angliya poytaxti.</p>

<h2 class="city">Parij</h2>
<p>Parij - Fransiyaning poytaxti.</p>

<h2 class="city">Tokio</h2>
<p>Tokio - Yaponiya poytaxti.</p>

</body>
</html>
```
* Bir nechta sinflar.

HTML elementlari bir nechta sinflarga tegishli bo'lishi mumkin. Sinf nomlarini bo'sh joy bilan ajratib, bir nechta sinflarni aniqlang. Element belgilangan barcha sinflar bo'yicha uslublanadi.

Quyida ```<h2>``` elementlari ham shahar sinfiga, ham asosiy sinfga tegishli (```<div class="city main">```)

Quyida h2 elementi shahar sinfiga ham, asosiy sinfga ham tegishli va ikkala sinfdan CSS uslublarini oladi.
```
<h2 class="city main">London</h2>
<h2 class="city">Parij</h2>
<h2 class="city">Tokio</h2>
```

* To'liq html
```
<!DOCTYPE html>
<html>
<head>
<uslub>
.shahar {
   fon rangi: pomidor;
   rang: oq;
   to'ldirish: 10px;
}

.asosiy {
   matnni tekislash: markaz;
}
</style>
</head>
<tana>

<h2>Bir nechta sinflar</h2>
<p>Bu erda barcha uchta h2 elementi "shahar" sinfiga tegishli. Bundan tashqari, London ham matnni markazga tekislovchi “asosiy” sinfga tegishli.</p>

<h2 class="city main">London</h2>
<h2 class="city">Parij</h2>
<h2 class="city">Tokio</h2>

</body>
</html>
```

```<p>``` va ```<h2>``` kabi turli HTML elementlari shahar sinfiga ishora qiladi va bir xil uslubga ega.

```
<h2 class="city">Parij</h2>
<p class="city">Parij - Fransiya poytaxti</p>
```
** Javascriptda sinf atributidan foydalaning
Sinf nomi JS tomonidan muayyan elementlar uchun muayyan vazifalarni bajarish uchun ham ishlatilishi mumkin.
JS odatda ```getElementByClassName()``` usuli bilan ma`lum sinf nomiga ega elementlarga kirishadi:

```
<skript>
funktsiya myFunction() {
   var x = document.getElementsByClassName("shahar");
   uchun (var i = 0; i < x.length; i++) {
     x[i].style.display = "yo'q";
   }
}
</script>
```
<kbd>qaytish</kbd>[Mundarijaga qaytish](#homepage)


---------
## HTML identifikatori
HTML ID ATTRIBUTE: HTML elementi uchun noyob identifikatorni belgilash uchun ishlatiladi.

Faqat bitta element ma'lum bir identifikatorga ega.


Id atributi uslublar jadvalidagi muayyan uslub deklaratsiyasiga ishora qilish uchun ishlatiladi. JS tomonidan ma'lum identifikatorga ega elementlarga kirish va ularni boshqarish uchun ham foydalaniladi.

id sintaksisi: ```(#)``` xeshdan keyin id nomini yozing. Keyin CSS xususiyatlarini jingalak qavslar bilan belgilang {}. quyidagi varaqda ```<h1>``` elementi ga muvofiq uslublangan
Sarlavha qismida HashmyHeader uslubi ta'rifi

```
<!DOCTYPE html>
<html>
<head>
<uslub>
#mening sarlavham {
   fon rangi: ochiq ko'k;
   rang: qora;
   to'ldirish: 40px;
   matnni tekislash: markaz;
}
</style>
</head>
<tana>

<h1 id="myHeader">Mening sarlavham</h1>

</body>
</html>
```

** ID nomi katta-kichik harflarga sezgir! Va u kamida bitta belgidan iborat bo'lishi kerak va bo'sh joylar (bo'shliqlar, yorliqlar va boshqalar) bo'lmasligi kerak.

Class va ID o'rtasidagi farq: Class bir nechta HTML elementlari tomonidan ishlatilishi mumkin, id nomi esa sahifadagi faqat bitta HTML elementi tomonidan ishlatilishi kerak.

** Quyida biz Class va ID o'rtasidagi farqni ko'rsatamiz
```
<!DOCTYPE html>
<html>
<head>
<uslub>
/* Elementga “myHeader” identifikatori bilan uslub bering */
#mening sarlavham {
   fon rangi: ochiq ko'k;
   rang: qora;
   to'ldirish: 40px;
   matnni tekislash: markaz;
}

/* Barcha elementlarni “shahar” sinf nomi bilan uslublang */
.shahar {
   fon rangi: pomidor;
   rang: oq;
   to'ldirish: 10px;
}
</style>
</head>
<tana>

<h2>Sinf va ID o'rtasidagi farq</h2>
<p>Sinf nomi bir nechta HTML elementlari tomonidan ishlatilishi mumkin, id nomi esa sahifadagi faqat bitta HTML elementi tomonidan ishlatilishi kerak:</p>

<!-- Noyob identifikatorli element -->
<h1 id="myHeader">Mening shaharlarim</h1>

<!-- Bir xil sinfga ega bir nechta elementlar -->
<h2 class="city">London</h2>
<p>London - Angliya poytaxti.</p>

<h2 class="city">Parij</h2>
<p>Parij - Fransiyaning poytaxti.</p>

<h2 class="city">Tokio</h2>
<p>Tokio - Yaponiya poytaxti.</p>

</body>
</html>
```

** ID va havolalar bilan HTML xatcho'plari.

Html xatcho'plari o'quvchilarga veb-sahifaning ma'lum bir qismiga o'tish imkonini beradi, bu juda uzun sahifalar uchun foydalidir.

Xatcho‘pdan foydalanish uchun uni yarating va unga havola qo‘shing. Havolani bosgandan so'ng, sahifa xatcho'p joylashgan joyga o'tadi.


** Xatcho'p yaratish uchun,

```<h2 id="C4">4-bob</h2>```


* Unga havola qo'shish uchun:
```
<a href="#C4">4-bobga o‘tish</a>
```
* Boshqa sahifadan xatcho'pga havola qo'shish uchun (4-bo'limga o'tish).

```
<a href="html_demo.html#C4">4-bobga o‘tish</a>
```

** Quyidagi namoyishga qarang:
```
<!DOCTYPE html>
<html>
<tana>

<p><a href="#C4">4-bobga o‘tish</a></p>
<p><a href="#C10">10-bobga o‘tish</a></p>

<h2>1-bob</h2>
<p>Ushbu bobda ba bla bla tushuntiriladi</p>

<h2>2-bob</h2>
<p>Ushbu bobda ba bla bla tushuntiriladi</p>

<h2>3-bob</h2>
<p>Ushbu bobda ba bla bla tushuntiriladi</p>

<h2 id="C4">4-bob</h2>
<p>Ushbu bobda ba bla bla tushuntiriladi</p>

<h2>5-bob</h2>
<p>Ushbu bobda ba bla bla tushuntiriladi</p>

<h2>6-bob</h2>
<p>Ushbu bobda ba bla bla tushuntiriladi</p>

<h2>7-bob</h2>
<p>Ushbu bobda ba bla bla tushuntiriladi</p>

<h2>8-bob</h2>
<p>Ushbu bobda ba bla bla tushuntiriladi</p>

<h2>9-bob</h2>
<p>Ushbu bobda ba bla bla tushuntiriladi</p>

<h2 id="C10">10-bob</h2>
<p>Ushbu bobda ba bla bla tushuntiriladi</p>

<h2>11-bob</h2>
<p>Ushbu bobda ba bla bla tushuntiriladi</p>

<h2>12-bob</h2>
<p>Ushbu bobda ba bla bla tushuntiriladi</p>

<h2>13-bob</h2>
<p>Ushbu bobda ba bla bla tushuntiriladi</p>

<h2>14-bob</h2>
<p>Ushbu bobda ba bla bla tushuntiriladi</p>

<h2>15-bob</h2>
<p>Ushbu bobda ba bla bla tushuntiriladi</p>

<h2>16-bob</h2>
<p>Ushbu bobda ba bla bla tushuntiriladi</p>

<h2>17-bob</h2>
<p>Ushbu bobda ba bla bla tushuntiriladi</p>

<h2>18-bob</h2>
<p>Ushbu bobda ba bla bla tushuntiriladi</p>

<h2>19-bob</h2>
<p>Ushbu bobda ba bla bla tushuntiriladi</p>

<h2>20-bob</h2>
<p>Ushbu bobda ba bla bla tushuntiriladi</p>

<h2>21-bob</h2>
<p>Ushbu bobda ba bla bla tushuntiriladi</p>

<h2>22-bob</h2>
<p>Ushbu bobda ba bla bla tushuntiriladi</p>

<h2>23-bob</h2>
<p>Ushbu bobda ba bla bla tushuntiriladi</p>

</body>
</html>
```

* JavaScript-da id atributidan foydalanish

Id atributi JavaScript tomonidan ushbu element uchun ba'zi vazifalarni bajarish uchun ham ishlatilishi mumkin.

JavaScript ```getElementById()``` usuli bilan ma`lum identifikatorli elementga kirishi mumkin:

```
<skript>
funktsiya displayResult() {
   document.getElementById("myHeader").innerHTML = "Kuningiz xayrli o'tsin!";
}
</script>
```

* Bo'lim xulosasi::
Bo'lim xulosasi
Id atributi HTML elementi uchun noyob identifikatorni belgilash uchun ishlatiladi
ID atributining qiymati HTML hujjatida yagona bo'lishi kerak
Id atributi CSS va JavaScript tomonidan muayyan elementni uslublash/tanlash uchun ishlatiladi
Id atributining qiymati katta-kichik harflarga sezgir
Id atributi HTML xatcho'plarini yaratish uchun ham ishlatiladi
JavaScript getElementById() usuli yordamida ma'lum identifikatorga ega elementga kirishi mumkin

<kbd>qaytish</kbd>[Mundarijaga qaytish](#homepage)


-------


#CSS fonlari

CSS bir nechta fon

Ushbu bo'limda siz bir elementga bir nechta fon rasmlarini qanday qo'shishni o'rganasiz.

Shuningdek, siz quyidagi xususiyatlar haqida bilib olasiz:

     fon o'lchami
     fon kelib chiqishi
     fon klipi

CSS bir nechta fon

CSS fon tasviri xususiyati orqali element uchun bir nechta fon rasmlarini qo'shish imkonini beradi.

Turli fon rasmlari vergul bilan ajratiladi va tasvirlar bir-birining ustiga joylashtiriladi,

birinchi rasm tomoshabinga eng yaqin bo'lgan joyda.

Quyidagi misolda ikkita fon tasviri bor, birinchi rasm gul (pastga tekislangan va

o'ng) va ikkinchi rasm qog'oz fon (yuqori chap burchakka tekislangan):


<!DOCTYPE html>
<html>
<head>
<uslub>
#misol1 {
   fon rasmi: url(img_flwr.gif), url(paper.gif);
   fon-pozitsiya: o'ng pastki, chap yuqori;
   fon-takrorlash: takrorlanmaslik, takrorlash;
   to'ldirish: 15px;
}
</style>
</head>
<tana>

<h1>Bir nechta fon</h1>
<p>Quyidagi div elementida ikkita fon tasviri mavjud:</p>

<div id="example1">
   <h1>Lorem Ipsum Dolor</h1>
   <p>Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut

laoreet dolore magna aliquam erat volutpat.</p>
   <p>Ut wisi enim ad minim vaniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip

ex ea commodo consequat.</p>
</div>

</body>
</html>




Bir nechta fon tasvirlari alohida fon xususiyatlaridan (yuqoridagi kabi) yoki yordamida belgilanishi mumkin

fon stenografiyasi xususiyati.

Quyidagi misol fon stenografiyasi xususiyatidan foydalanadi (yuqoridagi misol bilan bir xil natija):

<!DOCTYPE html>
<html>
<head>
<uslub>
#misol1 {
   fon: url(img_flwr.gif) o'ng pastki takrorlanmaydi, url(paper.gif) chap yuqori takror;
   to'ldirish: 15px;
}
</style>
</head>
<tana>

<div id="example1">
   <h1>Lorem Ipsum Dolor</h1>
   <p>Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut

laoreet dolore magna aliquam erat volutpat.</p>
   <p>Ut wisi enim ad minim vaniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip

ex ea commodo consequat.</p>
</div>

</body>
</html>




CSS fon hajmi

CSS fon o'lchami xususiyati fon tasvirlarining o'lchamini belgilash imkonini beradi.

Hajmi uzunliklarda, foizlarda yoki ikkita kalit so'zdan biri yordamida ko'rsatilishi mumkin: o'z ichiga yoki qoplash.

Quyidagi misol fon tasvirini asl tasvirdan ancha kichikroq qilib o'zgartiradi (piksellar yordamida). Qarang

quyidagi kod:


<!DOCTYPE html>
<html>
<head>
<uslub>
#misol1 {
   chegara: 1px qattiq qora;
   fon: url (img_flwr.gif);
   fon o'lchami: 100px 80px;
   fon-takrorlash: takrorlanmaslik;
   to'ldirish: 15px;
}

#misol2 {
   chegara: 1px qattiq qora;
   fon: url (img_flwr.gif);
   fon-takrorlash: takrorlanmaslik;
   to'ldirish: 15px;
}
</style>
</head>
<tana>

<h1>Fon o'lchamidagi xususiyat</h1>

<p>O'lchami o'zgartirilgan fon rasmi:</p>
<div id="example1">
   <h2>Lorem Ipsum Dolor</h2>
   <p>Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut

laoreet dolore magna aliquam erat volutpat.</p>
   <p>Ut wisi enim ad minim vaniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip

ex ea commodo consequat.</p>
</div>

<p>Fon-tasvirning asl hajmi:</p>
<div id="example2">
   <h2>Lorem Ipsum Dolor</h2>
   <p>Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut

laoreet dolore magna aliquam erat volutpat.</p>
   <p>Ut wisi enim ad minim vaniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip

ex ea commodo consequat.</p>
</div>

</body>
</html>




Fon o'lchami uchun boshqa ikkita mumkin bo'lgan qiymatlar o'z ichiga va qopqoqdir.

Content kalit so'zi fon tasvirini iloji boricha kattalashtirishga imkon beradi (lekin uning kengligi ham, uning ham

balandligi kontent maydoniga mos kelishi kerak). Shunday qilib, fon tasvirining nisbatlariga qarab va

fon joylashuvi maydonida, fonning tomonidan qoplanmagan ba'zi joylari bo'lishi mumkin

fon tasviri.

Muqova kalit so'zi fon tasvirini o'lchaydi, shunda kontent maydoni to'liq qoplanadi

fon tasviri (uning kengligi ham, balandligi ham kontent maydoniga teng yoki undan katta). Shunday qilib, ba'zi qismlari

fon rasmi fonni joylashtirish sohasida ko'rinmasligi mumkin.

Quyidagi misolda contain va cover dan foydalanish ko‘rsatilgan:

<!DOCTYPE html>
<html>
<head>
<uslub>
.div1 {
   chegara: 1px qattiq qora;
   balandligi: 120px;
   kengligi: 150px;
   fon: url (img_flwr.gif);
   fon-takrorlash: takrorlanmaslik;
   fon o'lchami: o'z ichiga oladi;
}

.div2 {
   chegara: 1px qattiq qora;
   balandligi: 120px;
   kengligi: 150px;
   fon: url (img_flwr.gif);
   fon-takrorlash: takrorlanmaslik;
   fon o'lchami: qopqoq;
}

.div3 {
   chegara: 1px qattiq qora;
   balandligi: 120px;
   kengligi: 150px;
   fon: url (img_flwr.gif);
   fon-takrorlash: takrorlanmaslik;
}
</style>
</head>
<tana>

<h1>Fon o'lchamidagi xususiyat</h1>

<h2>fon o'lchami: tarkibi:</h2>
<div class="div1">
<p>Lorem ipsum dolor sit amet.</p>
</div>

<h2>fon o'lchami: qopqoq:</h2>
<div class="div2">
<p>Lorem ipsum dolor sit amet.</p>
</div>

<h2>Fon o'lchami aniqlanmagan:</h2>
<div class="div3">
<p>Lorem ipsum dolor sit amet.</p>
</div>

<p>Asl rasm:</p>
<img src="img_flwr.gif" alt="Gullar" kengligi="224" balandligi="162">

</body>
</html>




Bir nechta fon rasmlarining o'lchamlarini aniqlang

Fon o'lchami xususiyati fon o'lchami uchun bir nechta qiymatlarni ham qabul qiladi (vergul bilan ajratilgan

ro'yxat), bir nechta fon bilan ishlashda.

Quyidagi misolda har biri uchun har xil fon o'lchami qiymatiga ega uchta fon tasviri ko'rsatilgan

rasm:



<!DOCTYPE html>
<html>
<head>
<uslub>
#misol1 {
   fon: url(img_tree.gif) chap tepada takrorlanmaydi, url(img_flwr.gif) o‘ng pastki qismida takrorlanmaydi, url(paper.gif)

chap yuqori takrorlash;
   to'ldirish: 15px;
   fon o'lchami: 50px, 130px, avtomatik;
}
</style>
</head>
<tana>

<div id="example1">
   <h1>Lorem Ipsum Dolor</h1>
   <p>Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut

laoreet dolore magna aliquam erat volutpat.</p>
   <p>Ut wisi enim ad minim vaniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip

ex ea commodo consequat.</p>
</div>

</body>
</html>





To'liq o'lchamli fon rasmi

Endi biz veb-saytda har doim butun brauzer oynasini qamrab oladigan fon tasviriga ega bo'lishni xohlaymiz.

Talablar quyidagicha:

     Butun sahifani rasm bilan to'ldiring (bo'sh joysiz)
     Tasvirni kerak bo'lganda masshtablashtiring
     Sahifadagi markaziy rasm
     O'tkazish paneliga olib kelmang

Quyidagi misol buni qanday qilishni ko'rsatadi; <html> elementidan foydalaning (<html> elementi har doim kamida

brauzer oynasining balandligi). Keyin unga sobit va markazlashtirilgan fonni o'rnating. Keyin uning o'lchamini o'rnating

fon o'lchami xususiyati:



<!DOCTYPE html>
<html>
<head>
<uslub>
html {
   fon: url(img_man.jpg) takrorlanmaydigan markaz o'rnatildi;
   fon o'lchami: qopqoq;
}

tana {
   rang: oq;
}
</style>
</head>
<tana>

<h1>To'liq sahifa fon rasmi</h1>
<p>Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut

laoreet dolore magna aliquam erat volutpat. Ut wisi enim ad minimal vaniam, quis nostrud exercitation

ullamcorper suscipit lobortis nisl ut aliquip ex ea commodo consequat.</p>

</body>
</html>



Qahramon tasviri

Qahramon tasvirini yaratish uchun <div> da turli xil fon xususiyatlaridan foydalanishingiz mumkin (katta rasm

matn) va uni xohlagan joyga joylashtiring.


<!DOCTYPE html>
<html>
<head>
<uslub>
html {
   fon: url(img_man.jpg) takrorlanmaydigan markaz o'rnatildi;
   fon o'lchami: qopqoq;
}

tana {
   rang: oq;
}
</style>
</head>
<tana>

<h1>To'liq sahifa fon rasmi</h1>
<p>Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut

laoreet dolore magna aliquam erat volutpat. Ut wisi enim ad minimal vaniam, quis nostrud exercitation

ullamcorper suscipit lobortis nisl ut aliquip ex ea commodo consequat.</p>

</body>
</html>




CSS background-origin xususiyati fon tasviri qayerda joylashganligini belgilaydi.

Mulk uch xil qiymatga ega:

     border-box - fon tasviri chegaraning yuqori chap burchagidan boshlanadi
     padding-box - (standart) fon tasviri to'ldirish chetining yuqori chap burchagidan boshlanadi
     content-box - fon tasviri kontentning yuqori chap burchagidan boshlanadi

Quyidagi misol fon-origin xususiyatini ko'rsatadi:

<!DOCTYPE html>
<html>
<head>
<uslub>
#misol1 {
   chegara: 10px qattiq qora;
   to'ldirish: 35px;
   fon: url (img_flwr.gif);
   fon-takrorlash: takrorlanmaslik;
}

#misol2 {
   chegara: 10px qattiq qora;
   to'ldirish: 35px;
   fon: url (img_flwr.gif);
   fon-takrorlash: takrorlanmaslik;
   fon-kelib chiqishi: chegara qutisi;
}

#misol3 {
   chegara: 10px qattiq qora;
   to'ldirish: 35px;
   fon: url (img_flwr.gif);
   fon-takrorlash: takrorlanmaslik;
   fon-kelib chiqishi: kontent-box;
}
</style>
</head>
<tana>
<h1>Fondan kelib chiqadigan xususiyat</h1>

<p>Fon manbasi yo'q (to'ldirish qutisi sukut bo'yicha):</p>
<div id="example1">
   <h2>Lorem Ipsum Dolor</h2>
   <p>Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut

laoreet dolore magna aliquam erat volutpat.</p>
   <p>Ut wisi enim ad minim vaniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip

ex ea commodo consequat.</p>
</div>

<p>fon-kelib chiqishi: chegara qutisi:</p>
<div id="example2">
   <h2>Lorem Ipsum Dolor</h2>
   <p>Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut

laoreet dolore magna aliquam erat volutpat.</p>
   <p>Ut wisi enim ad minim vaniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip

ex ea commodo consequat.</p>
</div>

<p>fon-kelib chiqishi: kontent-box:</p>
<div id="example3">
   <h2>Lorem Ipsum Dolor</h2>
   <p>Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut

laoreet dolore magna aliquam erat volutpat.</p>
   <p>Ut wisi enim ad minim vaniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip

ex ea commodo consequat.</p>
</div>

</body>
</html>

  

CSS fon-klip xususiyati

CSS background-clip xususiyati fonning bo'yash maydonini belgilaydi.

Mulk uch xil qiymatga ega:

     chegara qutisi - (standart) fon chegaraning tashqi chetiga bo'yalgan
     padding-box - fon plombaning tashqi chetiga bo'yalgan
     kontent qutisi - fon kontent oynasida bo'yalgan

Quyidagi misolda background-clip xususiyati tasvirlangan:

<!DOCTYPE html>
<html>
<head>
<uslub>
#misol1 {
   chegara: 10px nuqtali qora;
   to'ldirish: 35px;
   fon: sariq;
}

#misol2 {
   chegara: 10px nuqtali qora;
   to'ldirish: 35px;
   fon: sariq;
   fon-klip: padding-box;
}

#misol3 {
   chegara: 10px nuqtali qora;
   to'ldirish: 35px;
   fon: sariq;
   fon-klip: kontent qutisi;
}
</style>
</head>
<tana>

<h1>Fon-klip xususiyati</h1>

<p>Fon-klip yo'q (chegara qutisi birlamchi):</p>
<div id="example1">
   <h2>Lorem Ipsum Dolor</h2>
   <p>Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut

laoreet dolore magna aliquam erat volutpat.</p>
</div>

<p>fon-klip: padding-box:</p>
<div id="example2">
   <h2>Lorem Ipsum Dolor</h2>
   <p>Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut

laoreet dolore magna aliquam erat volutpat.</p>
</div>

<p>fon-klip: kontent qutisi:</p>
<div id="example3">
   <h2>Lorem Ipsum Dolor</h2>
   <p>Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut

laoreet dolore magna aliquam erat volutpat.</p>
</div>

</body>
</html>



CSS Advanced Background Properties
Property 	Description
background 	A shorthand property for setting all the background properties in one declaration
background-clip 	Specifies the painting area of the background
background-image 	Specifies one or more background images for an element
background-origin 	Specifies where the background image(s) is/are positioned
background-size 	Specifies the size of the background image(s)


<kbd>return</kbd>[Back to table of contents](#homepage)
- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -   
  
 
## CSS ranglari


RGBA ranglari

RGBA rang qiymatlari alfa kanali bilan RGB rang qiymatlarining kengaytmasi bo'lib, shaffoflikni belgilaydi.

rang uchun.

RGBA rang qiymati quyidagi bilan belgilanadi: rgba (qizil, yashil, ko'k, alfa). Alfa parametri raqamdir

0,0 (to'liq shaffof) va 1,0 (to'liq shaffof) orasida. RGBA ta'rifi uchun quyidagi misolga qarang

ranglar:


<!DOCTYPE html>
<html>
<head>
<uslub>
#p1 {fon rangi: rgba (255,0,0,0,3);}
#p2 {fon rangi: rgba (0,255,0,0,3);}
#p3 {fon rangi:rgba(0,0,255,0,3);}
#p4 {fon rangi: rgba (192,192,192,0.3);}
#p5 {fon rangi:rgba(255,255,0,0,3);}
#p6 {fon rangi:rgba(255,0,255,0,3);}
</style>
</head>
<tana>

<h1>RGBA qiymatlari bilan ranglarni aniqlang</h1>

<p id="p1">Qizil</p>
<p id="p2">Yashil</p>
<p id="p3">Moviy</p>
<p id="p4">Kulrang</p>
<p id="p5">Sariq</p>
<p id="p6">Cerise</p>

</body>
</html>



HSL ranglari

HSL qisqartmasi Hue, Saturation va Lightness degan ma'noni anglatadi.

HSL rang qiymati quyidagi bilan belgilanadi: hsl (rang, to'yinganlik, yorug'lik).

     Hue - rang g'ildiragidagi daraja (0 dan 360 gacha):
         0 (yoki 360) qizil
         120 yashil
         240 ko'k
     To'yinganlik - bu foizli qiymat: 100% - to'liq rang.
     Yengillik ham foiz hisoblanadi; 0% quyuq (qora) va 100% oq.
Quyidagi misol HSL ranglarining ta'rifini ko'rsatadi:


<!DOCTYPE html>
<html>
<head>
<uslub>
#p1 {fon rangi: hsl(120,100%,50%);}
#p2 {fon rangi: hsl(120,100%,75%);}
#p3 {fon rangi: hsl(120,100%,25%);}
#p4 {fon rangi: hsl(120,60%,70%);}
#p5 {fon rangi: hsl(290,100%,50%);}
#p6 {fon rangi: hsl(290,60%,70%);}
</style>
</head>
<tana>

<h1>HSL qiymatlari bilan ranglarni aniqlang</h1>

<p id="p1">Yashil</p>
<p id="p2">Och yashil</p>
<p id="p3">To‘q yashil</p>
<p id="p4">Yashil pastel</p>
<p id="p5">Binafsha</p>
<p id="p6">Pastel binafsha</p>

</body>
</html>



HSLA ranglari

HSLA rang qiymatlari HSL rang qiymatlarining alfa-kanalli kengaytmasi bo'lib, shaffoflikni belgilaydi.

rang uchun.

HSLA rang qiymati quyidagi bilan belgilanadi: hsla(rang, toʻyinganlik, yorugʻlik, alfa), bu yerda alfa parametri

shaffoflikni belgilaydi. Alfa parametri 0,0 (to'liq shaffof) va 1,0 (to'liq shaffof) orasidagi raqamdir.

Turli xil HSLA ranglari uchun quyidagi misolga qarang:

<!DOCTYPE html>
<html>
<head>
<uslub>
#p1 {fon rangi: hsla(120,100%,50%,0,3);}
#p2 {fon rangi: hsla(120,100%,75%,0,3);}
#p3 {fon rangi: hsla (120,100%, 25%, 0,3);}
#p4 {fon rangi: hsla(120,60%,70%,0,3);}
#p5 {fon rangi: hsla(290,100%,50%,0,3);}
#p6 {fon rangi: hsla(290,60%,70%,0,3);}
</style>
</head>
<tana>

<h1>Ranglarni HSLA qiymatlari bilan aniqlang</h1>

<p id="p1">Yashil</p>
<p id="p2">Och yashil</p>
<p id="p3">To‘q yashil</p>
<p id="p4">Yashil pastel</p>
<p id="p5">Binafsha</p>
<p id="p6">Pastel binafsha</p>

</body>
</html>




Shaffoflik

CSS noaniqlik xususiyati butun element uchun shaffoflikni o'rnatadi (fon rangi ham, matn ham shunday bo'ladi).

shaffof/shaffof).

Shaffoflik xususiyati qiymati 0,0 (to'liq shaffof) va 1,0 (to'liq shaffof) orasidagi raqam bo'lishi kerak.

Yuqoridagi matnlar ham shaffof bo'ladi. Belgilangan shaffoflikka ega elementlar uchun quyidagi misolga qarang:


<!DOCTYPE html>
<html>
<head>
<uslub>
#p1 {fon rangi: rgb(255,0,0); shaffoflik: 0,6;}
#p2 {fon rangi:rgb(0,255,0); shaffoflik:0,6;}
#p3 {fon rangi: rgb(0,0,255); shaffoflik: 0,6;}
#p4 {fon rangi: rgb (192,192,192); shaffoflik: 0,6;}
#p5 {fon rangi: rgb(255,255,0); shaffoflik: 0,6;}
#p6 {fon rangi: rgb(255,0,255); shaffoflik: 0,6;}
</style>
</head>
<tana>

<h1>Ranglarni shaffofligi bilan aniqlang</h1>

<p id="p1">Qizil</p>
<p id="p2">Yashil</p>
<p id="p3">Moviy</p>
<p id="p4">Kulrang</p>
<p id="p5">Sariq</p>
<p id="p6">Cerise</p>

</body>
</html>


<kbd>qaytish</kbd>[Mundarijaga qaytish](#homepage)


-----------
## CSS chegaralari

CSS chegara uslubi

Chegara uslubi xossasi qanday chegarani ko'rsatishni belgilaydi.

Quyidagi qiymatlarga ruxsat beriladi:

nuqta - nuqta chegarasini belgilaydi
chiziqli - chiziqli chegarani belgilaydi
qattiq - qattiq chegarani belgilaydi
double - juft chegarani belgilaydi
groove - 3D yivli chegarani belgilaydi. Effekt chegara rangi qiymatiga bog'liq
ridge - 3D qirrali chegarani belgilaydi. Effekt chegara rangi qiymatiga bog'liq
inset - 3D ichki chegarani belgilaydi. Effekt chegara rangi qiymatiga bog'liq
outset - 3D boshlang'ich chegarani belgilaydi. Effekt chegara rangi qiymatiga bog'liq
none - Chegarani belgilamaydi
yashirin - Yashirin chegarani belgilaydi

Chegara uslubidagi xususiyat birdan to'rtgacha qiymatga ega bo'lishi mumkin (yuqori chegara, o'ng chegara, pastki chegara,

va chap chegara).


<!DOCTYPE html>
<html>
<head>
<uslub>
p.dotted {chegara uslubi: nuqta;}
p.dashed {chegara uslubi: chiziqcha;}
p.solid {chegara uslubi: qattiq;}
p.double {chegara uslubi: double;}
p.groove {chegara uslubi: groove;}
p.ridge {chegara uslubi: tizma;}
p.inset {chegara uslubi: inset;}
p.outset {chegara uslubi: boshlang'ich;}
p.none {chegara uslubi: yo'q;}
p.hidden {chegara uslubi: yashirin;}
p.mix {chegara uslubi: nuqtali chiziqli qattiq dubl;}
</style>
</head>
<tana>

<h2>Chegara uslubidagi xususiyat</h2>
<p>Bu xususiyat qanday chegarani ko'rsatishni belgilaydi:</p>

<p class="dotted">Nuqtali hoshiya.</p>
<p class="dashed">Chiziq chiziq.</p>
<p class="solid">Battiq chegara.</p>
<p class="double">Qo'shaloq chegara.</p>
<p class="groove">Yivik chegara.</p>
<p class="ridge">Tiz chegarasi.</p>
<p class="inset">O'rnatilgan chegara.</p>
<p class="outset">Boshlabki chegara.</p>
<p class="none">Chegara yo'q.</p>
<p class="hidden">Yashirin chegara.</p>
<p class="mix">Aralash chegara.</p>

</body>
</html>



Eslatma: BOSHQA CSS chegara xususiyatlaridan hech biri (chegara kengligi, chegara ranglari, chegara tomonlari, chegara kabi)

stenografiya, yumaloq chegaralar) chegara uslubi xususiyati o'rnatilmasa, HAR QANDAY ta'sirga ega bo'ladi!


Chegara kengligi::

<!DOCTYPE html>
<html>
<head>
<uslub>
p.bir {
   chegara uslubi: qattiq;
   chegara kengligi: 5px;
}

ikkinchi p. {
   chegara uslubi: qattiq;
   chegara kengligi: o'rtacha;
}

uchinchi p. {
   chegara uslubi: nuqta;
   chegara kengligi: 2px;
}

to'rt {
   chegara uslubi: nuqta;
   chegara kengligi: qalin;
}

bet {
   chegara uslubi: juftlik;
   chegara kengligi: 15px;
}

p.6 {
   chegara uslubi: juftlik;
   chegara kengligi: qalin;
}
</style>
</head>
<tana>

<h2>Chegara kengligi xossasi</h2>
<p>Bu xususiyat to'rtta chegaraning kengligini belgilaydi:</p>

<p class="one">Ba'zi matn.</p>
<p class="two">Ba'zi matn.</p>
<p class="three">Ba'zi matn.</p>
<p class="four">Ba'zi matn.</p>
<p class="five">Ba'zi matn.</p>
<p class="six">Ba'zi matn.</p>

<p><b>Eslatma:</b> "border-width" xususiyati, agar u yolg'iz ishlatilsa, ishlamaydi.
Avval chegaralarni belgilash uchun har doim “border-style” xususiyatini belgilang.</p>

</body>
</html>






CSS chegara kengligi

border-width xususiyati to‘rtta chegaraning kengligini belgilaydi (yuqori chegara, o‘ng chegara, pastki chegara,

va chap chegara) px, pt, sm, em va boshqalar yordamida yoki ingichka, o'rta yoki qalin. Muayyan yon kengliklari uchun ikkita

chegaralari belgilanadi. Birinchisi yuqori va pastki chegarani, ikkinchisi esa chegarani ifodalaydi

yon chegaralar uchun kenglik.



<!DOCTYPE html>
<html>
<head>
<uslub>
p.bir {
   chegara uslubi: qattiq;
   chegara kengligi: 5px 20px; /* yuqori va pastki 5px, yon tomonlarda 20px */
}

ikkinchi p. {
   chegara uslubi: qattiq;
   chegara kengligi: 20px 5px; /* yuqori va pastda 20px, yon tomonlarda 5px */
}

uchinchi p. {
   chegara uslubi: qattiq;
   chegara kengligi: 25px 10px 4px 35px; /* 25px tepada, 10px oʻngda, 4px pastda va 35px chapda */
}
</style>
</head>
<tana>

<h2>Chegara kengligi xossasi</h2>
<p>Chegara kengligi xususiyati birdan toʻrtgacha qiymatga ega boʻlishi mumkin (yuqori chegara, oʻng chegara, pastki uchun

chegara va chap chegara):</p>

<p class="one">Ba'zi matn.</p>
<p class="two">Ba'zi matn.</p>
<p class="three">Ba'zi matn.</p>

</body>
</html>

CSS chegara rangi::

Chegara rangi xususiyati nom (masalan, qizil), HEX qiymati yordamida to'rtta chegara rangini o'rnatish uchun ishlatiladi.

(masalan, #ff0000), RGB qiymati (masalan, rgb(255,0,0) va HSL qiymati (masalan, hsl (0, 100%, 50%)) va shaffoflik

(alfa qiymatidan foydalangan holda ko'rsatilgan).


Eslatma: Agar siz chegara rangini o'rnatmagan bo'lsangiz, elementlarning rangi standart chegara rangidir.

<!DOCTYPE html>
<html>
<head>
<uslub>
p.bir {
   chegara uslubi: qattiq;
   chegara rangi: qizil;
}

ikkinchi p. {
   chegara uslubi: qattiq;
   chegara rangi: yashil;
}

uchinchi p. {
   chegara uslubi: nuqta;
   chegara rangi: ko'k;
}
</style>
</head>
<tana>

<h2>Chegara rangi xususiyati</h2>
<p>Bu xususiyat to'rtta chegara rangini belgilaydi:</p>

<p class="one">Qizil chegara</p>
<p class="two">Yashil chegara</p>
<p class="three">Nuqtali ko'k hoshiya</p>

<p><b>Eslatma:</b> "border-color" xususiyati yolg'iz ishlatilsa ishlamaydi. "Chegara uslubi" dan foydalaning

avval chegaralarni belgilash uchun xususiyat.</p>

</body>
</html>



Maxsus yon ranglar


border-color xususiyati birdan toʻrtgacha qiymatga ega boʻlishi mumkin (yuqori chegara, oʻng chegara, pastki chegara,

va chap chegara).


<!DOCTYPE html>
<html>
<head>
<uslub>
p.bir {
   chegara uslubi: qattiq;
   chegara rangi: qizil yashil ko'k sariq; /* qizil tepa, yashil o'ng, ko'k pastki va sariq chap */
}
</style>
</head>
<tana>

<h2>Chegara rangi xususiyati</h2>
<p>chegara rangi xususiyati birdan toʻrtgacha qiymatga ega boʻlishi mumkin (yuqori chegara, oʻng chegara, pastki uchun

chegara va chap chegara):</p>

<p class="one">Yaxshi ko'p rangli hoshiya</p>

</body>
</html>


O'n oltilik (HEX) qiymatlari

Chegaraning rangi HEX qiymatlari yordamida ham aniqlanishi mumkin.


<!DOCTYPE html>
<html>
<head>
<uslub>
p.bir {
   chegara uslubi: qattiq;
   chegara rangi: #ff0000; /* qizil */
}

ikkinchi p. {
   chegara uslubi: qattiq;
   chegara rangi: #0000ff; /* ko'k */
}

uchinchi p. {
   chegara uslubi: qattiq;
   chegara rangi: #bbbbbb; /* kulrang */
}
</style>
</head>
<tana>

<h2>Chegara rangi xususiyati</h2>
<p>Chegara rangini oʻn oltilik qiymat (HEX) yordamida ham belgilash mumkin:</p>

<p class="one">Qizil chegara</p>
<p class="two">Yagona ko'k hoshiya</p>
<p class="three">Yaxlit kulrang hoshiya</p>

</body>
</html>



RGB qiymatlari

RGB qiymatlari rangni belgilash uchun ham ishlatilishi mumkin.

<!DOCTYPE html>
<html>
<head>
<uslub>
p.bir {
   chegara uslubi: qattiq;
   chegara rangi: rgb(255, 0, 0); /* qizil */
}

ikkinchi p. {
   chegara uslubi: qattiq;
   chegara rangi: rgb(0, 0, 255); /* ko'k */
}

uchinchi p. {
   chegara uslubi: qattiq;
   chegara rangi: rgb(187, 187, 187); /* kulrang */
}
</style>
</head>
<tana>

<h2>Chegara rangi xususiyati</h2>
<p>Chegara rangini RGB qiymatlari yordamida ham belgilash mumkin:</p>

<p class="one">Qizil chegara</p>
<p class="two">Yagona ko'k hoshiya</p>
<p class="three">Yaxlit kulrang hoshiya</p>

</body>
</html>


HSL qiymatlari

HSL qiymatlari belgilash uchun ishlatilishi mumkin.

<!DOCTYPE html>
<html>
<head>
<uslub>
p.bir {
   chegara uslubi: qattiq;
   chegara rangi: hsl(0, 100%, 50%); /* qizil */
}

ikkinchi p. {
   chegara uslubi: qattiq;
   chegara rangi: hsl(240, 100%, 50%); /* ko'k */
}

uchinchi p. {
   chegara uslubi: qattiq;
   chegara rangi: hsl(0, 0%, 73%); /* kulrang */
}
</style>
</head>
<tana>

<h2>Chegara rangi xususiyati</h2>
<p>Chegara rangini HSL qiymatlari yordamida ham belgilash mumkin:</p>

<p class="one">Qizil chegara</p>
<p class="two">Yagona ko'k hoshiya</p>
<p class="three">Yaxlit kulrang hoshiya</p>

</body>
</html>



CSS chegara tomonlari::

CSS chegarasi - individual tomonlar

Har bir tomon (yuqori, o'ng, pastki va chap) chegara turini belgilash uchun ba'zi CSS xususiyatlaridan foydalanishingiz mumkin

<!DOCTYPE html>
<html>
<head>
<uslub>
p {
   chegara tepasi uslubi: nuqta;
   chegara o'ng uslubi: qattiq;
   chegara-pastki uslub: nuqta;
   chegara-chap uslubi: qattiq;
}
</style>
</head>
<tana>

<h2>Alohida chegara tomonlari</h2>
<p>2 xil chegara uslubi.</p>

</body>
</html>


Yuqoridagi kodni shunday yozish ham mumkin (nuqta va qattiq mos ravishda yuqori+past va chap+o‘ngni ifodalaydi:

<!DOCTYPE html>
<html>
<head>
<uslub>
p {
   chegara uslubi: nuqtali qattiq;
}
</style>
</head>
<tana>

<h2>Alohida chegara tomonlari</h2>
<p>2 xil chegara uslubi.</p>

</body>
</html>


Chegara uslubini tushuntirish:
Agar chegara uslubidagi xususiyat to'rtta qiymatga ega bo'lsa:

     chegara uslubi: nuqtali qattiq qo'sh chiziqli;
         yuqori chegarasi nuqtali
         o'ng chegara mustahkam
         pastki chegara ikki barobar
         chap chegara chizilgan

Agar chegara uslubidagi xususiyat uchta qiymatga ega bo'lsa:

     chegara uslubi: nuqtali qattiq juftlik;
         yuqori chegarasi nuqtali
         o'ng va chap chegaralar mustahkam
         pastki chegara ikki barobar

Agar chegara uslubidagi xususiyat ikkita qiymatga ega bo'lsa:

     chegara uslubi: nuqtali qattiq;
         yuqori va pastki chegaralari nuqtali
         o'ng va chap chegaralar mustahkam

Agar chegara uslubidagi xususiyat bitta qiymatga ega bo'lsa:

     chegara uslubi: nuqta;
         barcha to'rtta chegara nuqtali


Yuqoridagilar chegara kengligi va chegara rangi bilan ham ishlaydi

Chegara uslubi parametrlaridan amaliy foydalanish misoli uchun quyidagi kodga qarang

<!DOCTYPE html>
<html>
<head>
<uslub>
tana {
   matnni tekislash: markaz;
}
/* To'rt qiymat */
to'rt {
   chegara uslubi: nuqtali qattiq qo'sh chiziqli;
}

/* Uchta qiymat */
uchinchi p. {
   chegara uslubi: nuqtali qattiq juftlik;
}

/* Ikki qiymat */
ikkinchi p. {
   chegara uslubi: nuqtali qattiq;
}

/* Bitta qiymat */
p.bir {
   chegara uslubi: nuqta;
}
</style>
</head>
<tana>

<h2>Alohida chegara tomonlari</h2>
<p class="four">4 xil chegara uslubi.</p>
<p class="three">3 xil chegara uslubi.</p>
<p class="two">2 xil chegara uslubi.</p>
<p class="one">1 ta chegara uslubi.</p>

</body>
</html>

CSS Border-Shorthand xususiyati::
Chegara uslublari kodlarini qisqartirishni yoqing. "Chegara" xususiyati individual chegaraning qisqartmasi hisoblanadi

xususiyatlari, quyida ko'rsatilganidek (masalan)


     chegara kengligi
     chegara uslubi (majburiy)
     chegara rangi
<!DOCTYPE html>
<html>
<head>
<uslub>
p {
   chegara: 5px qattiq qizil;
}
</style>
</head>
<tana>

<h2>Chegara xususiyati</h2>

<p>Bu xususiyat chegara kengligi, hoshiya uslubi va hoshiya rangi uchun stenografiya xususiyatidir.</p>

</body>
</html>



Chegara xususiyatlari har bir tomon uchun ham belgilanishi mumkin:
<!DOCTYPE html>
<html>
<head>
<uslub>
p {
   chegara-chap: 6px qattiq qizil;
   fon rangi: och kulrang;
}
</style>
</head>
<tana>

<h2>Chap chegarasidagi xususiyat</h2>
<p>Bu xususiyat chegara-chap-kenglik, chegara-chap-uslubi va chegara-chap- uchun stenografiya xususiyatidir.

rang.</p>

</body>
</html>

To repeat the same for bottom border:

<!DOCTYPE html>
<html>
<head>
<style>
p {
  border-bottom: 6px solid red;
  background-color: lightgrey;
}
</style>
</head>
<body>

<h2>The border-bottom Property</h2>
<p>This property is a shorthand property for border-bottom-width, border-bottom-style, and border-bottom-

color.</p>

</body>
</html>


CSS Rounded Borders::
Use border radius to add rounded borders to an element


<!DOCTYPE html>
<html>
<head>
<style>
p.normal {
  border: 2px solid red;
}

p.round1 {
  border: 2px solid red;
  border-radius: 5px;
}

p.round2 {
  border: 2px solid red;
  border-radius: 8px;
}

p.round3 {
  border: 2px solid red;
  border-radius: 12px;
}
</style>
</head>
<body>

<h2>The border-radius Property</h2>
<p>This property is used to add rounded borders to an element:</p>

<p class="normal">Normal border</p>
<p class="round1">Round border</p>
<p class="round2">Rounder border</p>
<p class="round3">Roundest border</p>

</body>
</html>


NB: Some shortcuts on border styling

To set all properties of top border in one go:
<!DOCTYPE html>
<html>
<head>
<style>
p {
  border-style: solid;
  border-top: thick double #ff0000;
}
</style>
</head>
<body>

<p>This is some text in a paragraph.</p>

</body>
</html>


To set the style of the bottom border

<!DOCTYPE html>
<html>
<head>
<style>
p {border-style: solid;}
p.none {border-bottom-style: none;}
p.dotted {border-bottom-style: dotted;}
p.dashed {border-bottom-style: dashed;}
p.solid {border-bottom-style: solid;}
p.double {border-bottom-style: double;}
p.groove {border-bottom-style: groove;}
p.ridge {border-bottom-style: ridge;}
p.inset {border-bottom-style: inset;}
p.outset {border-bottom-style: outset;}
</style>
</head>
<body>

<p class="none">No bottom border.</p>
<p class="dotted">A dotted bottom border.</p>
<p class="dashed">A dashed bottom border.</p>
<p class="solid">A solid bottom border.</p>
<p class="double">A double bottom border.</p>
<p class="groove">A groove bottom border.</p>
<p class="ridge">A ridge bottom border.</p>
<p class="inset">An inset bottom border.</p>
<p class="outset">An outset bottom border.</p>

</body>
</html>



Chap chegaraning kengligini o'rnatish uchun

<!DOCTYPE html>
<html>
<head>
<uslub>
p {
   chegara uslubi: qattiq;
   chegara-chap-kengligi: 15px;
}
</style>
</head>
<tana>

<p><b>Eslatma:</b> "chegara-chap-kenglik" xususiyati, agar u yolg'iz ishlatilsa, ishlamaydi. "Chegara uslubi" dan foydalaning

avval chegaralarni belgilash uchun xususiyat.</p>

</body>
</html>


To'rtta chegara rangini o'rnatish uchun:

<!DOCTYPE html>
<html>
<head>
<uslub>
p.bir {
   chegara uslubi: qattiq;
  
   chegara rangi: #0000ff;
}

ikkinchi p. {
   chegara uslubi: qattiq;
   chegara rangi: #ff0000 #0000ff;
}

uchinchi p. {
   chegara uslubi: qattiq;
   chegara rangi: #ff0000 #00ff00 #0000ff;
}

to'rt {
   chegara uslubi: qattiq;
   chegara rangi: #ff0000 #00ff00 #0000ff rgb(250,0,255);
}
</style>
</head>
<tana>

<p class="one">Bir rangli hoshiya!</p>
<p class="two">Ikki rangli hoshiya!</p>
<p class="three">Uch rangli hoshiya!</p>
<p class="four">To'rt rangli hoshiya!</p>
<p><b>Eslatma:</b> "border-color" xususiyati yolg'iz ishlatilsa ishlamaydi. "Chegara uslubi" dan foydalaning

avval chegaralarni belgilash uchun xususiyat.</p>

</body>
</html>


O'ng chegara rangini o'rnatish uchun:
<!DOCTYPE html>
<html>
<head>
<uslub>
p {
   chegara uslubi: qattiq;
   chegara-o'ng-rang: #ff0000;
}
</style>
</head>
<tana>

<p>Bu xatboshidagi ayrim matn.</p>

</body>
</html>


Barcha CSS chegara xususiyatlari
Mulk tavsifi
border Barcha chegara xususiyatlarini bitta deklaratsiyada o'rnatadi
border-bottom Barcha pastki chegara xususiyatlarini bitta deklaratsiyada o'rnatadi
border-bottom-color Pastki chegara rangini o'rnatadi
border-bottom-style Pastki chegara uslubini o'rnatadi
border-bottom-width Pastki chegaraning kengligini o'rnatadi
border-color Toʻrtta chegara rangini oʻrnatadi
border-left Barcha chap chegara xususiyatlarini bitta deklaratsiyada o'rnatadi
border-left-color Chap chegara rangini o'rnatadi
border-left-style Chap chegara uslubini o'rnatadi
border-left-width Chap chegaraning kengligini o'rnatadi
border-radius Yumaloq burchaklar uchun to'rtta chegara-*-radius xususiyatlarini o'rnatadi
border-right Bitta deklaratsiyada barcha to'g'ri chegara xususiyatlarini o'rnatadi
border-right-color Oʻng chegara rangini oʻrnatadi
border-right-style O'ng chegara uslubini o'rnatadi
border-right-width Oʻng chegaraning kengligini oʻrnatadi
border-style To'rtta hoshiya uslubini o'rnatadi
border-top Bitta deklaratsiyada barcha yuqori chegara xususiyatlarini o'rnatadi
border-top-color Yuqori chegara rangini o'rnatadi
border-top-style Yuqori chegara uslubini o'rnatadi
border-top-width Yuqori chegaraning kengligini o'rnatadi
border-width To'rtta chegaraning kengligini o'rnatadi

<kbd>qaytish</kbd>[Mundarijaga qaytish](#homepage)

-----
## CSS chegaralari

Belgilangan chegaralardan tashqarida element atrofida bo'sh joy yaratish uchun. "marja" marja ustidan nazoratni beradi

element atrofida. Shuningdek, siz to'rt tomondan chekka o'rnatishingiz mumkin. Chegarani o'rnatish uchun xususiyatlar mavjud

elementning har bir tomoni uchun (yuqori, o'ng, pastki va chap).

Quyidagi kod <p> elementi atrofida 70px bo'sh joy qo'shadi.

<!DOCTYPE html>
<html>
<head>
<uslub>
div {
   chegara: 70px;
   chegara: 1px qattiq #4CAF50;
}
</style>
</head>
<tana>

<h2>CSS chegaralari</h2>
<div>Ushbu element 70px chetiga ega.</div>

</body>
</html>



Chegara - Individual tomonlar::

CSS elementning har bir tomoni uchun chegarani belgilash uchun xususiyatlarga ega:

     chekka tepa
     chekka o'ng
     chekka-pastki
     chekka-chap

Barcha marj xususiyatlari quyidagi qiymatlarga ega bo'lishi mumkin:

     avtomatik - brauzer chegarani hisoblab chiqadi
     uzunlik - px, pt, sm va hokazolarda chegarani belgilaydi.
     % - o'z ichiga olgan element kengligining % da chetini belgilaydi
     inherit - chekka asosiy elementdan meros bo'lishi kerakligini bildiradi

Maslahat: Salbiy qiymatlarga ruxsat beriladi.

<!DOCTYPE html>
<html>
<head>
<uslub>
div {
   chegara: 1px qattiq qora;
   yuqori chegara: 100px;
   pastki chet: 100px;
   chekka o'ng: 150px;
   chap chekka: 80px;
   fon rangi: ochiq ko'k;
}
</style>
</head>
<tana>

<h2>Alohida chegara xususiyatlaridan foydalanish</h2>

<div>Ushbu div elementining yuqori cheti 100px, oʻng tomoni 150px, pastki cheti 100px va

chap cheti 80px.</div>

</body>
</html>



Margin stenografiya xususiyati

Kodni qisqartirish uchun barcha chegara xususiyatlarini bitta xususiyatda ko'rsatish mumkin.

Margin xususiyati quyidagi individual marja xususiyatlari uchun stenografiya xususiyatidir:

     chekka tepa
     chekka o'ng
     chekka-pastki
     chekka-chap

Shunday qilib, bu qanday ishlaydi:

Agar margin xususiyati to'rtta qiymatga ega bo'lsa:

     hoshiya: 25px 50px 75px 100px;
         yuqori chegarasi 25px
         o'ng cheti 50px
         pastki cheti 75px
         chap chekka 100px


Misol:

<!DOCTYPE html>
<html>
<head>
<uslub>
div {
   chegara: 1px qattiq qora;
   hoshiya: 25px 50px 75px 100px;
   fon rangi: ochiq ko'k;
}
</style>
</head>
<tana>

<h2>Marja stenografiya xususiyati - 4 ta qiymat</h2>

<div>Ushbu div elementining yuqori cheti 25px, oʻng tomoni 50px, pastki cheti 75px va chap tomoni bor

chegarasi 100px.</div>

<hr>

</body>
</html>


Agar margin xususiyati uchta qiymatga ega bo'lsa:

     hoshiya: 25px 50px 75px;
         yuqori chegarasi 25px
         o'ng va chap chekkalar 50px
         pastki cheti 75px

<!DOCTYPE html>
<html>
<head>
<uslub>
div {
   chegara: 1px qattiq qora;
   hoshiya: 25px 50px 75px;
   fon rangi: ochiq ko'k;
}
</style>
</head>
<tana>

<h2>Marja stenografiya xususiyati - 3 ta qiymat</h2>

<div>Ushbu div elementining yuqori cheti 25px, oʻng va chap chetlari 50px va pastki chetlari:

75px.</div>

<hr>

</body>
</html>


Agar margin xususiyati ikkita qiymatga ega bo'lsa:

     chegara: 25px 50px;
         yuqori va pastki chetlari 25px
         o'ng va chap chekkalar 50px


<!DOCTYPE html>
<html>
<head>
<uslub>
div {
   chegara: 1px qattiq qora;
   chegara: 25px 50px;
   fon rangi: ochiq ko'k;
}
</style>
</head>
<tana>

<h2>Marja stenogramma xususiyati - 2 qiymat</h2>

<div>Ushbu div elementining yuqori va pastki chetlari 25px, oʻng va chap chetlari esa 50px.</div>

<hr>

</body>
</html>



Agar margin xususiyati bitta qiymatga ega bo'lsa:

     chekka: 25px;
         to'rtta chekkaning hammasi 25px




<!DOCTYPE html>
<html>
<head>
<uslub>
div {
   chegara: 1px qattiq qora;
   chegara: 25px;
   fon rangi: ochiq ko'k;
}
</style>
</head>
<tana>

<h2>Marja stenografiya xususiyati - 1 qiymat</h2>

<div>Ushbu div elementining yuqori, pastki, chap va oʻng chetlari 25px.</div>

<hr>

</body>
</html>




Chegara: avtomatik, qiymat

Elementni konteyner ichida gorizontal markazlashtirish uchun margin xususiyatini avtomatik qilib sozlashingiz mumkin.

Keyin element belgilangan kenglikni egallaydi va qolgan bo'sh joy teng ravishda bo'linadi

chap va o'ng chetlari.


<!DOCTYPE html>
<html>
<head>
<uslub>
div {
   kengligi: 300px;
   chegara: avtomatik;
   chegara: 1px qattiq qizil;
}
</style>
</head>
<tana>

<h2>Marjadan foydalanish:avto</h2>
<p>Elementni konteyner ichida gorizontal markazlashtirish uchun margin xususiyatini avtomatik qilib sozlashingiz mumkin. The

keyin element belgilangan kenglikni egallaydi va qolgan bo'sh joy o'rtasida teng ravishda bo'linadi

chap va o'ng chetlari:</p>

<div>
Bu div gorizontal markazlashtirilgan bo'ladi, chunki uning chegarasi bor: auto;
</div>

</body>
</html>
Marja uchun meros qiymati
<p class="ex1"> elementining chap chetiga asosiy elementdan meros qilib olinishiga ruxsat berish.


<!DOCTYPE html>
<html>
<head>
<uslub>
div {
   chegara: 1px qattiq qizil;
   chap chekka: 100px;
}

p.ex1 {
   margin-left: meros;
}
</style>
</head>
<tana>

<h2> Meros qiymatidan foydalanish</h2>
<p>Chap chekka asosiy elementdan meros bo'lsin:</p>

<div>
<p class="ex1">Ushbu paragraf meros qilib olingan chap chetiga ega (div elementidan).</p>
</div>

</body>
</html>


CSS chegarasini yig'ish::
2 ta chetni bittaga yig'ish imkonini beradi.

Chegaraning siqilishi

Elementlarning yuqori va pastki chetlari ba'zan eng kattasiga teng bo'lgan bitta chekkaga yig'iladi

ikki chetidan.

Bu chap va o'ng chekkalarda sodir bo'lmaydi! Faqat yuqori va pastki chegaralar!


<!DOCTYPE html>
<html>
<head>
<uslub>
h1 {
   chegara: 0 0 50px 0;
}

h2 {
   chegara: 20px 0 0 0;
}
</style>
</head>
<tana>

<p>Ushbu misolda h1 elementining pastki chegarasi 50px va h2 elementining yuqori chegarasi 20px.

Shunday qilib, h1 va h2 orasidagi vertikal chegara 70px (50px + 20px) bo'lishi kerak edi. Biroq, marj tufayli

siqilsa, haqiqiy chegara 50px boʻladi.</p>

<h1>1-sarlavha</h1>
<h2>2-sarlavha</h2>

</body>
</html>


Yuqoridagi misolda <h1> elementi pastki chetiga 50px, <h2> elementi esa yuqori chegaraga ega.

20px gacha.

Sog'lom fikr <h1> va <h2> orasidagi vertikal chegara jami bo'lishini taxmin qiladi.

70px (50px + 20px). Ammo marjaning yiqilishi tufayli haqiqiy chegara 50px ni tashkil qiladi.



Barcha CSS Margin xususiyatlari
Mulk tavsifi
margin Bitta deklaratsiyada chegara xususiyatlarini o'rnatish uchun stenografiya xususiyati
margin-bottom Elementning pastki chetini o'rnatadi
margin-left Elementning chap chetini o'rnatadi
margin-right Elementning o'ng chetini o'rnatadi
margin-top Elementning yuqori chetini o'rnatadi

<kbd>qaytish</kbd>[Mundarijaga qaytish](#homepage)

-----



## CSS to'ldirish

CSS "padding" har qanday belgilangan chegaralar ichida element tashqarisida bo'shliqlar yaratish uchun ishlatiladi. CSS paddingdan foydalanish uchun,

misol uchun pastga qarang. CSS elementining barcha to'rt tomoni uchun to'ldirishni o'rnatish uchun CSS-dan foydalanishingiz mumkin.

<!DOCTYPE html>
<html>
<head>
<uslub>
div {
   to'ldirish: 100px;
   chegara: 1px qattiq #4CAF50;
}
</style>
</head>
<tana>

<h2>CSS padding</h2>
<div>Ushbu element 70px hajmga ega.</div>

</body>
</html>



To'ldirish - individual tomonlar


CSS elementning har bir tomoni uchun to'ldirishni belgilash uchun xususiyatlarga ega:

     to'ldiruvchi
     to'ldirish - o'ng
     to'ldirish - pastki
     to'ldirish - chap

Barcha to'ldirish xususiyatlari quyidagi qiymatlarga ega bo'lishi mumkin:

     uzunlik - px, pt, sm va hokazolarda to'ldirishni belgilaydi.
     % - o'z ichiga olgan element kengligining % da to'ldirishni belgilaydi
     inherit - to'ldirish asosiy elementdan meros bo'lishi kerakligini bildiradi

Eslatma: Salbiy qiymatlarga ruxsat berilmaydi.


To'rt tomondan to'ldirgichdan foydalanish uchun foydalanish misoli uchun quyida ko'ring:

<!DOCTYPE html>
<html>
<head>
<uslub>
div {
   chegara: 1px qattiq qora;
   fon rangi: ochiq ko'k;
   to'ldirish tepasi: 50px;
   to'ldirish - o'ng: 30px;
   pastki qism: 50px;
   padding-chap: 80px;
}
</style>
</head>
<tana>

<h2>Alohida to'ldirish xususiyatlaridan foydalanish</h2>

<div>Ushbu div elementining yuqori toʻldirgichi 50px, oʻng tomoni 30px, pastki qismi 50px va

80px chap toʻldirish.</div>

</body>
</html>




Padding - stenografiya xususiyati

Bu xususiyatlar bitta xususiyatda to'ldirish xususiyatlarini qisqartirishga imkon beradi. Masalan:


To'ldirish xususiyati quyidagi individual to'ldirish xususiyatlari uchun qisqartma xususiyatdir:

     to'ldiruvchi-usti
     to'ldirish - o'ng
     to'ldirish - pastki
     to'ldirish - chap

Shunday qilib, bu qanday ishlaydi:

Agar to'ldirish xususiyati to'rtta qiymatga ega bo'lsa:

     to'ldirish: 25px 50px 75px 100px;
         yuqori to'ldirish - 25px
         o'ng to'ldirish 50px
         pastki to'ldirish - 75px
         chap to'ldirish 100px


Masalan:

<!DOCTYPE html>
<html>
<head>
<uslub>
div {
   chegara: 1px qattiq qora;
   to'ldirish: 25px 50px 75px 100px;
   fon rangi: ochiq ko'k;
}
</style>
</head>
<tana>

<h2>To'ldirish stenografiyasi xususiyati - 4 ta qiymat</h2>

<div>Ushbu div elementining yuqori toʻldirgichi 25px, oʻng tomoni 50px, pastki qismi 75px va

100px chap toʻldirish.</div>

</body>
</html>


Uch qiymatga ega bo'lgan to'ldirish xususiyatlari uchun:

Agar padding xususiyati uchta qiymatga ega bo'lsa:

     to'ldirish: 25px 50px 75px;
         yuqori to'ldirish - 25px
         o'ng va chap to'ldirishlar 50px
         pastki to'ldirish - 75px


Masalan,


<!DOCTYPE html>
<html>
<head>
<uslub>
div {
   chegara: 1px qattiq qora;
   to'ldirish: 25px 50px 75px;
   fon rangi: ochiq ko'k;
}
</style>
</head>
<tana>

<h2>To'ldirish stenografiyasi xususiyati - 3 ta qiymat</h2>

<div>Ushbu div elementi 25px yuqori toʻldirishga, oʻng va chapga 50px va pastki toʻldirishga ega.

75px.</div>

</body>
</html>




Ikki qiymatli toʻldirish xususiyatlari uchun,

Agar padding xususiyati ikkita qiymatga ega bo'lsa:

     to'ldirish: 25px 50px;
         yuqori va pastki to'ldirishlar 25px
         o'ng va chap to'ldirishlar 50px


Masalan:

<!DOCTYPE html>
<html>
<head>
<uslub>
div {
   chegara: 1px qattiq qora;
   to'ldirish: 25px 50px;
   fon rangi: ochiq ko'k;
}
</style>
</head>
<tana>

<h2>To'ldirish stenografiyasi xususiyati - 2 ta qiymat</h2>

<div>Ushbu div elementining yuqori va pastki toʻldirgichlari 25px, oʻng va chap tomonlari esa 50px.</div>

</body>
</html>



Agar padding xususiyati bitta qiymatga ega bo'lsa:

Agar padding xususiyati bitta qiymatga ega bo'lsa:

     to'ldirish: 25px;
         to'rtta to'ldirishning hammasi 25px


Masalan,
<!DOCTYPE html>
<html>
<head>
<uslub>
div {
   chegara: 1px qattiq qora;
   to'ldirish: 25px;
   fon rangi: ochiq ko'k;
}
</style>
</head>
<tana>

<h2>To'ldirish stenografiyasi xususiyati - 1 qiymat</h2>

<div>Ushbu div elementi 25px yuqori, pastki, chap va oʻng toʻldirishga ega.</div>

</body>
</html>




To'ldirish va element kengligi

Kenglik elementi elementning kontent maydonining kengligini belgilaydi (to'ldirish, chegara va chekka ichidagi maydon)

quti modeliga muvofiq elementning). Belgilangan kenglikdagi element uchun bunday to'ldirish

element belgilangan kenglik qiymatiga qo'shiladi (ko'pincha istalmagan natija).


Masalan,
<!DOCTYPE html>
<html>
<head>
<uslub>
div.ex1 {
   kengligi: 300px;
   fon rangi: sariq;
}

div.ex2 {
   kengligi: 300px;
   to'ldirish: 25px;
   fon rangi: ochiq ko'k;
}
</style>
</head>
<tana>

<h2>To'ldirish va element kengligi</h2>

<div class="ex1">Bu div kengligi 300px.</div>
<br>

<div class="ex2">Ushbu divning kengligi CSS-da 300px sifatida belgilangan boʻlsa ham, 350px.</div>

</body>
</html>


Kenglikni saqlashingiz kerak bo'lganda, box-sizing xususiyati kenglikdan qat'i nazar, doimiylikni saqlash uchun ishlatiladi.

to'ldirish miqdori. Bu ta'sir element uchun mavjud bo'sh joyni aniqlanganning ichkarisiga qisqartiradi

chegaralar.

 
Masalan.

<!DOCTYPE html>
<html>
<head>
<uslub>
div.ex1 {
   kengligi: 300px;
   fon rangi: sariq;
}

div.ex2 {
   kengligi: 300px;
   to'ldirish: 25px;
   quti o'lchami: chegara qutisi;
   fon rangi: ochiq ko'k;
}
</style>
</head>
<tana>

<h2>To'ldirish va element kengligi - quti o'lchami bilan</h2>

<div class="ex1">Bu div kengligi 300px.</div>
<br>

<div class="ex2">Ushbu divning kengligi chap va o'ngning umumiy soni 50px bo'lishiga qaramay, 300px da qoladi.

padding, box-sizing: border-box xususiyati tufayli.
</div>

</body>
</html>



Boshqa to'ldirish misollari,


Elementning chap toʻldirishini oʻrnatish uchun,


<!DOCTYPE html>
<html>
<head>
<uslub>
p.padding {
   to'ldirish - chap: 2 sm;
}
p.padding2 {
   to'ldirish-chap: 50%;
}
</style>
</head>
<tana>

<h1>chap to'ldirish xususiyati</h1>

<p>Bu matn chap toʻldirishsiz.</p>
<p class="padding">Ushbu matnning chap tomoni 2 sm.</p>
<p class="padding2">Ushbu matnning chap qismi 50% ni tashkil etadi.</p>

</body>
</html>



To'g'ri to'ldirishni o'rnatish uchun,

<!DOCTYPE html>
<html>
<head>
<uslub>
p.padding {
   to'ldirish - o'ng: 2 sm;
}

p.padding2 {
   to'ldirish - o'ng: 50%;
}
</style>
</head>
<tana>

<h1>To'ldirish-o'ng xususiyati</h1>

<p>Bu toʻgʻri toʻldirilmagan matn. Bu to'g'ri to'ldirishsiz matn. Bu huquqsiz matn

to'ldirish.</p>
<p class="padding">Ushbu matnning o'ng tomoni 2 sm hajmga ega. Ushbu matn 2 sm o'ng to'ldirishga ega. Ushbu matn

2 sm o'ng yostig'i bor.</p>
<p class="padding2">Ushbu matnning o'ng tomoni 50% to'ldirilgan. Ushbu matn 50% o'ng to'ldirishga ega. Ushbu matn

50% oʻng toʻldirishga ega.</p>

</body>
</html>


Yuqori to'ldirishni o'rnatish uchun,

<!DOCTYPE html>
<html>
<head>
<uslub>
p.padding {
   to'ldiruvchi ustki qismi: 2 sm;
}

p.padding2 {
   to'ldiruvchi - 50%;
}
</style>
</head>
<tana>

<h1>To'ldiruvchi ustki xususiyat</h1>

<p>Bu yuqori toʻldirishsiz matn. Bu yuqori toʻldirishsiz matn. Bu tepada bo'lmagan matn

to'ldirish.</p>
<p class="padding">Ushbu matnning ustki qismi 2 sm. Ushbu matnning yuqori qismi 2 sm. Ushbu matnda mavjud

2 sm yuqori qoplama.</p>
<p class="padding2">Ushbu matn 50% yuqori toʻldirishga ega. Bu matn 50% yuqori toʻldirishga ega. Ushbu matnda mavjud

yuqori toʻldirish 50%.</p>

</body>
</html>

Pastki qoplamani o'rnatish uchun,


<!DOCTYPE html>
<html>
<head>
<uslub>
p.padding {
   to'ldirish - pastki: 2 sm;
}

p.padding2 {
   to'ldirish-pastki: 50%;
}
</style>
</head>
<tana>

<h1>To'ldiruvchi-pastki xususiyat</h1>

<p>Bu matnning pastki qismi boʻlmagan matn. Bu pastki toʻldirishsiz matn. Bu raqam bilan yozilgan matn

pastki to'ldirish.</p>
<p class="padding">Ushbu matnning pastki qismi 2 sm. Ushbu matnning pastki qismi 2 sm. Ushbu matn

pastki qoplamasi 2 sm.</p>
<p class="padding2">Ushbu matnning pastki qismi 50% toʻldirilgan. Ushbu matnning pastki qismi 50% ni tashkil qiladi. Ushbu matn

50% pastki to'ldirishga ega.</p>

</body>
</html>



Barcha CSS padding xususiyatlarining xulosasi
Mulk tavsifi
padding Bitta deklaratsiyada barcha to'ldirish xususiyatlarini o'rnatish uchun stenografiya xususiyati
padding-bottom Elementning pastki toʻldirishini oʻrnatadi
padding-left Elementning chap toʻldirishini oʻrnatadi
padding-right Elementning toʻgʻri toʻldirishini oʻrnatadi
padding-top Elementning yuqori toʻldirishini oʻrnatadi

<kbd>qaytish</kbd>[Mundarijaga qaytish](#homepage)