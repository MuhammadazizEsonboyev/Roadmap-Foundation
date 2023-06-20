## HTML FORMATLASH
```
<b> - Qalin matn
<strong> - Muhim matn
<i> - kursiv matn...koʻpincha texnik atama, boshqa tildagi ibora, fikr, kema nomi va hokazolarni koʻrsatish uchun ishlatiladi.
<em> - ta'kidlangan matn. Ekranni o'quvchi matnni og'zaki stress yordamida ta'kidlaydi
<belgi> - Belgilangan matn. Belgilanishi kerak bo'lgan element. Rangni o'zgartirish uchun uslubdan foydalanishingiz mumkin.
<kichik> - kichikroq matn
<del> - o'chirilgan matn. Brauzerlar odatda bir qatorga o'tadi
<ins> - Kiritilgan matn... (hujjatga) Brauzerlar odatda buni tagiga chizadilar. Del dan keyin foydalanish mumkin.
<sub> - Subscript matni... oddiy satrdan yarim belgi ostida paydo bo'ladi
<sup> - Yuqori skript matni... izohlarga iqtibos keltirish uchun ishlatilishi mumkin
```
```
*<p>My favorite color is <del>blue</del> <ins>red</ins>.</p>
```
<kbd>return</kbd>[Mundarijaga qaytish](#homepage)


--------------


## HTML IQTISODIYoTI
HTML IQTISODIYoTI VA IQTISODIYoTI Elementlari
```
<abbr> Qisqartma yoki qisqartmani belgilaydi. Ularni belgilash brauzerlar, tarjima tizimlari va qidiruv tizimlariga ma'lumot beradi. Qisqartmaning to'liq ma'nosini ko'rsatish uchun u bilan global atribut sarlavhasidan foydalaning.
<adres> Hujjat yoki maqola muallifi/egasi uchun aloqa ma'lumotlarini belgilaydi. Bu e-pochta, url, jismoniy, mobil raqam, ijtimoiy media tutqichlari va boshqalar bo'lishi mumkin. Brauzerlar <adres> elementidan oldin va keyin qatorlarni qo'shadilar.
<bdo> Matn yoʻnalishini belgilaydi. Joriy matn yoʻnalishini bekor qilish uchun ishlatiladi
<blockquote> Boshqa manbadan keltirilgan bo'limni belgilaydi. Brauzer odatda buni cheklaydi. cite bu erda href emas, manbani ko'rsatish uchun ishlatiladi.
<cite> Ijodiy ish nomini belgilaydi. Ijodkor nomi sarlavha emas. Brauzerlar odatda bu elementni kursiv bilan keltiradilar
<q> Qisqa chiziqli tirnoqni belgilaydi. Brauzer tirnoq atrofida qo'shtirnoq qo'yadi.
```
* Iqtibos
```
<p>Bu yerda WWF veb-saytidan iqtibos:</p>
<blockquote cite="http://www.worldwildlife.org/who/index.html">
50 yil davomida WWF tabiat kelajagini himoya qilib keladi.
Tabiatni muhofaza qilish bo‘yicha dunyodagi yetakchi tashkilot,
WWF 100 ta mamlakatda ishlaydi va tomonidan qo'llab-quvvatlanadi
Qo'shma Shtatlarda 1,2 million a'zo va
dunyo bo'ylab 5 millionga yaqin.
</blockquote>
```
* Qisqa iqtiboslar
```
 <p>WWF's goal is to: <q>Build a future where people live in harmony with nature.</q></p> 
```
* Qisqartirishdan foydalanish ```<abbr>```
```
<p>The <abbr title="World Health Organization">WHO</abbr> was founded in 1948.</p> 
```
Manzil
```
<address>
Jon Doe tomonidan yozilgan.<br>
Bizga tashrif buyuring:<br>
Misol.com<br>
Box 564, Disneylend<br>
AQSH
</address>
```
* Ish nomi uchun iqtibos keltiring
 ```
<p><cite>Qichqiriq</cite>, Edvard Munch. 1893 yilda chizilgan.</p>
```
* Ikki tomonlama bekor qilish (BDO)
```
 <bdo dir="rtl">This text will be written from right to left</bdo> 
```
<kbd>return</kbd>[Mundarijaga qaytish](#homepage)

--------


## HTML MUHAMMOTLARI
Faqat boshida emas, oxirida undov bor
```
<!-- Fikrlaringizni shu yerga yozing -->
```
Foydalanish misoli
```
<!-- Bu izoh -->

<p>Bu paragraf.</p>

<!-- Bu yerga qo'shimcha ma'lumot qo'shishni unutmang -->
```
* Sharhlar HTML kod satrlarini disk raskadrovka qilishga yordam beradi
<kbd>return</kbd>[Mundarijaga qaytish](#homepage)



---------------

## HTML RANGLARI
Siz ularni rang nomlari, RGB, HEX, HSL, RGBA (alfa shaffoflik uchun), HSLA qiymatlari bilan belgilaysiz.
HTML 140 ta standart rang nomlarini qo'llab-quvvatlaydi
* Quyida ko'rsatilgandek fon rangini belgilang:
```
<h1 style="background-color:DodgerBlue;">Hello World</h1>
<p style="background-color:Tomato;">Lorem ipsum...</p> 
```
* Set color of text 
```
<h1 style="color:Tomato;">Hello World</h1>
<p style="color:DodgerBlue;">Lorem ipsum...</p>
<p style="color:MediumSeaGreen;">Ut wisi enim...</p> 
```
* Matn atrofidagi chegara rangini (kvadrat quti) o'rnating
```
<h1 style="border:2px solid Pomidor;">Salom Dunyo</h1>
<h1 style="border:2px solid DodgerBlue;">Salom Dunyo</h1>
<h1 style="border:2px solid Violet;">Salom dunyo</h1>
```
## RGB
* Bularning barchasi bir xil
```
rgb(255, 99, 71)
#ff6347
hsl(9, 100%, 64%)
```
* RGBA, HSLA
```
rgba(255, 99, 71, 0,5)
hsla(9, 100%, 64%, 0,5)
```
```
<h1 style="background-color:rgb(255, 99, 71);">...</h1>
<h1 style="background-color:#ff6347;">...</h1>
<h1 style="background-color:hsl(9, 100%, 64%);">...</h1>

<h1 style="background-color:rgba(255, 99, 71, 0.5);">...</h1>
<h1 style="background-color:hsla(9, 100%, 64%, 0.5);">...</h1>
```
<kbd>qaytish</kbd>[Mundarijaga qaytish](#homepage)
## RGBA
RGB va RGBA rang berish
Qizil, yashil, ko'k va alfa
```rgb(r,g,b)``` har bir parametr 0 dan 255 gacha bo`lgan qiymatga ega, ya'ni jami 256 ta
Ranglarning umumiy soni: 256 x 256 x 256 = 16777216 mumkin bo'lgan ranglar!
```
Qizil rang: rgb(255, 0, 0),
Yashil rang: rgb(0, 255, 0)
Qora: rgb(0, 0, 0)
Oq: rgb (255, 255, 255).
Kulrang: rgb( x,x,x) bu yerda x nol emas yoki 255. Qora va oq rang spektrining ikki uchida joylashgan.
```
RGBA
```rgba(qizil, yashil, ko`k, alfa)``` alfa 0 butunlay shaffof degan ma'noni anglatadi, 1.0 esa umuman shaffof emas.
<kbd>qaytish</kbd>[Mundarijaga qaytish](#homepage)
HTML HEX RANGLARI
RR(QIZIL), GG(GREEN)BB(BLUE)...OLTINTILI BUTUN SALAR HAR BIR 00 dan ff gacha boʻlgan QIYMATLAR BILAN RANGLAR KOMPONENTLARINI AYTARILADI (0-255 kasr bilan bir xil)
```#ff0000```- qizil, chunki qizil rang eng yuqori qiymatga (ff) ega, yashil va ko`k esa 00 va 00 sifatida ko`rinadi.
```#00ff00``` yashil rangda ko`rinadi, chunki yashil rang eng yuqori qiymatga (ff) o`rnatilgan va qolgan ikkitasi nol qiymatga ega
Qora rangni ko'rsatish uchun barcha rang parametrlarini 00 ga o'rnating, masalan: ```#000000```.
Oq rangni ko'rsatish uchun barcha rang parametrlarini ff ga o'rnating: ```#ffffff```
Kulrang soyalar: barcha parametrlar uchun teng qiymatlar:
Ularning har biri turli xil kul ranglardir.
```
#404040
#686868
#a0a0a0
```
<kbd>qaytish</kbd>[Mundarijaga qaytish](#homepage)
## HSL VA HSLA
HSL: rang, to'yinganlik va yorug'lik
HSLA: rang, to'yinganlik, yorug'lik va alfa.
Rang: rang g'ildiragidagi 0 dan 360 0 gacha bo'lgan daraja qizil, 120 yashil, 240 ko'k
To'yinganlik: bu foizli qiymat. 0% qora, 100% esa to'liq rangli
Yengillik: Alsp foiz qiymati: 0% qora va 100% oq
To'yinganlikni rangning intensivligi deb ta'riflash mumkin. Bu rangda qancha kul rang ko'rinishini xohlashingiz haqida.
100% sof rang, kulrang soyalar yo'q
50% 50% kulrang, lekin siz hali ham rangni ko'rishingiz mumkin.
0% butunlay kulrang, endi rangni ko'ra olmaysiz.
** Rangning ochiqligini siz rangga qancha yorug‘lik berishni xohlayotganingizni tasvirlash mumkin, bu erda 0% yorug‘lik yo‘q (qora), 50% 50% yorug‘lik (na qorong‘u, na yorug‘lik) 100% to‘liq ochiqlikni (oq) bildiradi. ).
Kulrang soyalar: Toʻqroq/ochroq soyalarni olish uchun rang va toʻyinganlikni 0 ga oʻrnatish va yorugʻlikni 0 % dan 100 % gacha sozlash orqali olish mumkin:
```
hsl(0, 0%, 20%) --kulrangning quyuqroq soyasi
hsl(0, 0%, 70%)== ochroq kul rang
```
HSLA rang qiymatlari:
Alfa rep shaffofligi. 0,00 to'liq shaffof va 1,0 umuman shaffof emas degan ma'noni anglatadi.
<kbd>qaytish</kbd>[Mundarijaga qaytish](#homepage)


---------



## HTML CSS
HTML STYLES-CSS
CSS bir vaqtning o'zida bir nechta sahifalar tartibini boshqarishi mumkin.
CSS: CAscading uslublar jadvallari: rang, shrift, matn o'lchami, elementlar orasidagi masofa, elementlar qanday joylashishi va joylashtirilishi, qanday fon tasvirlari yoki fon ranglari ishlatilishi, turli qurilmalar va ekran o'lchamlari uchun turli xil displeylar va boshqalarni boshqarish uchun.
Maslahat: Kaskad so'zi asosiy elementga qo'llaniladigan uslub ota-ona ichidagi barcha kichik elementlarga ham qo'llanilishini anglatadi. Shunday qilib, agar siz asosiy matn rangini "ko'k" rangga o'rnatsangiz, barcha sarlavhalar, paragraflar va matn ichidagi boshqa matn elementlari ham bir xil rangga ega bo'ladi (agar siz boshqa narsani belgilamasangiz)!
CSS-ni HTML hujjatlariga 3 usulda qo'shish mumkin:
    Inline - HTML elementlari ichidagi uslub atributidan foydalanish orqali
    Ichki - ```<head>``` bo`limidagi ```<style>``` elementi yordamida
    Tashqi - tashqi CSS fayliga ulanish uchun ```<link>``` elementi yordamida

<kbd>qaytish</kbd>[Mundarijaga qaytish](#homepage)
## CSS INLINE
Inline CSS: bitta HTML elementiga noyob uslubni qo'llash uchun va u bunday elementning uslub atributidan foydalanadi.
* h1 rangini ko'k rangga va p qizil rangga o'rnating
```
<h1 style="color:blue;">Moviy sarlavha</h1>

<p style="color:red;">Qizil paragraf.</p>
```
<kbd>qaytish</kbd>[Mundarijaga qaytish](#homepage)
# CSS ICHKI
Ichki CSS: Bitta HTML sahifasi uchun uslubni aniqlash va u HTML sahifasining <style> elementidagi <head> bo'limida aniqlangan.
```
<!DOCTYPE html>
<html>
<head>
<uslub>
tana (fon rangi: chang ko'k;}
h1 {rang: ko'k;}
p {rang: qizil;}
</style>
</head>
<tana>

<h1>Bu sarlavha</h1>
<p>Bu paragraf.</p>

</body>
</html>
```
<kbd>qaytish</kbd>[Mundarijaga qaytish](#homepage)


--------

## CSS KIRISH


CSS katta muammoni hal qildi:
HTML hech qachon veb-sahifani formatlash uchun teglarni o'z ichiga olmaydi!

HTML veb-sahifa mazmunini tavsiflash uchun yaratilgan, masalan:

```
<h1>Bu sarlavha</h1>

<p>Bu paragraf.</p>
```
  
HTML 3 da kiritilgan HTML elementlariga shrift rangini qo'shish HTML nazarda tutilganidan og'ish edi.

birinchi navbatda qilish.

CSS ko'p ishni tejaydi!

Uslub ta'riflari odatda tashqi .css fayllarida saqlanadi.

Tashqi uslublar jadvali fayli yordamida siz faqat bitta faylni o'zgartirish orqali butun veb-sayt ko'rinishini o'zgartirishingiz mumkin!


<kbd>qaytish</kbd>[Mundarijaga qaytish](#homepage)


---------

## CSS SYNTAX

```
h1 {rang: ko'k; shrift o'lchami: 12px;}

selektor {xususiyat: qiymat; xususiyat: qiymat;}
```
mulk+qiymat=deklaratsiya bloki.

  
```
p {
   rang: qizil;
   matnni tekislash: markaz;
}

```

p qizil rangga o'rnatiladi va avtomatik ravishda markazlashtiriladi.


<kbd>return</kbd>[Mundarijaga qaytish](#homepage)


------



## CSS SELECTORS

Ular ma'lum html elementlarining uslublarini belgilashda yordam beradi

CSS selektorlari toifalari::

Oddiy selektorlar: elementlarni tanlash uchun nom, id va sinfdan foydalaning
Kombinator selektorlari: ularni tanlash uchun elementlar orasidagi munosabatlardan foydalaning
Pseudo-klass selektorlari: elementlarni ma'lum holatga qarab tanlash uchun
Pseudoelement selektorlari: elementning bir qismini tanlash va uslublash
Atribut selektorlari: elementni tanlash uchun atribut yoki atribut qiymatidan foydalaning

Eng asosiy CSS selektorlarini tushuntirish

1. CSS element Selektori: HTML elementlarini tanlash uchun element nomidan foydalanadi

```
p {
   matnni tekislash: markaz;
   rang: qizil;
}

```


2. CSS id Selector: Elementni tanlash uchun uning id atributidan foydalanadi. Element identifikatori veb-sahifa ichida noyobdir

va u bitta noyob elementni tanlashi mumkin.
Elementni tanlashda identifikatordan foydalanish uchun hash(#) dan keyin element identifikatoridan foydalaning. Id nomi boshlanmaydi

raqam bilan.

```
<!DOCTYPE html>
<html>
<head>
<uslub>
#para1 {
   matnni tekislash: markaz;
   rang: qizil;
}
</style>
</head>
<tana>

<p id="para1">Salom dunyo!</p>
<p>Ushbu paragrafga uslub ta'sir qilmaydi.</p>

</body>
</html>

```



CSS klassi selektori: muayyan sinf atributiga ega HTML elementlarini tanlaydi. (.) belgisidan keyin foydalaning

sinf nomi. Quyidagi kod class="center" ni qizil va markazga moslashtiradi

```

<!DOCTYPE html>
<html>
<head>
<uslub>
.markaz {
   matnni tekislash: markaz;
   rang: qizil;
}
</style>
</head>
<tana>

<h1 class="center">Qizil va markazga tekislangan sarlavha</h1>
<p class="center">Qizil va markazga tekislangan paragraf.</p>

</body>
</html>

```


Bundan tashqari, siz faqat sinf uslubiga ta'sir qilishi kerak bo'lgan HTML elementlarini belgilashingiz mumkin. Quyidagi kodda faqat

```class="center"``` bo`lgan ```p``` elementlar qizil rangda bo`ladi va markazga tekislanadi.

```

<!DOCTYPE html>
<html>
<head>
<uslub>
p.markaz {
   matnni tekislash: markaz;
   rang: qizil;
}
</style>
</head>
<tana>

<h1 class="center">Bu sarlavha ta'sir qilmaydi</h1>
<p class="center">Ushbu paragraf qizil rangda va markazga hizalanadi.</p>

</body>
</html>

```

HTML elementlari bir nechta sinflarga murojaat qilishi mumkin. Bunday holda, p element barchaga mos ravishda uslublanadi

sinflar


```
<!DOCTYPE html>
<html>
<head>
<uslub>
p.markaz {
   matnni tekislash: markaz;
   rang: qizil;
}

katta {
   shrift hajmi: 300%;
}
</style>
</head>
<tana>

<h1 class="center">Bu sarlavha ta'sir qilmaydi</h1>
<p class="center">Ushbu paragraf qizil rangda va markazga hizalanadi.</p>
<p class="center large">Ushbu paragraf qizil, markazga tekislangan va katta shrift o'lchamida bo'ladi.</p>

</body>
</html>
```


CSS universal selektori

* sahifadagi barcha HTML elementlarini tanlaydi

```
<!DOCTYPE html>
<html>
<head>
<uslub>
* {
   matnni tekislash: markaz;
   rang: ko'k;
}
</style>
</head>
<tana>

<h1>Salom dunyo!</h1>

<p>Sahifadagi har bir elementga uslub ta'sir qiladi.</p>
<p id="para1">Men ham!</p>
<p>Va men!</p>

</body>
</html>

```


CSS guruhlash selektori::

Bir xil ta'riflarga ega barcha HTML elementlarini tanlaydi.


quyidagi kodga ega bo'lish o'rniga:

```
h1 {
   matnni tekislash: markaz;
   rang: qizil;
}

h2 {
   matnni tekislash: markaz;
   rang: qizil;
}

p {
   matnni tekislash: markaz;
   rang: qizil;
}
```

Bizda oddiygina bo'lishi mumkin:

```

h1, h2, p {
   matnni tekislash: markaz;
   rang: qizil;
}

```
va hali ham bir xil natijaga erishasiz


Barcha CSS selektorlarining qisqacha mazmuni:

Barcha CSS oddiy selektorlari
  
```
Selektor misoli Misol tavsifi

#id #firstname id="firstname"li elementni tanlaydi
.class .intro Class="intro" bilan barcha elementlarni tanlaydi
element.class p.intro Faqat class="intro" bilan <p> elementlarni tanlaydi
* * Barcha elementlarni tanlaydi
element p Barcha <p> elementlarni tanlaydi
element,element,.. div, p Barcha <div> va barcha <p> elementlarni tanlaydi
```



<kbd>qaytish</kbd>[Mundarijaga qaytish](#homepage)

---------


## CSS SELECTORS

Ular ma'lum html elementlarining uslublarini belgilashda yordam beradi

CSS selektorlari toifalari::

Oddiy selektorlar: elementlarni tanlash uchun nom, id va sinfdan foydalaning
Kombinator selektorlari: ularni tanlash uchun elementlar orasidagi munosabatlardan foydalaning
Pseudo-klass selektorlari: elementlarni ma'lum holatga qarab tanlash uchun
Pseudoelement selektorlari: elementning bir qismini tanlash va uslublash
Atribut selektorlari: elementni tanlash uchun atribut yoki atribut qiymatidan foydalaning

Eng asosiy CSS selektorlarini tushuntirish

1. CSS element Selektori: HTML elementlarini tanlash uchun element nomidan foydalanadi

```
p {
   matnni tekislash: markaz;
   rang: qizil;
}

```


2. CSS id Selector: Elementni tanlash uchun uning id atributidan foydalanadi. Element identifikatori veb-sahifa ichida noyobdir

va u bitta noyob elementni tanlashi mumkin.
Elementni tanlashda identifikatordan foydalanish uchun hash(#) dan keyin element identifikatoridan foydalaning. Id nomi boshlanmaydi

raqam bilan.

```
<!DOCTYPE html>
<html>
<head>
<uslub>
#para1 {
   matnni tekislash: markaz;
   rang: qizil;
}
</style>
</head>
<tana>

<p id="para1">Salom dunyo!</p>
<p>Ushbu paragrafga uslub ta'sir qilmaydi.</p>

</body>
</html>

```



CSS klassi selektori: muayyan sinf atributiga ega HTML elementlarini tanlaydi. (.) belgisidan keyin foydalaning

sinf nomi. Quyidagi kod class="center" ni qizil va markazga moslashtiradi

```

<!DOCTYPE html>
<html>
<head>
<uslub>
.markaz {
   matnni tekislash: markaz;
   rang: qizil;
}
</style>
</head>
<tana>

<h1 class="center">Qizil va markazga tekislangan sarlavha</h1>
<p class="center">Qizil va markazga tekislangan paragraf.</p>

</body>
</html>

```


Bundan tashqari, siz faqat sinf uslubiga ta'sir qilishi kerak bo'lgan HTML elementlarini belgilashingiz mumkin. Quyidagi kodda faqat

```class="center"``` bo`lgan ```p``` elementlar qizil rangda bo`ladi va markazga tekislanadi.

```

<!DOCTYPE html>
<html>
<head>
<uslub>
p.markaz {
   matnni tekislash: markaz;
   rang: qizil;
}
</style>
</head>
<tana>

<h1 class="center">Bu sarlavha ta'sir qilmaydi</h1>
<p class="center">Ushbu paragraf qizil rangda va markazga hizalanadi.</p>

</body>
</html>

```

HTML elementlari bir nechta sinflarga murojaat qilishi mumkin. Bunday holda, p element barchaga mos ravishda uslublanadi

sinflar


```
<!DOCTYPE html>
<html>
<head>
<uslub>
p.markaz {
   matnni tekislash: markaz;
   rang: qizil;
}

katta {
   shrift hajmi: 300%;
}
</style>
</head>
<tana>

<h1 class="center">Bu sarlavha ta'sir qilmaydi</h1>
<p class="center">Ushbu paragraf qizil rangda va markazga hizalanadi.</p>
<p class="center large">Ushbu paragraf qizil, markazga tekislangan va katta shrift o'lchamida bo'ladi.</p>

</body>
</html>
```


CSS universal selektori

* sahifadagi barcha HTML elementlarini tanlaydi

```
<!DOCTYPE html>
<html>
<head>
<uslub>
* {
   matnni tekislash: markaz;
   rang: ko'k;
}
</style>
</head>
<tana>

<h1>Salom dunyo!</h1>

<p>Sahifadagi har bir elementga uslub ta'sir qiladi.</p>
<p id="para1">Men ham!</p>
<p>Va men!</p>

</body>
</html>

```


CSS guruhlash selektori::

Bir xil ta'riflarga ega barcha HTML elementlarini tanlaydi.


quyidagi kodga ega bo'lish o'rniga:

```
h1 {
   matnni tekislash: markaz;
   rang: qizil;
}

h2 {
   matnni tekislash: markaz;
   rang: qizil;
}

p {
   matnni tekislash: markaz;
   rang: qizil;
}
```

Bizda oddiygina bo'lishi mumkin:

```

h1, h2, p {
   matnni tekislash: markaz;
   rang: qizil;
}

```
va hali ham bir xil natijaga erishasiz


Barcha CSS selektorlarining qisqacha mazmuni:

Barcha CSS oddiy selektorlari
  
```
Selektor misoli Misol tavsifi

#id #firstname id="firstname"li elementni tanlaydi
.class .intro Class="intro" bilan barcha elementlarni tanlaydi
element.class p.intro Faqat class="intro" bilan <p> elementlarni tanlaydi
* * Barcha elementlarni tanlaydi
element p Barcha <p> elementlarni tanlaydi
element,element,.. div, p Barcha <div> va barcha <p> elementlarni tanlaydi
```



<kbd>qaytish</kbd>[Mundarijaga qaytish](#homepage)


----------

## Xatcho‘plarni bog‘lash
HTML havolalari - xatcho'plar yaratish: foydalanuvchilarga veb-sahifaning ma'lum bir qismiga o'tish imkonini beradi. Bu uzoq veb-sahifa uchun yordam beradi.

* Xatcho‘p yaratish uchun xatcho‘p yarating va unga havola qo‘shing. Sahifani bosish avtomatik ravishda veb-sahifadagi xatcho'plangan joyga yo'naltiriladi

- Xatcho'p yaratish uchun id atributidan foydalaning:
```
<h2 id="C4">4-bob</h2>
```
- Xatcho'pga o'sha sahifadan havola qo'shing.
```
  <a href="#C4">4-bobga o‘tish</a>
```
-Boshqa sahifadagi xatcho'pga havola qo'shing:
```
<a href="html_demo.html#C4">4-bobga o‘tish</a>
```
**Havoladan pastki chiziqni olib tashlash uchun matn bezaklarini olib tashlang:
```
<a href="html_images.asp" style="text-decoration:none">HTML rasmlar</a>
```
Bo'lim xulosasi:

Bo'lim xulosasi

Sahifadagi xatcho‘plarni aniqlash uchun id atributidan (```id="qiymat"```) foydalaning
Xatcho‘pga havola qilish uchun href atributidan (```href="#value"```) foydalaning

<kbd>qaytish</kbd>[Mundarijaga qaytish](#homepage)