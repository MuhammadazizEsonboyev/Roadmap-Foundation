## HTML TASVIRLAR

## TASVIR

```<img src="pic_trulli.jpg" alt="Italian Trulli">```

Rasm tegi veb-sahifaga rasmlarni kiritish uchun ishlatiladi. Rasmlar o'rnatilmagan veb-sahifaga bog'langan.

SRC atributlari
src - tasvirga yo'lni belgilaydi
alt - tasvir uchun muqobil matnni belgilaydi

Sintaksis
```<img src="url" alt="alternatetext">```

Brauzerlar veb-serverdan rasm oladi va har safar yuklanganda sahifaga kiritadi. Rasm veb-sahifaga nisbatan bir xil joyda qoladi... aks holda havola buzilganligini bildirish uchun pastki matn paydo bo'ladi.

**Alt atributining qiymati quyidagi hollarda ko‘rsatiladi: sekin ulanish tufayli, src atributidagi xatolik yoki foydalanuvchi html kodni o‘qiydigan va foydalanuvchi uchun o‘qib chiqadigan ekranni o‘qish moslamasidan foydalansa...odatda ko‘zi ojizlar tomonidan foydalaniladi. odamlar.

**Shuningdek, siz tasvirning uslub atributida kenglik va balandlikni belgilashingiz mumkin

  ```<img src="img_girl.jpg" alt="Kumtkadagi qiz" style="width:500px;height:600px;">```

**Wi and height atributi kenglik va balandlik atributi sifatida... bu har doim pikselda
  ```<img src="img_girl.jpg" alt="Kumtkadagi qiz" eni="500" balandligi="600">```

**Uslublar jadvali tasvir hajmini o'zgartirmasligi uchun uslub atributidan foydalangan ma'qul.

```
<!DOCTYPE html>
<html>
<head>
<uslub>
img {
   kengligi: 100%;
}
</style>
</head>
<tana>

<img src="html5.gif" alt="HTML5 belgisi" kengligi="128" balandligi="128">

<img src="html5.gif" alt="HTML5 belgisi" style="width:128px;height:128px;">

</body>
</html>
```

**Ichki jilddagi tasvirlar uchun siz jild nomini kiritishingiz kerak

```<img src="/images/html5.gif" alt="HTML5 Icon" style="width:128px;height:128px;">```

Agar saytingiz boshqa serverdagi tashqi rasmga ishora qilsa, tasvirga ishora qilish uchun toʻliq URL manzilini koʻrsating.

  ```mg src="https://www.w3schools.com/images/w3schools_green.jpg" alt="W3Schools.com">```

Tashqi tasvirlarga eslatma: istalgan vaqtda sayt egasi tomonidan olib tashlanishi mumkin. Shuningdek, mualliflik huquqi buzilishining oldini olish uchun ruxsat olish kerak bo'lishi mumkin

**Animatsiyalangan rasmlar:: HTML GIF-larga ruxsat beradi

```<img src="programming.gif" alt="Kompyuter odami" style="width:48px;height:48px;">```

**Tasvirni teg sifatida:: <a> tegi ichiga <img> tegini qo'ying

```
<a href="default.asp">
   <img src="smiley.gif" alt="HTML qo'llanmasi" style="width:42px;height:42px;">
</a>
```
**CSS float xususiyatidan foydalangan holda tasvirni matnning o‘ng yoki chap tomonida suzishga ruxsat bering
```
<p><img src="smiley.gif" alt="Tabassumli yuz" style="float:right;width:42px;height:42px;">
Tasvir matnning o‘ng tomonida suzib yuradi.</p>

<p><img src="smiley.gif" alt="Tabassumli yuz" style="float:left;width:42px;height:42px;">
Rasm matnning chap tomonida suzib yuradi.</p>
```
** Veb-saytda qo'llab-quvvatlanadigan umumiy rasm formatlari

qisqartma Fayl formati fayl kengaytmasi
APNG animatsion portativ tarmoq grafikasi .apng
GIF grafik almashish formati .gif
ICO Microsoft Icon .ico, .cur
JPEG Joint Photographic Expert Group rasmi .jpg, .jpeg, .jfif, .pjpeg, .pjp
PNG Portativ tarmoq grafikasi .png
SVG Scalable vektor grafikasi .svg


**Katta rasmlarni yuklash vaqt talab etadi va veb-sahifangizni sekinlashtirishi mumkin...shuning uchun rasmlardan ehtiyotkorlik bilan foydalaning.

<kbd>qaytish</kbd>[Mundarijaga qaytish](#homepage)


------- 



## HTML TASVIRLAR

## TASVIR

```<img src="pic_trulli.jpg" alt="Italian Trulli">```

Rasm tegi veb-sahifaga rasmlarni kiritish uchun ishlatiladi. Rasmlar o'rnatilmagan veb-sahifaga bog'langan.

SRC atributlari
src - tasvirga yo'lni belgilaydi
alt - tasvir uchun muqobil matnni belgilaydi

Sintaksis
```<img src="url" alt="alternatetext">```

Brauzerlar veb-serverdan rasm oladi va har safar yuklanganda sahifaga kiritadi. Rasm veb-sahifaga nisbatan bir xil joyda qoladi... aks holda havola buzilganligini bildirish uchun pastki matn paydo bo'ladi.

**Alt atributining qiymati quyidagi hollarda ko‘rsatiladi: sekin ulanish tufayli, src atributidagi xatolik yoki foydalanuvchi html kodni o‘qiydigan va foydalanuvchi uchun o‘qib chiqadigan ekranni o‘qish moslamasidan foydalansa...odatda ko‘zi ojizlar tomonidan foydalaniladi. odamlar.

**Shuningdek, siz tasvirning uslub atributida kenglik va balandlikni belgilashingiz mumkin

  ```<img src="img_girl.jpg" alt="Kumtkadagi qiz" style="width:500px;height:600px;">```

**Wi and height atributi kenglik va balandlik atributi sifatida... bu har doim pikselda
  ```<img src="img_girl.jpg" alt="Kumtkadagi qiz" eni="500" balandligi="600">```

**Uslublar jadvali tasvir hajmini o'zgartirmasligi uchun uslub atributidan foydalangan ma'qul.

```
<!DOCTYPE html>
<html>
<head>
<uslub>
img {
   kengligi: 100%;
}
</style>
</head>
<tana>

<img src="html5.gif" alt="HTML5 belgisi" kengligi="128" balandligi="128">

<img src="html5.gif" alt="HTML5 belgisi" style="width:128px;height:128px;">

</body>
</html>
```

**Ichki jilddagi tasvirlar uchun siz jild nomini kiritishingiz kerak

```<img src="/images/html5.gif" alt="HTML5 Icon" style="width:128px;height:128px;">```

Agar saytingiz boshqa serverdagi tashqi rasmga ishora qilsa, tasvirga ishora qilish uchun toʻliq URL manzilini koʻrsating.

  ```mg src="https://www.w3schools.com/images/w3schools_green.jpg" alt="W3Schools.com">```

Tashqi tasvirlarga eslatma: istalgan vaqtda sayt egasi tomonidan olib tashlanishi mumkin. Shuningdek, mualliflik huquqi buzilishining oldini olish uchun ruxsat olish kerak bo'lishi mumkin

**Animatsiyalangan rasmlar:: HTML GIF-larga ruxsat beradi

```<img src="programming.gif" alt="Kompyuter odami" style="width:48px;height:48px;">```

**Tasvirni teg sifatida:: <a> tegi ichiga <img> tegini qo'ying

```
<a href="default.asp">
   <img src="smiley.gif" alt="HTML qo'llanmasi" style="width:42px;height:42px;">
</a>
```
**CSS float xususiyatidan foydalangan holda tasvirni matnning o‘ng yoki chap tomonida suzishga ruxsat bering
```
<p><img src="smiley.gif" alt="Tabassumli yuz" style="float:right;width:42px;height:42px;">
Tasvir matnning o‘ng tomonida suzib yuradi.</p>

<p><img src="smiley.gif" alt="Tabassumli yuz" style="float:left;width:42px;height:42px;">
Rasm matnning chap tomonida suzib yuradi.</p>
```
** Veb-saytda qo'llab-quvvatlanadigan umumiy rasm formatlari

qisqartma Fayl formati fayl kengaytmasi
APNG animatsion portativ tarmoq grafikasi .apng
GIF grafik almashish formati .gif
ICO Microsoft Icon .ico, .cur
JPEG Joint Photographic Expert Group rasmi .jpg, .jpeg, .jfif, .pjpeg, .pjp
PNG Portativ tarmoq grafikasi .png
SVG Scalable vektor grafikasi .svg


**Katta rasmlarni yuklash vaqt talab etadi va veb-sahifangizni sekinlashtirishi mumkin...shuning uchun rasmlardan ehtiyotkorlik bilan foydalaning.

<kbd>qaytish</kbd>[Mundarijaga qaytish](#homepage)

## TASVIR XARITA
Image Maps::Rasmning qayerini bosganingizga qarab amallarni bajarish imkonini beradi. Sizga rasm, bosiladigan maydonni tavsiflovchi html kod kerak.

Rasm: Tasvir yorlig'i yordamida kiritilgan, ammo bu holda usemap atributini qo'shishingiz kerak.

```
<img src="workplace.jpg" alt="Ish joyi" usemap="#ishchimap">
```

-Usermap qiymati # xesh-tegidan boshlanadi, undan keyin rasm xaritasi nomi keladi va rasm va tasvir xaritasi o'rtasida aloqa yaratish uchun ishlatiladi.

Tasvir xaritasi sifatida istalgan tasvirdan foydalanishingiz mumkin.

-name atributidan foydalangan holda rasmga bog'langan ```<map>``` elementni qo`shing.

```
<map name="ishchi xaritasi">
```
name atributi <img> ning usemap atributi bilan bir xil qiymatga ega bo'lishi kerak

-Rasmga bosiladigan maydon qo'shish: Siz bosiladigan maydonni <maydon> elementi yordamida belgilaysiz.
* Quyidagi qiymatlardan birini ishlatib bosiladigan maydon shaklini aniqlang:
  rect - to'rtburchaklar hududni belgilaydi
  aylana - dumaloq hududni belgilaydi
  poly - ko'pburchak mintaqani belgilaydi
  standart - butun mintaqani belgilaydi

- Rasmga bosiladigan maydonni joylashtirish uchun koordinatani aniqlang.

```
Shakl = "to'g'ri"
```
```shape="rect"``` uchun koordinatalar juft bo`lib, biri x o`qi (chapdan masofa) va biri y o`qi (yuqoridan masofa) uchundir.

Shunday qilib, 34,44 koordinatalari chap chetidan 34 piksel va yuqoridan 44 piksel masofada joylashgan:

270,350 koordinatalari chap chetidan 270 piksel va yuqoridan 350 piksel masofada joylashgan:


``` Shakl="doira"```

Doira maydonini qo'shish uchun avval doira markazining koordinatalarini toping:

337,300

keyin radiusni belgilang: 44 piksel

**
```
<area shape="circle" coords="337, 300, 44" href="coffee.htm">
```
```Shape=poli"```

```shape="poly"``` bir nechta koordinata nuqtalarini o`z ichiga oladi, ular to`g`ri chiziqlar (ko`pburchak) bilan hosil qilingan shaklni yaratadi.

Bu har qanday shaklni yaratish uchun ishlatilishi mumkin. Kruvasan kabi. Kruvasanning barcha qirralari uchun x va y koordinatalarini topishingiz kerak.

* Har bir nuqtada x va y ... ko'pburchak shaklning perimetri atrofidagi barcha koordinatalarni belgilang.

  ```
  <area shape="poly" coords="140,121,181,116,204,160,204,222,191,270,140,329,85,355,58,352,37,322,40,259,103,161,103,161,103,16141," href="m)
  ```
**Poissant shaklini bosish orqali JS funksiyasini ham ishga tushirishingiz mumkin.
JavaScript funksiyasini bajarish uchun <area> elementiga bosish hodisasini qo'shing:

```
  <map name="ishchi xaritasi">
   <area shape="circle" coords="337,300,44" onclick="myFunction()">
</map>

<skript>
funktsiya myFunction() {
   alert("Siz kofe stakanini bosdingiz!");
}
</script>
```
Rasmdagi giperhavolaga amal qilishdan oldin foydalanuvchi nima qilmoqchi bo'lganligini tasdiqlash uchun foydalanuvchini xabardor qilish uchun href funktsiyasidan foydalanishingiz mumkin.

**Rasm xaritasi xulosasi: =

```
<img> Tasvirni belgilaydi
<map> Rasm xaritasini belgilaydi
<maydon> Rasm xaritasi ichidagi bosiladigan maydonni belgilaydi
<rasm> Bir nechta rasm resurslari uchun konteynerni belgilaydi
```
<kbd>qaytish</kbd>[Mundarijaga qaytish](#homepage)

## Fon rasmlari

Fon rasmlari: Agar u kichikroq bo'lsa, o'zini takrorlaydi

*Stil atributi va CSS fon tasviridan foydalangan holda HTML elementiga fon rasmini qo'shing.
```
  <div style="background-image: url('img_girl.jpg');">
```

**Shuningdek, siz fon tasvirini bosh qismining uslub elementida ham belgilashingiz mumkin
```
  <uslub>
div {
   fon rasmi: url('img_girl.jpg');
}
</style>
```

**To‘liq sahifa uchun fon rasmini qo‘shish: tana elementida fon tasvirini belgilang
```
<uslub>
tana {
   fon rasmi: url('img_girl.jpg');
}
</style>
```

**Fon tasvirini takrorlash:: Elementdan kichikroq fon tasviri element oxiriga yetguncha gorizontal va vertikal ravishda takrorlanadi.

```
<uslub>
tana {
   fon rasmi: url('img_girl.jpg');
}
</style>

**Fon tasvirini takrorlashning oldini olish uchun siz fonni takrorlash xususiyatini takrorlanmaydigan qilib sozlashingiz mumkin.

  <uslub>
tana {
   fon rasmi: url('misol_img_girl.jpg');
   fon-takrorlash: takrorlanmaslik;
}
</style>
```

* Fon qopqog'i: butun elementni qoplash uchun fon tasvirini yaratish uchun qoplash uchun fon o'lchami xususiyatini o'rnatishingiz mumkin. Butun element har doim qoplanishiga ishonch hosil qilish uchun background-attachment xususiyatini fixed ga sozlang... Bu tasvirning asl nisbatlarini saqlaydi.

```
<uslub>
tana {
   fon rasmi: url('img_girl.jpg');
   fon-takrorlash: takrorlanmaslik;
   fon-ilova: belgilangan;
   fon o'lchami: qopqoq;
```
** Fon cho‘zilishi:: Fon tasvirini butun elementga mos keladigan qilib cho‘zish imkonini beradi. Fon o'lchami xususiyatini 100% 100% ga o'rnating

```
  <uslub>
tana {
   fon rasmi: url('img_girl.jpg');
   fon-takrorlash: takrorlanmaslik;
   fon-ilova: belgilangan;
   fon o'lchami: 100% 100%;
}
</style>
```

<kbd>qaytish</kbd>[Mundarijaga qaytish](#homepage)

------


## CSS CSS QANDAY QO'SHISH MUMKIN

Brauzer uslublar jadvalidagi yoki <style>dagi ma'lumotlardan foydalangan holda html-ni formatlaydi


Tashqi CSS::

Bu butun veb-sayt uslubini o'zgartirish uchun foydalanishingiz mumkin bo'lgan fayl. Keyin veb-saytning har bir sahifasi

boshqaruvchi tashqi uslublar varag'iga havolani o'z ichiga olgan <head> bo'limiga <link> ni qo'shing

butun hujjatning uslubi. Siz har qanday matn muharriri yordamida tashqi fayl yaratishingiz mumkin. Bu fayl bo'lishi kerak

.css kengaytmasi bilan saqlangan va faylda HTML teglari bo'lmasligi kerak.


"mystyle.css" kodini o'z ichiga olganida:

```
tana {
   fon rangi: ochiq ko'k;
}

h1 {
   rang: ko'k;
   chap chekka: 20px;
}
  
```


Mystyle quyida meros qilib olinishi mumkin:
  
```
<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" href="mystyle.css">
</head>
<tana>

<h1>Bu sarlavha</h1>
<p>Bu paragraf.</p>

</body>
</html>
```

Eslatma: Mulk qiymati va uning birligi o'rtasida bo'sh joy yo'q. Ya'ni foydalaning: 20 piksel emas, balki 20 piksel


Ichki CSS::

Bitta HTML sahifasi o'ziga xos uslubga ega bo'lsa foydalanish mumkin. Siz ```<style>``` element ichida, ichida belgilashingiz kerak

```<head>``` bo`limi. Ichki CSS misoli quyida ko'rsatilgan:

```
!DOCTYPE html>
<html>
<head>
<uslub>
tana {
   fon rangi: zig'ir;
}

h1 {
   rang: to'q qizil;
   chap chekka: 40px;
}
</style>
</head>
<tana>

<h1>Bu sarlavha</h1>
<p>Bu paragraf.</p>

</body>
</html>
```


Inline CSS::

Siz faqat bitta elementga noyob uslubni qo'llash uchun inline uslubdan foydalanishingiz mumkin. Inline uslublaridan foydalanish uchun qo'shing

mos elementga uslub atributi. Style atributi har qanday CSS xususiyatlarini o'z ichiga olishi mumkin.

```
<!DOCTYPE html>
<html>
<tana>

<h1 style="color:blue;text-align:center;">Bu sarlavha</h1>
<p style="color:red;">Bu paragraf.</p>

</body>
</html>
```

Eslatma: Inline uslub sizga uslublar jadvalining afzalliklarini rad etadi, chunki siz endi uslubni tahrirlashingiz kerak.

elementlar alohida. Faqat kerak bo'lganda CSS inline foydalaning



Bir nechta uslublar jadvallari::

Turli xil uslublar jadvalida bir xil element uchun uslublar mavjud bo'lsa, elementlar uchun oxirgi o'qilgan varaq uslubi

elementga qo'llaniladi.


mystyle.css faylida:

```
h1 {
   rang: ko'k;
}

va ichki uslublar jadvali quyidagilarni o'z ichiga oladi:


h1 {
   rang: to'q sariq;
}
```

A holi: tashqi uslublar jadvaliga havoladan keyin belgilangan ichki uslub,```<h1>``` elementlar to'q sariq rangga ega bo'ladi

rang, chunki ichki uslub oxirgi keladi

```
<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" type="text/css" href="mystyle.css">
<uslub>
h1 {
   rang: to'q sariq;
}
</style>
</head>
<tana>

<h1>Bu sarlavha</h1>
<p>Ushbu hujjatning uslubi tashqi uslublar jadvali va ichki uslubning kombinatsiyasidan iborat</p>

</body>
</html>
```

B holi: Agar ichki uslub tashqi uslublar jadvali havolasidan oldin aniqlangan bo'lsa, u holda ```<h1>``` elementlari

uslublar jadvalida belgilangan ko'k rangni oladi.

```
<!DOCTYPE html>
<html>
<head>
<uslub>
h1 {
   rang: to'q sariq;
}
</style>
<link rel="stylesheet" type="text/css" href="mystyle.css">
</head>
<tana>

<h1>Bu sarlavha</h1>
<p>Ushbu hujjatning uslubi tashqi uslublar jadvali va ichki uslubning kombinatsiyasidan iborat</p>

</body>
</html>
```


Kaskad tartibi::

Agar HTML elementida bir nechta uslublar belgilangan bo'lsa, barcha uslublar yangi virtualga "kaskad" qiladi

quyidagi qoidalarga muvofiq uslublar jadvali 1. eng yuqori ustuvorlikka ega va 3. eng kam.


1. Inline uslub (HTML elementi ichida)
2. Tashqi va ichki uslublar jadvallari (bosh qismida)
3. Brauzer standarti

Inline uslub eng ustuvor hisoblanadi va tashqi uslublar va brauzer standartlarini bekor qilishi mumkin.

<kbd>qaytish</kbd>[Mundarijaga qaytish](#homepage)
  
-------

## CSS SHOXLARI

  

Ular brauzerda ko'rsatilmaydi, lekin kodni o'qishni yaxshilaydi:


Ular keyinchalik manba kodini tahrirlashda yordam berishi mumkin. Izoh <style> elementi ichiga joylashtiriladi, bilan boshlanadi

```/* va */``` bilan tugaydi va o`zingizga yoqqan kodning istalgan joyida sharh qoldirishingiz mumkin.

```
  /* Bu bir qatorli izoh */
p {
   rang: qizil;
}


/* Bu
ko'p qatorli
izoh */


p {
   rang: qizil;
}
```

HTML va CSS sharhlari

HTML izohi: ```<!--bu sharh--!>```. Element uchun HTML uslubini CSS bilan birlashtirishingiz mumkin:

```
<!DOCTYPE html>
<html>
<head>
<uslub>
p {
   rang: qizil; /* Matn rangini qizil rangga o'rnating */
}
</style>
</head>
<tana>

<h2>Mening sarlavham</h2>

<!-- Bu paragraflar qizil bo'ladi -->
<p>Salom dunyo!</p>
<p>Ushbu paragraf CSS uslubida yaratilgan.</p>
<p>HTML va CSS sharhlari chiqishda ko'rsatilmaydi.</p>

</body>
</html>
```
<kbd>qaytish</kbd>[Mundarijaga qaytish](#homepage)


--------


## CSS RANGLARI


Ranglar::

Siz rangni oldindan belgilangan rang nomlari bilan belgilashingiz mumkin: RGB, HEX, HSL, RGBA, HSLA.


CSS Rang nomlari: 140 ta qo'llab-quvvatlanadigan standart rang nomlari mavjud. Toʻliq roʻyxat uchun quyidagi havolaga qarang.



CSS fon rangi: fon rangini quyida ko'rsatilganidek o'rnating
  
```
<h1 style="background-color:DodgerBlue;">Salom dunyo</h1>

<p style="background-color:Pomidor;">
```

CSS matn rangi: Matn rangini quyida ko'rsatilganidek o'rnatishingiz mumkin:

```
<h1 style="color:Tomato;">Salom dunyo</h1>
<p style="color:DodgerBlue;">Lorem ipsum...</p>
<p style="color:MediumSeaGreen;">Bu juda yaxshi...</p>
```

CSS chegara rangi: Foydalanish chegara rangini (matn atrofidagi quti) o'zgartirish uchun undan foydalanishi mumkin. The

```
<tana>

<h1 style="border: 2px solid Pomidor;">Salom dunyo</h1>

<h1 style="border: 2px solid DodgerBlue;">Salom dunyo</h1>

<h1 style="border: 2px solid Violet;">Salom dunyo</h1>

</body>
```

CSS rang qiymatlari

Rangni RGB qiymatlari, HEX qiymatlari, HSL qiymatlari va RGBA qiymatlari va HSLA qiymatlari yordamida belgilashingiz mumkin.



Quyidagi uchtasi hali ham pomidor ranglari

```
rgb(255, 99, 71)
#ff6347
hsl(9, 100%, 64%)
```



Quyida 50% shaffoflikdagi pomidor mavjud:

```
rgba(255, 99, 71, 0,5)
hsla(9, 100%, 64%, 0,5)
```

Quyidagi ilovaga qarang:
```
<!DOCTYPE html>
<html>
<tana>

<p>Rang nomi "Pomidor" bilan bir xil:</p>

<h1 style="background-color:rgb(255, 99, 71);">rgb(255, 99, 71)</h1>
<h1 style="background-color:#ff6347;">#ff6347</h1>
<h1 style="background-color:hsl(9, 100%, 64%);">hsl(9, 100%, 64%)</h1>

<p>Rang nomi "Pomidor" bilan bir xil, lekin 50% shaffof:</p>
<h1 style="background-color:rgba(255, 99, 71, 0.5);">rgba(255, 99, 71, 0.5)</h1>
<h1 style="background-color:hsla(9, 100%, 64%, 0.5);">hsla(9, 100%, 64%, 0.5)</h1>

<p>Oldindan belgilangan rang nomlariga qo'shimcha ravishda ranglarni RGB, HEX, HSL yoki hatto belgilash mumkin

RGBA yoki HSLA rang qiymatlaridan foydalangan holda shaffof ranglar.</p>

</body>
</html>
```



CSS RGB::

RGB qiymati: RGB vakili qizil, yashil va ko'k yorug'lik manbalari

```
format: rgb (qizil_qiymat, yashil_qiymat, ko'k_qiymat)

```
Rang qiymatlarining har biri 0 dan 255 gacha

```red= rgb(255,0,0);``` chunki qizil rang maksimal, ko`k va yashil esa yo`q.


```qora=rgb(0,0,0);``` chunki yorug`lik yo`q

```white=rgb(255,255,255);``` chunki barcha chiroqlar ko`p... rang ko`rsatilmaydi

```grey=rgb(x,x,x);``` teng rang qiymatlari kul rang hosil qiladi. Shunday qilib, sizda ```rgb(0,0,0)``` qora rang va ```rgb(255,255,255)``` da oq rang bor. 0 va 255 orasidagi har bir teng aralash kulrang, lekin har xil darajada. Qanchalik yaqin bo'lsa, shunchalik teng

qiymatlar nolga teng, kul rang qanchalik quyuqroq bo'lsa.

  
RGBA qiymati: U ranglarning har biri uchun alfa-kanalni (shaffoflik o'lchovi) o'z ichiga oladi.

format: rgba (qizil_qiymat, yashil_qiymat, ko'k_qiymat, alfa)

To'liq shaffof: alfa=0,0
Hech qanday shaffof emas: alfa=1,0



CSS HEX RANGLARI::

o‘n oltilik rang formati: #RRGGBB (RR=QIZIL, GG=YASIL, BB=KO‘K)

O'n oltilik butun sonlar rangning komponentini belgilaydi.


HEX qiymati 0 dan ff gacha, xuddi o'nlik 0 dan 255 gacha


#ff0000=qizil, chunki qizil rang maksimal, yashil va ko'k esa nolga o'rnatiladi.

#000000: qora, chunki rangli yorug'lik yo'q

#ffffff: oq, chunki barcha holatlarda maksimal rang yorug'lik mavjud.

000000 va ffffff orasidagi har qanday teng qiymatlar kulrang rang beradi

#787878=kulrang


3 raqamli HEX qiymati: Bu 6 xonali olti raqamli kodlarning qisqa shaklidir
3 xonali hex kod formati: #rgb

Qizil, yashil va ko‘k komponent qiymatlari bir xil bo‘lgandagina siz 3 raqamli hex kodidan foydalanishingiz mumkin

misol:

tana {
   fon rangi: #fc9; /* #ffcc99 bilan bir xil */
}

h1 {
   rang: #f0f; /* #ff00ff bilan bir xil */
}

p {
   rang: #b58; /* #bb5588 bilan bir xil */
}




CSS HSL ranglari::

HSL = Hue, Saturation, Lightness


format: hsl (rang, to'yinganlik, yorug'lik)


Rang = 0 dan 360 gacha bo'lgan rang g'ildiragidagi daraja ( Hue = 0 (Qizil), Hue = 120 (Yashil), Hue = 240 (Moviy))

Toʻyinganlik: kul rangdan (0%) toʻliq ranggacha (100%) foiz qiymati

Yorug'lik: Qoradan (0%) oq ranggacha (100%), oq yoki qora emas (50%) foiz qiymati



To'yinganlik::: Rangning intensivligi. Sof rang+kulrang soyalarsiz=100%, Kulrang+koʻrinmas rang=50%, Toʻliq

kulrang = 0% va siz endi rangni ko'ra olmaysiz


Yengillik: rang berishni qanchalik yorug'lik bilan ta'riflash mumkin. Yorug'lik yo'q (qora) = 0%, yorug'lik ham yo'q

na qorong'i = 50%, to'liq ochiqlik (oq) = 100%


Kulrang soyalar rang va to'yinganlikni nolga o'rnatishni va keyin yorug'likni 0% dan 100% gacha sozlashni o'z ichiga oladi.

quyuqroq / engilroq soyalarni oling.

hsl(0%,0%,0%)=qora

hsl(0%,0%,100%)=oq
hsl(0%,0%,47%)=kulrang


HsLA Value::: Ular alfa kanalini o'z ichiga olgan HSL rang qiymatlarining kengaytmasi

hsla(rang, toʻyinganlik, yengillik, alfa)


<kbd>qaytish</kbd>[Mundarijaga qaytish](#homepage)


---------


## CSS qutisi modeli

Barcha html elementlarini qutilar deb hisoblash mumkin. Quti modeli har bir HTML elementini o'rab oladi va undan iborat

hoshiyalar, hoshiyalar, toʻldirish va haqiqiy tarkib (element tashqarisidan ichkariga oʻtganingizda)

element.



Turli qismlarni tushuntirish:

     Kontent - matn va tasvirlar paydo bo'ladigan qutining mazmuni
     To'ldirish - kontent atrofidagi maydonni tozalaydi. Qoplama shaffof
     Chegara - to'ldirish va tarkibni aylanib o'tadigan chegara
     Chegara - chegaradan tashqaridagi maydonni tozalaydi. Chegara shaffof

Masalan,

<!DOCTYPE html>
<html>
<head>
<uslub>
div {
   fon rangi: och kulrang;
   kengligi: 300px;
   chegara: 15px qattiq yashil;
   to'ldirish: 50px;
   chegara: 20px;
}
</style>
</head>
<tana>

<h2>Boks modelini namoyish qilish</h2>

<p>CSS qutisi modeli aslida har bir HTML elementini oʻrab oladigan qutidir. U quyidagilardan iborat: chegaralar,

toʻldirish, chetlari va haqiqiy kontent.</p>

<div>Ushbu matn qutining mazmunidir. Biz 50px toʻldirish, 20px chekka va 15px yashil chegara qoʻshdik.

Ut enim ad minim veniam, quis nostrud exercitation ullamco workis nisi ut aliquip ex ea commodo consequat.

Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.

Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est

laborum.</div>

</body>
</html>


Elementning kengligi va balandligi

Quti modeli haqidagi bilim veb-sayt elementlarining kengligi va balandligini alda to'g'ri o'rnatish imkonini beradi

brauzerlar.


Muhim: CSS yordamida elementning kengligi va balandligi xususiyatlarini o'rnatganingizda, siz shunchaki kenglik va

tarkib maydonining balandligi. Elementning to'liq hajmini hisoblash uchun siz to'ldirish, chegaralar va qo'shishingiz kerak

chegaralar.


Quyidagi skriptda,

<!DOCTYPE html>
<html>
<head>
<uslub>
div {
   kengligi: 320px;
   to'ldirish: 10px;
   chegara: 5px qattiq kulrang;
   chegara: 0;
}
</style>
</head>
<tana>

<h2>Umumiy kenglikni hisoblang:</h2>

<img src="klematis4_big.jpg" width="350" height="263" alt="Klematis">
<div>Yuqoridagi rasmning kengligi 350px. Ushbu elementning umumiy kengligi ham 350px ni tashkil qiladi.</div>

</body>
</html>

Umumiy kenglik quyida ko'rsatilgandek hisoblanishi mumkin,


320px (kenglik)
+ 20px (chap + o'ng to'ldirish)
+ 10px (chap + o'ng chegara)
+ 0px (chap + o'ng chekka)
= 350px


Elementning umumiy kengligi quyidagicha hisoblanishi kerak:

Elementning umumiy kengligi = kenglik + chap to'ldirish + o'ng to'ldirish + chap chegara + o'ng chegara + chap chet +

o'ng chekka

Xuddi shunday, elementning umumiy balandligi quyida ko'rsatilgandek hisoblanishi kerak:

Elementning umumiy balandligi = balandlik + yuqori to'ldirish + pastki to'ldirish + yuqori chegara + pastki chegara + yuqori chet +

pastki chegara

<kbd>qaytish</kbd>[Mundarijaga qaytish](#homepage)


---------



## CSS konturi


Reja::

Kontur - bu elementni "ajratib turishi" uchun elementlar (tashqi chegaralar) atrofida chizilgan chiziq.

Quyida ko'rsatilgan skript yordamida element atrofida kontur yaratilishi mumkin:

<!DOCTYPE html>
<html>
<head>
<uslub>
p {
   chegara: 2px qattiq qora;
   kontur: #4CAF50 qattiq 2px;
   chegara: avtomatik;
   to'ldirish: 20px;
   matnni tekislash: markaz;
}
</style>
</head>
<tana>

<h2>CSS konturi</h2>
<p>Bu elementda 2px qora hoshiya va kengligi 10px yashil kontur mavjud.</p>

</body>
</html>



CSS-ning asosiy xususiyatlari quyidagilarni o'z ichiga oladi:

     kontur uslubi
     kontur-rang
     kontur kengligi
     kontur-ofset
     kontur


Eslatma: Kontur chegaralardan farq qiladi! Chegaradan farqli o'laroq, kontur element chegarasidan tashqarida chiziladi va

boshqa kontent bilan bir-biriga mos kelishi mumkin. Bundan tashqari, kontur element o'lchamlarining bir qismi EMAS; elementning umumiy miqdori

kenglik va balandlik konturning kengligidan ta'sirlanmaydi.


CSS kontur uslubi

Outline-style xususiyati kontur uslubini belgilaydi va quyidagi qiymatlardan biriga ega bo'lishi mumkin:

     nuqtali - nuqtali konturni belgilaydi
     chiziqli - chiziqli konturni belgilaydi
     qattiq - qattiq konturni belgilaydi
     double - juft konturni belgilaydi
     groove - 3D yivli konturni belgilaydi
     ridge - 3D qirrali konturni belgilaydi
     inset - 3D inset konturini belgilaydi
     outset - 3D boshlang'ich konturini belgilaydi
     none - hech qanday konturni belgilamaydi
     yashirin - Yashirin konturni belgilaydi


Yuqoridagi sxemalarni amalga oshirish quyida ko'rsatilgan:


<!DOCTYPE html>
<html>
<head>
<uslub>
p {kontur-rang: qizil;}

p.dotted {kontur uslubi: nuqta;}
p.dashed {kontur uslubi: chiziqcha;}
p.solid {kontur uslubi: qattiq;}
p.double {kontur uslubi: double;}
p.groove {kontur uslubi: groove;}
p.ridge {kontur uslubi: tizma;}
p.inset {kontur uslubi: inset;}
p.outset {kontur uslubi: boshlang'ich;}
</style>
</head>
<tana>

<h2>Kontur tarzidagi xususiyat</h2>

<p class="dotted">Nuqtali kontur</p>
<p class="dashed">Chiziq kontur</p>
<p class="solid">Yaxshi kontur</p>
<p class="double">Qo'shaloq kontur</p>
<p class="groove">Yuz konturi. Effekt kontur-rang qiymatiga bog'liq.</p>
<p class="ridge">Tiz konturi. Effekt kontur-rang qiymatiga bog'liq.</p>
<p class="inset">Kiritilgan kontur. Effekt kontur-rang qiymatiga bog'liq.</p>
<p class="outset">Boshlang'ich kontur. Effekt kontur-rang qiymatiga bog'liq.</p>

</body>
</html>


Eslatma: Eslatma: Boshqa kontur xususiyatlarining hech biri (keyingi boblarda ko'proq bilib olasiz)

Agar kontur uslubi xususiyati o'rnatilmagan bo'lsa, HAR QANDAY ta'sirga ega bo'ling!




CSS kontur kengligi

Konturning kengligi outline-width xususiyati yordamida belgilanadi va bu kontur kengligi bir nechta bo'lishi mumkin

qiymatlar:



     yupqa (odatda 1px)
     o'rtacha (odatda 3px)
     qalin (odatda 5px)
     Muayyan o'lcham (px, pt, sm, em va boshqalarda)

Kontur kengligini qanday belgilashga misol quyida ko'rsatilgan:


<!DOCTYPE html>
<html>
<head>
<uslub>
p.ex1 {
   chegara: 1px qattiq qora;
   kontur uslubi: qattiq;
   kontur rangi: qizil;
   kontur kengligi: ingichka;
}

p.ex2 {
   chegara: 1px qattiq qora;
   kontur uslubi: qattiq;
   kontur rangi: qizil;
   kontur kengligi: o'rtacha;
}

p.ex3 {
   chegara: 1px qattiq qora;
   kontur uslubi: qattiq;
   kontur rangi: qizil;
   kontur kengligi: qalin;
}

p.ex4 {
   chegara: 1px qattiq qora;
   kontur uslubi: qattiq;
   kontur rangi: qizil;
   kontur kengligi: 4px;
}
</style>
</head>
<tana>

<h2>Kontur kengligi xossasi</h2>

<p class="ex1">Yupqa kontur.</p>
<p class="ex2">O'rtacha kontur.</p>
<p class="ex3">Qalin kontur.</p>
<p class="ex4">4px qalinlikdagi kontur.</p>

</body>
</html>



CSS kontur rangi::


CSS kontur rangi

Outline-color xossasi kontur rangini belgilash uchun ishlatiladi.

Rangni quyidagicha sozlash mumkin:

     nom - "qizil" kabi rang nomini belgilang
     HEX - "#ff0000" kabi olti burchakli qiymatni belgilang
     RGB - RGB qiymatini belgilang, masalan, "rgb (255,0,0)"
     HSL - "hsl(0, 100%, 50%)" kabi HSL qiymatini belgilang
     invert - rangni o'zgartirishni amalga oshiradi (bu rangdan qat'iy nazar konturning ko'rinishini ta'minlaydi.

fon)


Outline-color xususiyatini qo'llash misoli quyida ko'rsatilgan:

<!DOCTYPE html>
<html>
<head>
<uslub>
p.ex1 {
   chegara: 2px qattiq qora;
   kontur uslubi: qattiq;
   kontur rangi: qizil;
}

p.ex2 {
   chegara: 2px qattiq qora;
   kontur uslubi: nuqta;
   kontur rangi: ko'k;
}

p.ex3 {
   chegara: 2px qattiq qora;
   kontur uslubi: boshlanish;
   kontur rangi: kulrang;
}
</style>
</head>
<tana>

<h2>Kontur-rang xususiyati</h2>
<p>Outline-color xususiyati kontur rangini belgilash uchun ishlatiladi.</p>

<p class="ex1">Yaxshi qizil kontur.</p>
<p class="ex2">Nuqtali ko'k kontur.</p>
<p class="ex3">Dastlabki kulrang kontur.</p>

</body>
</html>




HEX qiymatlari

O'n oltilik qiymat quyida ko'rsatilgandek kontur rangini belgilash uchun ishlatilishi mumkin:


<!DOCTYPE html>
<html>
<head>
<uslub>
p.ex1 {
   chegara: 2px qattiq qora;
   kontur uslubi: qattiq;
   kontur rangi: #ff0000; /* qizil */
}

p.ex2 {
   chegara: 2px qattiq qora;
   kontur uslubi: nuqta;
   kontur rangi: #0000ff; /* ko'k */
}

p.ex3 {
   chegara: 2px qattiq qora;
   kontur uslubi: qattiq;
   kontur rangi: #bbbbbb; /* kulrang */
}
</style>
</head>
<tana>

<h2>Kontur-rang xususiyati</h2>
<p>Kontur rangini oʻn oltilik qiymat (HEX) yordamida ham belgilash mumkin:</p>

<p class="ex1">Yaxshi qizil kontur.</p>
<p class="ex2">Nuqtali ko'k kontur.</p>
<p class="ex3">Bir tekis kulrang kontur.</p>

</body>
</html>


RGB qiymatlari

RGB qiymatlari quyida ko'rsatilganidek, kontur rangini belgilash uchun ham ishlatilishi mumkin:


<!DOCTYPE html>
<html>
<head>
<uslub>
p.ex1 {
   chegara: 2px qattiq qora;
   kontur uslubi: qattiq;
   kontur rangi: rgb(255, 0, 0); /* qizil */
}

p.ex2 {
   chegara: 2px qattiq qora;
   kontur uslubi: nuqta;
   kontur rangi: rgb(0, 0, 255); /* ko'k */
}

p.ex3 {
   chegara: 2px qattiq qora;
   kontur uslubi: qattiq;
   kontur rangi: rgb(187, 187, 187); /* kulrang */
}
</style>
</head>
<tana>

<h2>Kontur-rang xususiyati</h2>
<p>Kontur rangi RGB qiymatlari yordamida ham belgilanishi mumkin:</p>

<p class="ex1">Yaxshi qizil kontur.</p>
<p class="ex2">Nuqtali ko'k kontur.</p>
<p class="ex3">Bir tekis kulrang kontur.</p>

</body>
</html>




HSL qiymatlari

HSL qiymatlari (rang, to'yinganlik va yorug'lik qiymatlari) CSS rangini belgilash uchun ham ishlatilishi mumkin.

quyida ko'rsatilgandek kontur:


<!DOCTYPE html>
<html>
<head>
<uslub>
p.ex1 {
   chegara: 2px qattiq qora;
   kontur uslubi: qattiq;
   kontur rangi: hsl(0, 100%, 50%); /* qizil */
}

p.ex2 {
   chegara: 2px qattiq qora;
   kontur uslubi: nuqta;
   kontur rangi: hsl(240, 100%, 50%); /* ko'k */
}

p.ex3 {
   chegara: 2px qattiq qora;
   kontur uslubi: qattiq;
   kontur rangi: hsl(0, 0%, 73%); /* kulrang */
}
</style>
</head>
<tana>

<h2>Kontur-rang xususiyati</h2>
<p>Kontur rangi HSL qiymatlari yordamida ham belgilanishi mumkin:</p>

<p class="ex1">Yaxshi qizil kontur.</p>
<p class="ex2">Nuqtali ko'k kontur.</p>
<p class="ex3">Bir tekis kulrang kontur.</p>

</body>
</html>





Rangni o'zgartirish

Kontur rangi: invert rangni inversiyani amalga oshiradi, bu esa konturning qanday bo'lishidan qat'i nazar, ko'rinishini ta'minlaydi.

fon rangi.

<!DOCTYPE html>
<html>
<head>
<uslub>
p.ex1 {
   chegara: 1px qattiq sariq;
   kontur uslubi: qattiq;
   kontur-rang: invert;
}
</style>
</head>
<tana>

<h2>Outline-color:invert dan foydalanish</h2>

<p class="ex1">Qattiq teskari kontur.</p>

</body>
</html>


CSS-ning qisqacha matni::


CSS Outline - Stenografiya xususiyati

Outline xususiyati quyidagi individual kontur xususiyatlarini o'rnatish uchun stenografiya xususiyatidir:

     kontur kengligi
     kontur uslubi (majburiy)
     kontur-rang

Kontur xususiyati yuqoridagi roʻyxatdagi bir, ikki yoki uchta qiymat sifatida koʻrsatilgan. Qiymatlarning tartibi

farqi yo'q.

Quyidagi misolda stenogramma kontur xususiyati bilan belgilangan ba'zi konturlar ko'rsatilgan:


<!DOCTYPE html>
<html>
<head>
<uslub>
p.ex1 {kontur: chizilgan;}
p.ex2 {kontur: nuqta qizil;}
p.ex3 (kontur: 5px qattiq sariq;}
p.ex4 {kontur: qalin tizma pushti;}
</style>
</head>
<tana>

<h2>Konturiy xususiyat</h2>

<p class="ex1">Chiziq chiziq.</p>
<p class="ex2">Nuqtali qizil kontur.</p>
<p class="ex3">5px qattiq sariq kontur.</p>
<p class="ex4">Qalin tog'li pushti kontur.</p>

</body>
</html>



CSS Outline ofset

Outline-offset xususiyati kontur va elementning cheti/chegarasi orasidagi bo'shliqni kiritish uchun ishlatiladi,

element va uning konturlari orasidagi bo'shliqni shaffof qoldirish.


Quyidagi skriptda kontur ofset elementga qanday qo'shilganligi ko'rsatilgan, shunda kontur 15px tashqarida bo'ladi.

<p> elementining chegarasi:


<!DOCTYPE html>
<html>
<head>
<uslub>
p {
   chegara: 30px;
   chegara: 1px qattiq qora;
   kontur: 1px qattiq qizil;
   kontur-ofset: 15px;
}
</style>
</head>
<tana>

<h2>Kontur-offset xususiyati</h2>

<p>Ushbu paragraf chegaradan tashqarida 15px konturga ega.</p>

</body>
</html>



Element chegarasi va uning kontur ofseti orasidagi bo'shliq shaffof ekanligini tasavvur qilish uchun


<!DOCTYPE html>
<html>
<head>
<uslub>
p {
   chegara: 30px;
   fon: sariq;
   chegara: 1px qattiq qora;
   kontur: 1px qattiq qizil;
   kontur-ofset: 15px;
}
</style>
</head>
<tana>

<h2>Kontur-offset xususiyati</h2>

<p>Ushbu paragraf chegaradan tashqarida 15px konturga ega.</p>

</body>
</html>



Barcha CSS Outline xususiyatlari umumlashtirilgan

Barcha CSS Outline xususiyatlari
Mulk tavsifi
kontur Kontur-kenglik, kontur-uslub va kontur-rangni birida oʻrnatish uchun stenografiya xususiyati

deklaratsiya
outline-color Kontur rangini o'rnatadi
outline-offset Kontur va elementning cheti yoki chegarasi orasidagi bo'shliqni belgilaydi
outline-style Kontur uslubini o'rnatadi
outline-width Konturning kengligini o'rnatadi


<kbd>qaytish</kbd>[Mundarijaga qaytish](#homepage)



-----------


# CSS matni

Biz ushbu bo'lim va keyingi bo'limlar ostida CSS-da matnlarni formatlashda foydalaniladigan xususiyatlarni tushuntiramiz.


Matnni formatlash misoli quyida ko'rsatilgan:



<!DOCTYPE html>
<html>
<head>
<uslub>
div {
   chegara: 1px qattiq kulrang;
   to'ldirish: 8px;
}

h1 {
   matnni tekislash: markaz;
   matnni o'zgartirish: katta harf;
   rang: #4CAF50;
}

p {
   matn chegarasi: 50px;
   matnni tekislash: oqlash;
   harflar oralig'i: 3px;
}

a {
   matn-bezak: yo'q;
   rang: #008CBA;
}
</style>
</head>
<tana>

<div>
   <h1>matnni formatlash</h1>
   <p>Ushbu matn matnni formatlashning ba'zi xususiyatlari bilan yaratilgan. Sarlavha matnni tekislashdan foydalanadi,

matnni o'zgartirish va rang xususiyatlari.
   Abzas ichkariga kiritiladi, tekislanadi va belgilar orasidagi bo'shliq belgilanadi. Pastki chiziq

bu rangdan olib tashlangan
   <a target="_blank" href="tryit.asp?filename=trycss_text">"O‘zingiz sinab ko‘ring"</a> havolasi.</p>
</div>

</body>
</html>




Matn rangi::

Color xususiyati matn rangini o'rnatish uchun ishlatiladi:


     rang nomi - "qizil" kabi
     HEX qiymati - "#ff0000" kabi
     RGB qiymati - "rgb (255,0,0)" kabi
Eslatma: Standart matn rangi yoki sahifa <style> teglari ostidagi "tana" selektorida aniqlanadi. Pastga qarang

masalan:



<!DOCTYPE html>
<html>
<head>
<uslub>
tana {
   rang: ko'k;
}

h1 {
   rang: yashil;
}
</style>
</head>
<tana>

<h1>Bu sarlavha 1</h1>
<p>Bu oddiy paragraf. E'tibor bering, bu matn ko'k rangda. Sahifa uchun standart matn rangi

tana selektorida belgilangan.</p>
<p>Boshqa paragraf.</p>

</body>
</html>


Eslatma: W3C-ga mos keladigan CSS uchun: Agar rang xususiyatini aniqlasangiz, fon rangini ham belgilashingiz kerak.



Matn rangi va fon rangi

Ushbu misolda biz fon rangi xususiyatini ham, rang xususiyatini ham aniqlaymiz (element uchun):


<!DOCTYPE html>
<html>
<head>
<uslub>
tana {
   fon rangi: och kulrang;
   rang: ko'k;
}

h1 {
   fon rangi: qora;
   rang: oq;
}
</style>
</head>
<tana>

<h1>Bu sarlavha oq matn bilan qora rangda</h1>
<p>Ushbu sahifa kulrang fon rangi va koʻk matnga ega.</p>
<p>Boshqa paragraf.</p>

</body>
</html>




CSS matnni tekislash::

CSS text-align xususiyati matnning gorizontal tekislanishini chapga, o'ngga yoki oqlangan tomonga o'rnatish uchun ishlatiladi.

tekislangan. Agar matn yo'nalishi chapdan o'ngga bo'lsa, standart hizalama chapda bo'ladi. Boshqa tomondan, agar matn

o'ngdan chapga, standart hizalama o'ngga. Matnni tekislash xususiyatidan foydalanish misoli ko'rsatilgan

quyida:

<!DOCTYPE html>
<html>
<head>
<uslub>
h1 {
   matnni tekislash: markaz;
}

h2 {
   matnni tekislash: chapga;
}

h3 {
   matnni tekislash: o'ngga;
}
</style>
</head>
<tana>

<h1>1-sarlavha (markazda)</h1>
<h2>2-sarlavha (chapda)</h2>
<h3>3-sarlavha (o'ngda)</h3>

<p>Yuqoridagi uchta sarlavha markazga, chapga va oʻngga tekislangan.</p>

</body>
</html>


Matnni tekislash xususiyati "oqlash" ga o'rnatilganda, har bir satr teng kenglikka ega bo'lishi uchun har bir satr uzaytiriladi,

va chap va o'ng chetlari tekis (jurnal va gazetalardagi kabi):

<!DOCTYPE html>
<html>
<head>
<uslub>
div {
   chegara: 1px qattiq qora;
   to'ldirish: 10px;
   kengligi: 200px;
   balandligi: 200px;
   matnni tekislash: oqlash;
}
</style>
</head>
<tana>

<h1>Matnni tekislash misoli: oqlash;</h1>

<p>Matnni tekislash: asoslash; qiymat chiziqlarni har bir satrning kengligi teng bo'lishi uchun uzaytiradi (gazetalardagi kabi

va jurnallar).</p>

<div>
Yoshroq va zaifroq yillarimda otam menga bir qancha maslahatlar berdi, men xayolimda o'girilib yurganman.

shundan buyon. — Qachonki siz kimnidir tanqid qilmoqchi bo'lsangiz, - dedi u menga, - shuni yodda tutingki, hamma odamlar

Bu dunyoda sizlar kabi afzalliklar yo'q.
</div>

</body>
</html>



Matn yo'nalishi

Yo'nalish va unicode-bidi (har bir harfni chapdan o'ngga o'zgartirish) xususiyatlaridan foydalanish mumkin

elementning matn yo'nalishini o'zgartirish:

<!DOCTYPE html>
<html>
<head>
<uslub>
p.ex1 {
   yo'nalishi: rtl;
   unicode-bidi: bidi-override;
}
</style>
</head>
<tana>

<p>Bu standart matn yoʻnalishi.</p>

<p class="ex1">Bu matnning o'ngdan chapga yo'nalishi.</p>

</body>
</html>


Vertikal tekislash

Vertical-align xususiyati elementning vertikal tekislanishini o'rnatadi. Quyidagi misol qanday o'rnatishni ko'rsatadi

matndagi tasvirning vertikal tekislanishi.



<!DOCTYPE html>
<html>
<head>
<uslub>
img.a {
   vertikal tekislash: asosiy chiziq;
}

img.b {
   vertikal tekislash: matn tepasiga;
}

img.c {
   vertikal tekislash: matn-pastki;
}

img.d {
   vertikal tekislash: pastki;
}

img.e {
   vertikal tekislash: super;
}
</style>
</head>
<tana>

<h1>Vertikal tekislash xususiyati</h1>

<h2>vertikal tekislash: asosiy chiziq (standart):</h2>
<p>Birlamchi tekislangan <img class="a" src="sqpurple.gif" width="9" height="9"> rasm.</p>

<h2>vertikal tekislash: matn tepasida:</h2>
<p><img class="b" src="sqpurple.gif" width="9" height="9"> rasm, matn tepasiga tekislangan.</p>

<h2>vertikal tekislash: matn-pastki:</h2>
<p><img class="c" src="sqpurple.gif" width="9" height="9"> rasm, matnning pastki qismiga tekislangan.</p>

<h2>vertikal tekislash: pastki:</h2>
<p><img class="d" src="sqpurple.gif" width="9" height="9"> pastki tekislangan rasm.</p>

<h2>vertikal tekislash: sup:</h2>
<p>Super tekislangan <img class="e" src="sqpurple.gif" width="9" height="9"> rasm.</p>

</body>
</html>



CSS matnni bezash


Matnni bezash

Matnni bezash xususiyati matndan bezaklarni o'rnatish yoki olib tashlash uchun ishlatiladi.

Matn-bezatish qiymati: yo'q; ko'pincha havolalardan pastki chiziqni olib tashlash uchun ishlatiladi:



<!DOCTYPE html>
<html>
<head>
<uslub>
a {
   matn-bezak: yo'q;
}
</style>
</head>
<tana>

<p>Ustiga chizilmagan havola: <a href="https://www.w3schools.com">W3Schools.com</a></p>

</body>
</html>




Boshqa matnni bezash qiymatlari quyida ko'rsatilgan:


<!DOCTYPE html>
<html>
<head>
<uslub>
h1 {
   matn-bezatish: yuqori chiziq;
}

h2 {
   matn-bezak: chiziq orqali;
}

h3 {
   matnni bezash: tagiga chizish;
}
</style>
</head>
<tana>

<h1>Bu sarlavha 1</h1>
<h2>Bu 2-sarlavha</h2>
<h3>Bu 3-sarlavha</h3>

</body>
</html>


Eslatma: havola bo'lmagan matnning tagiga chizish tavsiya etilmaydi, chunki bu ko'pincha o'quvchini chalkashtirib yuboradi.



Matnni o'zgartirish::

Matnni o'zgartirish xususiyati matndagi katta va kichik harflarni belgilash uchun ishlatiladi.

U hamma narsani katta yoki kichik harflarga aylantirish yoki birinchi harfini katta qilish uchun ishlatilishi mumkin

har bir so'z:



<!DOCTYPE html>
<html>
<head>
<uslub>
p.katta {
   matnni o'zgartirish: katta harf;
}

p.kichik harf {
   matnni o'zgartirish: kichik harflar;
}

p.kapitalizatsiya {
   matnni o'zgartirish: bosh harf bilan yozish;
}
</style>
</head>
<tana>

<p class="uppercase">Bu qandaydir matn.</p>
<p class="lowercase">Bu qandaydir matn.</p>
<p class="capitalize">Bu qandaydir matn.</p>

</body>
</html>






CSS matn oralig'i::

Text-indent xossasi matnning birinchi qatorining chekinishini belgilash uchun ishlatiladi.



<!DOCTYPE html>
<html>
<head>
<uslub>
p {
   matn chegarasi: 50px;
}
</style>
</head>
<tana>

<p>Yosh va zaif yillarimda otam menga bir necha maslahatlar berdi, men ularni hayotimda o'zgartiraman.

o'shandan beri aql. — Qachonki siz kimnidir tanqid qilmoqchi bo'lsangiz, - dedi u menga, - hamma odamlar buni yodda tutinglar

Bu dunyoda siz ega bo'lgan afzalliklar yo'q.'</p>

</body>
</html>



Harf oralig'i

Harf oralig'i xususiyati matndagi belgilar orasidagi bo'shliqni belgilash uchun ishlatiladi.

Quyidagi misol belgilar orasidagi bo'shliqni qanday oshirish yoki kamaytirishni ko'rsatadi:


<!DOCTYPE html>
<html>
<head>
<uslub>
h1 {
   harflar oralig'i: 3px;
}

h2 {
   harflar oralig'i: -3px;
}
</style>
</head>
<tana>

<h1>Bu sarlavha 1</h1>
<h2>Bu 2-sarlavha</h2>

</body>
</html>




Chiziq balandligi

Line-height xususiyati qatorlar orasidagi bo'shliqni belgilash uchun ishlatiladi:


<!DOCTYPE html>
<html>
<head>
<uslub>
p.kichik {
   chiziq balandligi: 0,7;
}

katta {
   chiziq balandligi: 1,8;
}
</style>
</head>
<tana>

<p>
Bu standart satr balandligidagi paragraf.<br>
Ko'pgina brauzerlarda standart satr balandligi taxminan 110% dan 120% gacha.<br>
</p>

<p class="kichik">
Bu kichikroq satr balandligidagi paragraf.<br>
Bu kichikroq satr balandligidagi paragraf.<br>
</p>

<p class="katta">
Bu kattaroq satr balandligidagi paragraf.<br>
Bu kattaroq satr balandligidagi paragraf.<br>
</p>

</body>
</html>















































So'z oralig'i

So'z oralig'i xususiyati matndagi so'zlar orasidagi bo'shliqni ko'rsatish uchun ishlatiladi.

Quyidagi misolda bo'sh joyni qanday oshirish (ijobiy qiymat) yoki kamaytirish (salbiy qiymat) ko'rsatilgan

so'zlar orasida:


<!DOCTYPE html>
<html>
<head>
<uslub>
h1 {
   so'zlar oralig'i: 10px;
}

h2 {
   so'z oralig'i: -5px;
}
</style>
</head>
<tana>

<h1>Bu sarlavha 1</h1>
<h2>Bu 2-sarlavha</h2>

</body>
</html>




Oq bo'shliq

White-space xususiyati element ichidagi bo'sh joy qanday ishlov berilishini belgilaydi.

Ushbu misol element ichidagi matnni o'rashni qanday o'chirishni ko'rsatadi:



<!DOCTYPE html>
<html>
<head>
<uslub>
p {
   oq bo'shliq: nowrap;
}
</style>
</head>
<tana>

<h2>Oq bo'shliq</h2>

<p>
Bu qandaydir matn. Bu qandaydir matn. Bu qandaydir matn.
Bu qandaydir matn. Bu qandaydir matn. Bu qandaydir matn.
Bu qandaydir matn. Bu qandaydir matn. Bu qandaydir matn.
Bu qandaydir matn. Bu qandaydir matn. Bu qandaydir matn.
Bu qandaydir matn. Bu qandaydir matn. Bu qandaydir matn.
</p>

<p>Farqni ko'rish uchun bo'sh joy xususiyatini olib tashlashga harakat qiling.</p>

</body>
</html>






CSS matn soyasi::


Matn soyasi

Matn-shadow xossasi matnga soya qo‘shadi.

Eng oddiy foydalanishda siz faqat gorizontal soyani (2px) va vertikal soyani (2px) belgilaysiz:


<!DOCTYPE html>
<html>
<head>
<uslub>
h1 {
   matn soyasi: 2px 2px;
}
</style>
</head>
<tana>

<h1>Matn-soya effekti!</h1>

</body>
</html>




Soyaga rang (qizil) qo'shish uchun:

<!DOCTYPE html>
<html>
<head>
<uslub>
h1 {
   matn soyasi: 2px 2px qizil;
}
</style>
</head>
<tana>

<h1>Matn-soya effekti!</h1>

</body>
</html>




Soyaga loyqalik effektini (5px) qo'shish uchun:


<!DOCTYPE html>
<html>
<head>
<uslub>
h1 {
   matn soyasi: 2px 2px 5px qizil;
}
</style>
</head>
<tana>

<h1>Matn-soya effekti!</h1>

</body>
</html>


<kbd>qaytish</kbd>[Mundarijaga qaytish](#homepage)


--------



## CSS shriftlari


To'g'ri fond veb-saytning UX-ni yaxshilashi va noyob va kuchli brend identifikatorini yaratishi mumkin. O'qish qobiliyati

shrift matnga qiymat qo'shishi uchun shrift juda muhim. Shriftning rangi va matn hajmi ham muhimdir

shrift tanlash.



Umumiy shrift oilalari

CSS-da beshta umumiy shrift oilasi mavjud:

     Serif shriftlari har bir harfning chetida kichik chiziqqa ega. Ular rasmiyatchilik hissi yaratadi va

nafislik.
     Sans-serif shriftlari toza chiziqlarga ega (kichik chiziqlar biriktirilmagan). Ular zamonaviy va minimalizmni yaratadilar

qarang.
     Monospace shriftlari - bu erda barcha harflar bir xil sobit kenglikka ega. Ular mexanik ko'rinish hosil qiladi.
     Cursive shriftlar inson qo'l yozuviga taqlid qiladi.
     Fantaziya shriftlari dekorativ/o'ynoqi shriftlardir.

Barcha shrift nomlari umumiy shrift oilalaridan biriga tegishli.



Eslatma: Kompyuter ekranlarida sans-serif shriftlari serif shriftlarga qaraganda osonroq o'qiladi.


Ba'zi shriftlarga misollar

Shrift nomlarining umumiy shrift turkumiga misollar


Serif Times New Roman, Jorjiya, Garamond

Sans-serif Arial Verdana, Helvetica

Monospace Courier New, Lucida Console, Monako,

Cursive Brush Script MT, Lucida Handwriting

Fantasy mis plastinka, papirus



CSS shrift oilasi xususiyati

CSS-da biz matn shriftini belgilash uchun font-family xususiyatidan foydalanamiz.

Shrift-family xususiyati maksimal darajada ta'minlash uchun "qayta" tizim sifatida bir nechta shrift nomlariga ega bo'lishi kerak

brauzerlar/operatsion tizimlar o'rtasidagi muvofiqlik. O'zingiz xohlagan shrift bilan boshlang va umumiy bilan tugating

oila (agar boshqa shriftlar mavjud bo'lmasa, brauzerga umumiy oilada o'xshash shriftni tanlashiga ruxsat berish uchun). The

shrift nomlari vergul bilan ajratilishi kerak.

Eslatma: Agar shrift nomi bir nechta so'zlardan iborat bo'lsa, u tirnoq ichida bo'lishi kerak, masalan: "Times New Roman".

CSS-da font-family qo'llanilishiga misol quyida ko'rsatilgan:


<!DOCTYPE html>
<html>
<head>
<uslub>
.p1 {
   shrift oilasi: "Times New Roman", Times, serif;
}

.p2 {
   shrift oilasi: Arial, Helvetica, sans-serif;
}

.p3 {
   shrift oilasi: "Lucida Console", "Courier New", monospace;
}
</style>
</head>
<tana>

<h1>CSS font-family</h1>
<p class="p1">Bu paragraf Times New Roman shriftida ko'rsatilgan.</p>
<p class="p2">Bu Arial shriftida ko'rsatilgan paragraf.</p>
<p class="p3">Bu Lucida Console shriftida ko'rsatilgan paragraf.</p>

</body>
</html>



CSS veb-xavfsiz shriftlari::

Ular barcha brauzerlar va qurilmalarda universal o'rnatilgan shriftlardir.


Qayta shriftlar: 100% veb-xavfsiz shriftlar mavjud emasligi sababli, agar shrift bo'lmasa, har doim zaxira shriftlardan foydalaning.

topilgan yoki brauzer yoki qurilmada to'g'ri o'rnatilmagan.


Har doim font-family xususiyatiga o'xshash "zaxira shriftlar" ro'yxatini qo'shishingiz kerak. Agar birinchi shrift shunday qilsa.

ishlamasa, brauzer keyingisini sinab ko'radi va keyingisini va hokazo. Har doim ro'yxatni umumiy bilan yakunlang

shrift familiyasi.



Ushbu kontseptsiyaning tasviri quyida ko'rsatilgan:


<!DOCTYPE html>
<html>
<head>
<uslub>
p {
font-family: Tahoma, Verdana, sans-serif;
}
</style>
</head>
<tana>

<h1>CSS-ning orqa fontlari</h1>

<p>Bu paragraf.</p>
<p>Bu boshqa paragraf.</p>

</body>
</html>



HTML va CSS uchun eng yaxshi veb-xavfsiz shriftlar

Quyidagi ro'yxat HTML va CSS uchun eng yaxshi veb-xavfsiz shriftlardir:

     Arial (sans-serif)
     Verdana (sans-serif)
     Helvetica (sans-serif)
     Tahoma (sans-serif)
     Trebuchet MS (sans-serif)
     Times New Roman (serif)
     Gruziya (serif)
     Garamond (serif)
     Courier New (bir fazo)
     Brush Script MT (kursiv)

Eslatma: Veb-saytingizni nashr etishdan oldin har doim shriftlaringiz turli brauzer va qurilmalarda qanday ko‘rinishini tekshiring.

va har doim zaxira shriftlardan foydalaning!


Arial (sans-serif)

Arial ham onlayn, ham bosma ommaviy axborot vositalari uchun eng keng tarqalgan shriftdir. Arial ham standart shrift hisoblanadi

Google Docs.

Arial eng xavfsiz veb-shriftlardan biri bo'lib, u barcha asosiy operatsion tizimlarda mavjud.

Font-family bilan arial shriftni belgilashga misol



<!DOCTYPE html>
<html>
<head>
<uslub>
tana {
   font-family: Arial, sans-serif;
}
</style>
</head>
<tana>

<h1>Lorem ipsum dolor sit amet</h1>

<p>Lorem ipsum dolor sit amet.</p>
<p>0 1 2 3 4 5 6 7 8 9</p>

</body>
</html>



Verdana (sans-serif)

Verdana - juda mashhur shrift. Verdana hatto kichik shrift o'lchamlari uchun ham oson o'qilishi mumkin.


<!DOCTYPE html>
<html>
<head>
<uslub>
tana {
   font-family: Verdana, sans-serif;
}
</style>
</head>
<tana>

<h1>Lorem ipsum dolor sit amet</h1>

<p>Lorem ipsum dolor sit amet.</p>
<p>0 1 2 3 4 5 6 7 8 9</p>

</body>
</html>



Helvetica (sans-serif)

Helvetica shrifti dizaynerlar tomonidan yaxshi ko'riladi. Bu ko'plab biznes turlari uchun javob beradi. Quyidagi misolga qarang:


<!DOCTYPE html>
<html>
<head>
<uslub>
tana {
   font-family: Helvetica, sans-serif;
}
</style>
</head>
<tana>

<h1>Lorem ipsum dolor sit amet</h1>

<p>Lorem ipsum dolor sit amet.</p>
<p>0 1 2 3 4 5 6 7 8 9</p>

</body>
</html>




Tahoma (sans-serif)

Tahoma shriftida belgilar orasidagi bo'sh joy kamroq. Quyidagi misolga qarang:


<!DOCTYPE html>
<html>
<head>
<uslub>
tana {
   font-family: Tahoma, sans-serif;
}
</style>
</head>
<tana>

<h1>Lorem ipsum dolor sit amet</h1>

<p>Lorem ipsum dolor sit amet.</p>
<p>0 1 2 3 4 5 6 7 8 9</p>

</body>
</html>


Trebuchet MS (sans-serif)

Trebuchet MS 1996 yilda Microsoft tomonidan ishlab chiqilgan. Ushbu shriftdan ehtiyotkorlik bilan foydalaning. Barcha mobil qurilmalar tomonidan qo'llab-quvvatlanmaydi

operatsion tizimlar. Quyidagi misolga qarang:



<!DOCTYPE html>
<html>
<head>
<uslub>
tana {
   font-family: 'Trebuchet MS', sans-serif;
}
</style>
</head>
<tana>

<h1>Lorem ipsum dolor sit amet</h1>

<p>Lorem ipsum dolor sit amet.</p>
<p>0 1 2 3 4 5 6 7 8 9</p>

</body>
</html>



Times New Roman (serif)

Times New Roman - dunyodagi eng taniqli shriftlardan biri. Bu professional ko'rinadi va ishlatiladi

ko'plab gazetalar va "yangiliklar" veb-saytlari. Shuningdek, u Windows qurilmalari va ilovalari uchun asosiy shrift hisoblanadi. Qarang

misol bnw


<!DOCTYPE html>
<html>
<head>
<uslub>
tana {
   font-family: 'Times New Roman', serif;
}
</style>
</head>
<tana>

<h1>Lorem ipsum dolor sit amet</h1>

<p>Lorem ipsum dolor sit amet.</p>
<p>0 1 2 3 4 5 6 7 8 9</p>

</body>
</html>



Gruziya (serif)

Gruziya nafis serif shrifti. Turli shrift o'lchamlarida juda o'qilishi mumkin, shuning uchun u yaxshi nomzoddir

mobil javob beruvchi dizayn. Quyidagi misolga qarang:


<!DOCTYPE html>
<html>
<head>
<uslub>
tana {
   shrift oilasi: Georgia, serif;
}
</style>
</head>
<tana>

<h1>Lorem ipsum dolor sit amet</h1>

<p>Lorem ipsum dolor sit amet.</p>
<p>0 1 2 3 4 5 6 7 8 9</p>

</body>
</html>


Garamond (serif)

Garamond - ko'plab bosma kitoblar uchun ishlatiladigan klassik shrift. U abadiy ko'rinishga ega va yaxshi o'qilishi mumkin. Qarang

quyidagi misol:

<!DOCTYPE html>
<html>
<head>
<uslub>
tana {
   shrift oilasi: Garamond, serif;
}
</style>
</head>
<tana>

<h1>Lorem ipsum dolor sit amet</h1>

<p>Lorem ipsum dolor sit amet.</p>
<p>0 1 2 3 4 5 6 7 8 9</p>

</body>
</html>



Courier New (bir fazo)

Courier New - eng keng tarqalgan monospace serif shrifti. Courier New ko'pincha kodlash displeylari bilan ishlatiladi,

va ko'pgina elektron pochta provayderlari undan standart shrift sifatida foydalanadilar. Courier New ham kino uchun standart shrift hisoblanadi

ssenariylar.



<!DOCTYPE html>
<html>
<head>
<uslub>
tana {
   font-family: 'Courier New', monospace;
}
</style>
</head>
<tana>

<h1>Lorem ipsum dolor sit amet</h1>

<p>Lorem ipsum dolor sit amet.</p>
<p>0 1 2 3 4 5 6 7 8 9</p>

</body>
</html>


Brush Script MT (kursiv)

Brush Script MT shrifti qo'l yozuviga taqlid qilish uchun yaratilgan. Bu oqlangan va murakkab, ammo qiyin bo'lishi mumkin

o'qish. Ehtiyotkorlik bilan foydalaning. Quyidagi misolga qarang:


<!DOCTYPE html>
<html>
<head>
<uslub>
tana {
   font-family: 'Brush Script MT', kursiv;
}
</style>
</head>
<tana>

<h1>Lorem ipsum dolor sit amet</h1>

<p>Lorem ipsum dolor sit amet.</p>
<p>0 1 2 3 4 5 6 7 8 9</p>

</body>
</html>



CSS shriftlarining qaytarilishi::


Tez-tez ishlatiladigan shriftlarni tiklash

Quyida 5 ta umumiy shrift oilalari tomonidan tashkil etilgan ba'zi tez-tez ishlatiladigan shrift zaxiralari keltirilgan:

     Serif
     Sans-serif
     Monospace
     Kursiv
     Fantaziya

Turli shrift oilalari va ularni amalga oshirish uchun mos skript quyida ko'rsatilgan:


Serif shriftlari:::


font-family ("Times New Roman", Times, serif). quyidagi kodni ko'ring:

<!DOCTYPE html>
<html>
<head>
<uslub>
tana {
   shrift oilasi: "Times New Roman", Times, serif;
}
</style>
</head>
<tana>

<h1>Lorem ipsum dolor sit amet</h1>

<p>Lorem ipsum dolor sit amet.</p>
<p>0 1 2 3 4 5 6 7 8 9</p>

</body>
</html>



font-family (Gruziya, serif). Quyidagi kodga qarang:

<!DOCTYPE html>
<html>
<head>
<uslub>
tana {
   shrift oilasi: Georgia, serif;
}
</style>
</head>
<tana>

<h1>Lorem ipsum dolor sit amet</h1>

<p>Lorem ipsum dolor sit amet.</p>
<p>0 1 2 3 4 5 6 7 8 9</p>

</body>
</html>



shrift oilasi (Garamond, serif). Quyida ularni qo'llash uchun kodni ko'ring:

<!DOCTYPE html>
<html>
<head>
<uslub>
tana {
   shrift oilasi: Garamond, serif;
}
</style>
</head>
<tana>

<h1>Lorem ipsum dolor sit amet</h1>

<p>Lorem ipsum dolor sit amet.</p>
<p>0 1 2 3 4 5 6 7 8 9</p>

</body>
</html>

Sans-Serif shriftlari:::

shrift oilasi (Arial, Helvetica, san-serif). Quyidagi amaliyotga qarang:

<!DOCTYPE html>
<html>
<head>
<uslub>
tana {
   shrift oilasi: Arial, Helvetica, sans-serif;
}
</style>
</head>
<tana>

<h1>Lorem ipsum dolor sit amet</h1>

<p>Lorem ipsum dolor sit amet.</p>
<p>0 1 2 3 4 5 6 7 8 9</p>

</body>
</html>



shrift oilasi (Tahoma, Verdana, sans-serif). Quyidagi amaliyotga qarang:

<!DOCTYPE html>
<html>
<head>
<uslub>
tana {
   font-family: Tahoma, Verdana, sans-serif;
}
</style>
</head>
<tana>

<h1>Lorem ipsum dolor sit amet</h1>

<p>Lorem ipsum dolor sit amet.</p>
<p>0 1 2 3 4 5 6 7 8 9</p>

</body>
</html>



shrift oilasi ("Trebuchet MS", Helvetica, sans-serif). Quyidagi amaliyotga qarang:


<!DOCTYPE html>
<html>
<head>
<uslub>
tana {
   shrift oilasi: "Trebuchet MS", Helvetica, sans-serif;
}
</style>
</head>
<tana>

<h1>Lorem ipsum dolor sit amet</h1>

<p>Lorem ipsum dolor sit amet.</p>
<p>0 1 2 3 4 5 6 7 8 9</p>

</body>
</html>



font-family (Gruziya, Verdana, sans-serif). Quyida amalga oshirishga qarang:

<!DOCTYPE html>
<html>
<head>
<uslub>
tana {
   font-family: Georgia, Verdana, sans-serif;
}
</style>
</head>
<tana>

<h1>Lorem ipsum dolor sit amet</h1>

<p>Lorem ipsum dolor sit amet.</p>
<p>0 1 2 3 4 5 6 7 8 9</p>

</body>
</html>



Monospace shriftlari:::

font-family ("Courier New", Courier, monospace). Quyida amalga oshirishga qarang:

<!DOCTYPE html>
<html>
<head>
<uslub>
tana {
   font-family: "Courier New", Courier, monospace;
}
</style>
</head>
<tana>

<h1>Lorem ipsum dolor sit amet</h1>

<p>Lorem ipsum dolor sit amet.</p>
<p>0 1 2 3 4 5 6 7 8 9</p>

</body>
</html>



Kursiv shriftlar:::

font-family ("Brush Script MT", kursiv). Ushbu shriftlar oilasini qanday amalga oshirishni quyida ko'ring:


<!DOCTYPE html>
<html>
<head>
<uslub>
tana {
   font-family: "Brush Script MT", kursiv;
}
</style>
</head>
<tana>

<h1>Lorem ipsum dolor sit amet</h1>

<p>Lorem ipsum dolor sit amet.</p>
<p>0 1 2 3 4 5 6 7 8 9</p>

</body>
</html>



Fantasy shriftlar:::

shrift oilasi (Mis plastinka, papirus, fantaziya). Ushbu shriftlar oilasini qanday amalga oshirishni quyida ko'ring:


<!DOCTYPE html>
<html>
<head>
<uslub>
tana {
   shrift oilasi: Copperplate, Papyrus, fantasy;
}
</style>
</head>
<tana>

<h1>Lorem ipsum dolor sit amet</h1>

<p>Lorem ipsum dolor sit amet.</p>
<p>0 1 2 3 4 5 6 7 8 9</p>

</body>
</html>





CSS shrift uslubi::


Shrift uslubi

Shrift uslubi xususiyati asosan kursiv matnni belgilash uchun ishlatiladi.

Bu xususiyat uchta qiymatga ega:

     normal - matn an'anaviy tarzda ko'rsatiladi
     kursiv - matn kursiv bilan ko'rsatiladi
     oblique - matn "egilgan" (qiyshiq kursivga juda o'xshaydi, lekin kamroq qo'llab-quvvatlanadi)


Shrift uslubini amalga oshirish quyida ko'rsatilgan:


<!DOCTYPE html>
<html>
<head>
<uslub>
p.normal {
   shrift uslubi: normal;
}

p. kursiv {
   shrift uslubi: kursiv;
}

p.oblique {
   shrift uslubi: qiya;
}
</style>
</head>
<tana>

<p class="normal">Bu oddiy uslubdagi paragraf.</p>
<p class="italic">Bu kursiv uslubidagi paragraf.</p>
<p class="oblique">Bu oblique uslubidagi paragraf.</p>

</body>
</html>




Shrift vazni

Font-weight xususiyati shrift og'irligini belgilaydi:


<!DOCTYPE html>
<html>
<head>
<uslub>
p.normal {
   shrift og'irligi: normal;
}

yorug'lik {
   shrift vazni: engilroq;
}

p.qalin {
   shrift vazni: qalin;
}

p.qalinroq {
   shrift og'irligi: 900;
}
</style>
</head>
<tana>

<p class="normal">Bu paragraf.</p>
<p class="light">Bu paragraf.</p>
<p class="thick">Bu paragraf.</p>
<p class="thicker">Bu paragraf.</p>

</body>
</html>


Shrift varianti

Font-variant xususiyati matnni kichik bosh harflar bilan ko'rsatish yoki ko'rsatmaslik kerakligini belgilaydi.

Kichik boshli shriftda barcha kichik harflar katta harflarga aylantiriladi. Biroq, aylantirilgan

katta harflar matndagi asl bosh harflardan kichikroq shrift o'lchamida ko'rinadi.

<!DOCTYPE html>
<html>
<head>
<uslub>
p.normal {
   shrift-variant: normal;
}

p.kichik {
   shrift-variant: kichik bosh harflar;
}
</style>
</head>
<tana>

<p class="normal">Mening ismim Xege Refsnes.</p>
<p class="small">Mening ismim Xege Refsnes.</p>

</body>
</html>




CSS shrift hajmi::



Shrift hajmi

Font-size xossasi matn hajmini belgilaydi.

Matn hajmini boshqarish qobiliyati veb-dizaynda muhim ahamiyatga ega. Biroq, siz shrift o'lchamidan foydalanmasligingiz kerak

paragraflarni sarlavhalarga yoki sarlavhalarni paragraflarga o'xshatish uchun tuzatishlar.

Har doim tegishli HTML teglaridan foydalaning, masalan, sarlavhalar uchun <h1> - <h6> va paragraflar uchun <p>.

Shrift o'lchami qiymati mutlaq yoki nisbiy o'lcham bo'lishi mumkin.

Mutlaq o'lcham:

     Matnni belgilangan hajmga o'rnatadi
     Foydalanuvchiga barcha brauzerlarda matn hajmini o'zgartirishga ruxsat bermaydi (mavjud sabablarga ko'ra yomon)
     Chiqarishning jismoniy hajmi ma'lum bo'lganda, mutlaq o'lcham foydalidir

Nisbiy o'lcham:

     Atrofdagi elementlarga nisbatan o'lchamni o'rnatadi
     Foydalanuvchiga brauzerlarda matn hajmini o'zgartirish imkonini beradi


Eslatma: Agar siz shrift o'lchamini belgilamasangiz, oddiy matn uchun standart o'lcham, masalan, paragraflar uchun, 16px.

(16px=1em).

Konvertatsiya koeffitsienti: 1em=12pt=16px=100%



Shrift hajmini piksellar bilan o'rnating

Matn o'lchamini piksellar bilan belgilash sizga matn hajmini to'liq boshqarish imkonini beradi:


<!DOCTYPE html>
<html>
<head>
<uslub>
h1 {
   shrift o'lchami: 40px;
}

h2 {
   shrift o'lchami: 30px;
}

p {
   shrift o'lchami: 14px;
}
</style>
</head>
<tana>

<h1>Bu sarlavha 1</h1>
<h2>Bu 2-sarlavha</h2>
<p>Bu paragraf.</p>
<p>Bu boshqa paragraf.</p>

</body>
</html>


Maslahat: Agar siz piksellardan foydalansangiz, butun sahifa hajmini o'zgartirish uchun masshtablash vositasidan foydalanishingiz mumkin.



Em bilan shrift hajmini o'rnating

Foydalanuvchilarga matn hajmini o'zgartirishga ruxsat berish uchun (brauzer menyusida) ko'plab ishlab chiquvchilar piksel o'rniga em-dan foydalanadilar.

1em joriy shrift hajmiga teng. Brauzerlarda standart matn hajmi 16px. Shunday qilib, standart o'lcham

1em 16px.

O'lchamni pikseldan emgacha quyidagi formula yordamida hisoblash mumkin: piksel/16=em

Quyidagi ilovaga qarang:


<!DOCTYPE html>
<html>
<head>
<uslub>
h1 {
   shrift hajmi: 2,5em; /* 40px/16=2,5em */
}

h2 {
   shrift hajmi: 1.875em; /* 30px/16=1.875em */
  }

p {
   shrift o'lchami: 0,875em; /* 14px/16=0,875em */
}
</style>
</head>
<tana>

<h1>Bu sarlavha 1</h1>
<h2>Bu 2-sarlavha</h2>
<p>Bu paragraf.</p>
<p>Em-da shrift o'lchamini belgilash barcha asosiy brauzerlarga matn hajmini o'zgartirish imkonini beradi.
Afsuski, IE ning eski versiyalari bilan bog'liq muammo hali ham mavjud. Matn o'lchamini o'zgartirganda, u bo'ladi

kerak bo'lganidan kattaroq/kichikroq.</p>

</body>
</html>



Yuqoridagi misolda emdagi matn hajmi piksellardagi oldingi misol bilan bir xil. Biroq, bilan

em o'lchami, barcha brauzerlarda matn hajmini sozlash mumkin.

Afsuski, Internet Explorer-ning eski versiyalarida muammo hali ham mavjud. Matn kattalashadi

kattaroq qilinganida kerak bo'lganidan va kichikroq qilinganidan kichikroq.




Foiz va Em birikmasidan foydalaning

Barcha brauzerlarda ishlaydigan yechim <body> elementi uchun foizda standart shrift o'lchamini o'rnatishdir:


<!DOCTYPE html>
<html>
<head>
<uslub>
tana {
   shrift o'lchami: 100%;
}

h1 {
   shrift hajmi: 2,5em;
}

h2 {
   shrift hajmi: 1.875em;
}

p {
   shrift o'lchami: 0,875em;
}
</style>
</head>
<tana>

<h1>Bu sarlavha 1</h1>
<h2>Bu 2-sarlavha</h2>
<p>Bu paragraf.</p>
<p>Shrift o‘lchamini foiz va em bilan belgilash barcha asosiy brauzerlarda bir xil o‘lchamni ko‘rsatadi va barchaga ruxsat beradi

matn hajmini o'zgartirish uchun brauzerlar!</p>

</body>
</html>


Eslatma: Bizning kodimiz endi ajoyib ishlaydi! U barcha brauzerlarda bir xil matn hajmini ko'rsatadi va barcha brauzerlarga kattalashtirish imkonini beradi

yoki matn hajmini o'zgartiring!



Javob beruvchi shrift hajmi

Matn o'lchamini vw birligi bilan o'rnatish mumkin, bu "ko'rish maydoni kengligi" degan ma'noni anglatadi. Viewport - bu brauzer oynasi

hajmi. 1vw = ko'rish maydoni kengligining 1%. Agar ko'rish maydoni 50 sm kengligida bo'lsa, 1vw 0,5 sm.

Shunday qilib, matn hajmi brauzer oynasining o'lchamiga mos keladi:


<!DOCTYPE html>
<html>
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<tana>

<h1 style="font-size:10vw;">Javob beruvchi matn</h1>

<p style="font-size:5vw;">Matn o'lchami qanday o'zgarishini ko'rish uchun brauzer oynasining o'lchamini o'zgartiring.</p>

<p style="font-size:5vw;">Matn o'lchamini belgilashda "vw" birligidan foydalaning. 10vw o'lchamni 10% ga o'rnatadi

ko'rish maydoni kengligi.</p>

<p>Viewport - bu brauzer oynasining o'lchami. 1vw = ko'rish maydoni kengligining 1%. Agar ko'rish oynasi kengligi 50 sm bo'lsa, 1vw

0,5 sm.</p>

</body>
</html>





CSS Google shriftlari::


Google shriftlari standart HTML-dan foydalanishni istamaydigan odamlar uchun 1000 dan ortiq bepul qo'shimcha shriftlardir.

shriftlar.

Google shriftlaridan qanday foydalanish

Faqat <head> bo'limiga maxsus uslublar jadvali havolasini qo'shing va keyin CSS-dagi shriftga murojaat qiling.



<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Sofia">
<uslub>
tana {
   font-family: "Sofiya", sans-serif;
}
</style>
</head>
<tana>

<h1>Sofiya shrifti</h1>
<p>Lorem ipsum dolor sit amet.</p>
<p>123456790</p>

</body>
</html>



Google Shriftlardan “Trirong” nomli shriftdan foydalanish uchun:

<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Trirong">
<uslub>
tana {
   shrift oilasi: "Tirong", serif;
}
</style>
</head>
<tana>

<h1>Trirong shrifti</h1>
<p>Lorem ipsum dolor sit amet.</p>
<p>123456790</p>

</body>
</html>


Google Fonts’dan “Audiowide” nomli shriftdan foydalanish uchun:

<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Audiowide">
<uslub>
tana {
   font-family: "Audiowide", sans-serif;
}
</style>
</head>
<tana>

<h1>Ovozli shrift</h1>
<p>Lorem ipsum dolor sit amet.</p>
<p>123456790</p>

</body>
</html>




Eslatma: CSS-da shriftni belgilashda har doim kamida bitta zaxira shrift ro'yxatini kiriting (kutilmagan holatlarning oldini olish uchun

xatti-harakatlari). Shunday qilib, bu erda siz umumiy shrift oilasini (masalan, serif yoki sans-serif) oxiriga qo'shishingiz kerak.

ro'yxati.

Barcha mavjud google shriftlarini bu yerda koʻring: https://www.w3schools.com/howto/howto_google_fonts.asp


Bir nechta Google shriftlaridan foydalanish uchun shrift nomlarini chiziqli belgi (|) bilan ajrating, shunga o'xshash:



<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Audiowide|Sofiya|Trirong">
<uslub>
h1.a {
   font-family: "Audiowide", sans-serif;
}

h1.b {
   font-family: "Sofiya", sans-serif;
}

h1.c {
   shrift oilasi: "Tirong", serif;
}
</style>
</head>
<tana>

<h1 class="a">Audiowide shrifti</h1>

<h1 class="b">Sofiya shrifti</h1>

<h1 class="c">Trirong shrifti</h1>

</body>
</html>



Eslatma: Bir nechta shriftlarni so'rash veb-sahifalaringizni sekinlashtirishi mumkin! Shuning uchun bundan ehtiyot bo'ling.



Google shriftlarini uslublash

CSS-dan Google shriftlarini quyida ko'rsatilganidek uslublash uchun foydalanish mumkin:


<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Sofia">
<uslub>
tana {
   font-family: "Sofiya", sans-serif;
   shrift o'lchami: 30px;
   matn soyasi: 3px 3px 3px #ababab;
}
</style>
</head>
<tana>

<h1>Sofiya shrifti</h1>
<p>Lorem ipsum dolor sit amet.</p>
<p>123456790</p>

</body>
</html>



Shrift effektlarini yoqish

Google siz foydalanishingiz mumkin bo'lgan turli xil shrift effektlarini ham yoqdi.

Avval Google API-ga effekt=effekt nomini qo'shing, so'ngra boradigan elementga maxsus sinf nomini qo'shing

maxsus effektdan foydalaning. Sinf nomi har doim font-effect- bilan boshlanadi va effekt nomi bilan tugaydi.


"Sofiya" shriftiga olov effektini qo'shish uchun


<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Sofia&effect=fire">
<uslub>
tana {
   font-family: "Sofiya", sans-serif;
   shrift o'lchami: 30px;
}
</style>
</head>
<tana>

<h1 class="font-effect-fire">Yonayotgan Sofiya</h1>
<p class="font-effect-fire">Lorem ipsum dolor sit amet.</p>
<p class="font-effect-fire">123456790</p>

</body>
</html>


Bir nechta shrift effektlarini so'rash uchun effekt nomlarini chiziq belgisi (|) bilan ajrating, shunga o'xshash:



<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Sofia&effect=neon|outline|bo'rtma|

shadow-multiple">
<uslub>
tana {
   font-family: "Sofiya", sans-serif;
   shrift o'lchami: 30px;
}
</style>
</head>
<tana>

<h1 class="font-effect-neon">Neon effekti</h1>
<h1 class="font-effect-outline">Kontakt effekti</h1>
<h1 class="font-effect-emboss">Bo'rtma effekti</h1>
<h1 class="font-effect-shadow-multiple">Bir nechta soya effekti</h1>

</body>
</html>





CSS ajoyib shrift juftligi::

Veb-sayt uchun ajoyib shrift juftligiga ega bo'lish juda muhimdir. Bu dizaynni yaxshilaydi.


Shriftlarni ulash qoidalari

Ajoyib shrift juftlarini yaratish uchun bir necha asosiy qoidalar:
1. To‘ldiruvchi

Bir-birini to'ldiradigan shrift juftlarini topish har doim xavfsizdir.

Ajoyib shrift kombinatsiyasi juda o'xshash yoki juda farq qilmasdan uyg'unlashishi kerak.
2. Shrift Superfamilies dan foydalaning

Shrift superfamily - bu birgalikda yaxshi ishlash uchun mo'ljallangan shriftlar to'plami. Shunday qilib, ichida turli shriftlardan foydalanish

Xuddi shu super oila xavfsiz.

Masalan, Lucida super oilasi quyidagi shriftlarni o'z ichiga oladi: Lucida Sans, Lucida Serif, Lucida

Yozuv mashinkasi Sans, Lucida yozuv mashinasi Serif va Lucida Math.
3. Kontrast - King

Juda o'xshash ikkita shrift ko'pincha ziddiyatli bo'ladi. Biroq, qarama-qarshiliklar, to'g'ri yo'l bilan amalga oshirilgan, olib keladi

har bir shriftda eng yaxshisi.

Misol: Serifni sans serif bilan birlashtirish yaxshi ma'lum kombinatsiyadir.

Kuchli superoila bir xil shriftning serif va sans serif turlarini o'z ichiga oladi (masalan, Lucida va Lucida).

Sans).
4. Faqat bitta xo'jayinni tanlang

Bitta shrift boss bo'lishi kerak. Bu sizning sahifangizdagi shriftlar uchun ierarxiyani o'rnatadi. Bunga erishish mumkin

hajmi, vazni va rangini o'zgartirish orqali.


Quyidagi misolda, Jorjiya shriftlar oilasi boss hisoblanadi, chunki u kattaroq va mos keladi, lekin har xil shriftlar:

<!DOCTYPE html>
<html>
<head>
<uslub>
tana {
   fon rangi: qora;
   font-family: Verdana, sans-serif;
   shrift o'lchami: 16px;
   rang: kulrang;
}

h1 {
   shrift oilasi: Georgia, serif;
   shrift o'lchami: 60px;
   rang: oq;
}
</style>
</head>
<tana>

<h1>Chiroyli Norvegiya</h1>

<p>Norvegiyaning umumiy maydoni 385 252 kvadrat kilometr va aholisi 5 438 657 kishi (2020 yil dekabr).

Norvegiya shimoli-sharqda Shvetsiya, Finlyandiya va Rossiya bilan, janubda esa Skagerrak bilan chegaradosh.

Boshqa tomonda Daniya.</p>

<p>Norvegiyada go'zal tog'lar, muzliklar va ajoyib fyordlar bor. Poytaxt Oslo yashil shahar

joylar va muzeylar. Rangli yog'och uylari bo'lgan Bergen dramatik sayohatlar uchun boshlang'ich nuqtadir

Sognefjord. Norvegiya baliq ovlash, piyoda sayr qilish va chang'i sporti bilan ham mashhur.</p>

</body>
</html>




Ko'pgina brendlar va kontekstlarga mos keladigan mashhur shrift juftliklaridan ba'zilari ko'rsatilgan

quyidagi misollar:


Jorjiya va Verdana

Jorjiya va Verdana klassik kombinatsiyadir. Shuningdek, u veb-xavfsiz shrift standartlariga amal qiladi. "Gruziya" dan foydalaning

sarlavhalar uchun shrift va matn uchun "Verdana" shrifti. Quyidagi misolga qarang:



<!DOCTYPE html>
<html>
<head>
<uslub>
tana {
   font-family: Verdana, sans-serif;
   shrift o'lchami: 16px;
}

h1 {
   shrift oilasi: Georgia, serif;
   shrift o'lchami: 46px;
}
</style>
</head>
<tana>

<h1>Chiroyli Norvegiya</h1>

<p>Norvegiyaning umumiy maydoni 385 252 kvadrat kilometr va aholisi 5 438 657 kishi (2020 yil dekabr).

Norvegiya shimoli-sharqda Shvetsiya, Finlyandiya va Rossiya bilan, janubda esa Skagerrak bilan chegaradosh.

Boshqa tomonda Daniya.</p>

<p>Norvegiyada go'zal tog'lar, muzliklar va ajoyib fyordlar bor. Poytaxt Oslo yashil shahar

joylar va muzeylar. Rangli yog'och uylari bo'lgan Bergen dramatik sayohatlar uchun boshlang'ich nuqtadir

Sognefjord. Norvegiya baliq ovlash, piyoda sayr qilish va chang'i sporti bilan ham mashhur.</p>

</body>
</html>



Helvetica va Garamond

Helvetica va Garamond - bu veb-xavfsiz shriftlardan foydalanadigan yana bir klassik birikma. "Helvetica" shriftidan foydalaning

sarlavhalar va matn uchun "Garamond" shrifti. Quyidagi misolga qarang:


<!DOCTYPE html>
<html>
<head>
<uslub>
tana {
   shrift oilasi: Garamond, serif;
   shrift o'lchami: 16px;
}

h1 {
   font-family: Helvetica, sans-serif;
   shrift o'lchami: 46px;
}
</style>
</head>
<tana>

<h1>Chiroyli Norvegiya</h1>

<p>Norvegiyaning umumiy maydoni 385 252 kvadrat kilometr va aholisi 5 438 657 kishi (2020 yil dekabr).

Norvegiya shimoli-sharqda Shvetsiya, Finlyandiya va Rossiya bilan, janubda esa Skagerrak bilan chegaradosh.

Boshqa tomonda Daniya.</p>

<p>Norvegiyada go'zal tog'lar, muzliklar va ajoyib fyordlar bor. Poytaxt Oslo yashil shahar

joylar va muzeylar. Rangli yog'och uylari bo'lgan Bergen dramatik sayohatlar uchun boshlang'ich nuqtadir

Sognefjord. Norvegiya baliq ovlash, piyoda sayr qilish va chang'i sporti bilan ham mashhur.</p>

</body>
</html>





Mashhur Google shriftlari

Google shriftlari an'anaviy HTML shriftlariga 1000 dan ortiq muqobillarni taqdim etadi. Ulardan veb-saytingizda bepul foydalanish mumkin.


Quyida mos google shriftlari keltirilgan




Merriweather va Open Sans

Sarlavhalar uchun Meriwether shrifti va matn uchun "Ochiq Sans"::


<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Merriweather|Open+Sans">
<uslub>
tana {
   font-family: "Open Sans", sans-serif;
   shrift o'lchami: 16px;
}

h1 {
   shrift oilasi: Merriweather, serif;
   shrift o'lchami: 46px;
}
</style>
</head>
<tana>

<h1>Chiroyli Norvegiya</h1>

<p>Norvegiyaning umumiy maydoni 385 252 kvadrat kilometr va aholisi 5 438 657 kishi (2020 yil dekabr).

Norvegiya shimoli-sharqda Shvetsiya, Finlyandiya va Rossiya bilan, janubda esa Skagerrak bilan chegaradosh.

Boshqa tomonda Daniya.</p>

<p>Norvegiyada go'zal tog'lar, muzliklar va ajoyib fyordlar bor. Poytaxt Oslo yashil shahar

joylar va muzeylar. Rangli yog'och uylari bo'lgan Bergen dramatik sayohatlar uchun boshlang'ich nuqtadir

Sognefjord. Norvegiya baliq ovlash, piyoda sayr qilish va chang'i sporti bilan ham mashhur.</p>

</body>
</html>




Ubuntu va Lora

Sarlavhalar uchun Ubuntu va matn uchun Lora'dan foydalaning. Quyidagi misolga qarang:


<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Ubuntu|Lora">
<uslub>
tana {
   shrift oilasi: Lora, serif;
   shrift o'lchami: 16px;
}

h1 {
   font-family: Ubuntu, sans-serif;
   shrift o'lchami: 46px;
}
</style>
</head>
<tana>

<h1>Chiroyli Norvegiya</h1>

<p>Norvegiyaning umumiy maydoni 385 252 kvadrat kilometr va aholisi 5 438 657 kishi (2020 yil dekabr).

Norvegiya shimoli-sharqda Shvetsiya, Finlyandiya va Rossiya bilan, janubda esa Skagerrak bilan chegaradosh.

Boshqa tomonda Daniya.</p>

<p>Norvegiyada go'zal tog'lar, muzliklar va ajoyib fyordlar bor. Poytaxt Oslo yashil shahar

joylar va muzeylar. Rangli yog'och uylari bo'lgan Bergen dramatik sayohatlar uchun boshlang'ich nuqtadir

Sognefjord. Norvegiya baliq ovlash, piyoda sayr qilish va chang'i sporti bilan ham mashhur.</p>

</body>
</html>



Abril Fatface va Poppins

Sarlavhalar uchun “Abril Fatface” shriftidan, matn uchun esa “Poppins” shriftidan foydalaning. Masalan:


<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Abril+Fatface|Poppins">
<uslub>
tana {
   font-family: Poppins, sans-serif;
   shrift o'lchami: 16px;
}

h1 {
   font-family: 'Abril Fatface', serif;
   shrift o'lchami: 46px;
}
</style>
</head>
<tana>

<h1>Chiroyli Norvegiya</h1>

<p>Norvegiyaning umumiy maydoni 385 252 kvadrat kilometr va aholisi 5 438 657 kishi (2020 yil dekabr).

Norvegiya shimoli-sharqda Shvetsiya, Finlyandiya va Rossiya bilan, janubda esa Skagerrak bilan chegaradosh.

Boshqa tomonda Daniya.</p>

<p>Norvegiyada go'zal tog'lar, muzliklar va ajoyib fyordlar bor. Poytaxt Oslo yashil shahar

joylar va muzeylar. Rangli yog'och uylari bo'lgan Bergen dramatik sayohatlar uchun boshlang'ich nuqtadir

Sognefjord. Norvegiya baliq ovlash, piyoda sayr qilish va chang'i sporti bilan ham mashhur.</p>

</body>
</html>

Cinzel va fauna One

Sarlavhalar uchun "Cinzel" shrifti va matn uchun "Fauna One" shriftidan foydalaning.



<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Cinzel|Fauna+One">
<uslub>
tana {
   font-family: 'Fauna One', serif;
   shrift o'lchami: 16px;
}

h1 {
   shrift oilasi: Cinzel, serif;
   shrift o'lchami: 46px;
}
</style>
</head>
<tana>

<h1>Chiroyli Norvegiya</h1>

<p>Norvegiyaning umumiy maydoni 385 252 kvadrat kilometr va aholisi 5 438 657 kishi (2020 yil dekabr).

Norvegiya shimoli-sharqda Shvetsiya, Finlyandiya va Rossiya bilan, janubda esa Skagerrak bilan chegaradosh.

Boshqa tomonda Daniya.</p>

<p>Norvegiyada go'zal tog'lar, muzliklar va ajoyib fyordlar bor. Poytaxt Oslo yashil shahar

joylar va muzeylar. Rangli yog'och uylari bo'lgan Bergen dramatik sayohatlar uchun boshlang'ich nuqtadir

Sognefjord. Norvegiya baliq ovlash, piyoda sayr qilish va chang'i sporti bilan ham mashhur.</p>

</body>
</html>



Fjalla One va Libre Baskerville


Sarlavhalar uchun "Fjalla One" shrifti va matn uchun "Libre Baskerville" shrifti ishlatilishi kerak.


<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Fjalla+One|Libre+Baskerville">
<uslub>
tana {
   font-family: 'Libre Baskerville', serif;
   shrift o'lchami: 16px;
}

h1 {
   font-family: 'Fjalla One', sans-serif;
   shrift o'lchami: 46px;
}
</style>
</head>
<tana>

<h1>Chiroyli Norvegiya</h1>

<p>Norvegiyaning umumiy maydoni 385 252 kvadrat kilometr va aholisi 5 438 657 kishi (2020 yil dekabr).

Norvegiya shimoli-sharqda Shvetsiya, Finlyandiya va Rossiya bilan, janubda esa Skagerrak bilan chegaradosh.

Boshqa tomonda Daniya.</p>

<p>Norvegiyada go'zal tog'lar, muzliklar va ajoyib fyordlar bor. Poytaxt Oslo yashil shahar

joylar va muzeylar. Rangli yog'och uylari bo'lgan Bergen dramatik sayohatlar uchun boshlang'ich nuqtadir

Sognefjord. Norvegiya baliq ovlash, piyoda sayr qilish va chang'i sporti bilan ham mashhur.</p>

</body>
</html>




Space Mono va Muli

Sarlavhalar uchun "Space Mono" shriftidan foydalaning va matn uchun "Muli". Quyidagi misolga qarang:



<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Space+Mono|Muli">
<uslub>
tana {
   font-family: Muli, sans-serif;
   shrift o'lchami: 16px;
}

h1 {
   shrift oilasi: "Space Mono", monospace;
   shrift o'lchami: 46px;
}
</style>
</head>
<tana>

<h1>Chiroyli Norvegiya</h1>

<p>Norvegiyaning umumiy maydoni 385 252 kvadrat kilometr va aholisi 5 438 657 kishi (2020 yil dekabr).

Norvegiya shimoli-sharqda Shvetsiya, Finlyandiya va Rossiya bilan, janubda esa Skagerrak bilan chegaradosh.

Boshqa tomonda Daniya.</p>

<p>Norvegiyada go'zal tog'lar, muzliklar va ajoyib fyordlar bor. Poytaxt Oslo yashil shahar

joylar va muzeylar. Rangli yog'och uylari bo'lgan Bergen dramatik sayohatlar uchun boshlang'ich nuqtadir

Sognefjord. Norvegiya baliq ovlash, piyoda sayr qilish va chang'i sporti bilan ham mashhur.</p>

</body>
</html>



Spektral va Rubik

Sarlavhalar uchun Spektral shriftdan va matn uchun "Rubik" dan foydalaning:


<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Spectral|Rubik">
<uslub>
tana {
   font-family: Rubik, sans-serif;
   shrift o'lchami: 16px;
}

h1 {
   shrift oilasi: Spektral, serif;
   shrift o'lchami: 46px;
}
</style>
</head>
<tana>

<h1>Chiroyli Norvegiya</h1>

<p>Norvegiyaning umumiy maydoni 385 252 kvadrat kilometr va aholisi 5 438 657 kishi (2020 yil dekabr).

Norvegiya shimoli-sharqda Shvetsiya, Finlyandiya va Rossiya bilan, janubda esa Skagerrak bilan chegaradosh.

Boshqa tomonda Daniya.</p>

<p>Norvegiyada go'zal tog'lar, muzliklar va ajoyib fyordlar bor. Poytaxt Oslo yashil shahar

joylar va muzeylar. Rangli yog'och uylari bo'lgan Bergen dramatik sayohatlar uchun boshlang'ich nuqtadir

Sognefjord. Norvegiya baliq ovlash, piyoda sayr qilish va chang'i sporti bilan ham mashhur.</p>

</body>
</html>





Osvald va Noto Sans

Sarlavhalar uchun "Oswald" shrifti va matn uchun "Noto Sans" dan foydalaning. Quyidagi misolga qarang:


<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Oswald|Noto+Sans">
<uslub>
tana {
   font-family: "Noto Sans", sans-serif;
   shrift o'lchami: 16px;
}

h1 {
   font-family: Oswald, sans-serif;
   shrift o'lchami: 46px;
}
</style>
</head>
<tana>

<h1>Chiroyli Norvegiya</h1>

<p>Norvegiyaning umumiy maydoni 385 252 kvadrat kilometr va aholisi 5 438 657 kishi (2020 yil dekabr).

Norvegiya shimoli-sharqda Shvetsiya, Finlyandiya va Rossiya bilan, janubda esa Skagerrak bilan chegaradosh.

Boshqa tomonda Daniya.</p>

<p>Norvegiyada go'zal tog'lar, muzliklar va ajoyib fyordlar bor. Poytaxt Oslo yashil shahar

joylar va muzeylar. Rangli yog'och uylari bo'lgan Bergen dramatik sayohatlar uchun boshlang'ich nuqtadir

Sognefjord. Norvegiya baliq ovlash, piyoda sayr qilish va chang'i sporti bilan ham mashhur.</p>

</body>
</html>




CSS shrift xususiyati::


Kodni qisqartirish uchun barcha individual shrift xususiyatlarini bitta xususiyatda ko'rsatish ham mumkin.

Shrift xususiyati stenografiya xususiyatidir:

     shrift uslubi
     shrift-variant
     shrift og'irligi
     shrift o'lchami/satr balandligi
     shrift oilasi

Quyida ushbu ilovaning namunasini ko'ring:

<!DOCTYPE html>
<html>
<head>
<uslub>
p.a {
   shrift: 20px Arial, sans-serif;
}

p.b {
   shrift: kursiv qalin 12px/30px Georgia, serif;
}
</style>
</head>
<tana>

<h1>Shrift xususiyati</h1>

<p class="a">Bu paragraf. Shrift o‘lchami 20 pikselga o‘rnatilgan va shriftlar oilasi Arial.</p>

<p class="b">Bu paragraf. Shrift kursiv va qalin qilib o'rnatiladi, shrift o'lchami 12 pikselga o'rnatiladi,

satr balandligi 30 piksel qilib belgilangan, shrift oilasi esa Georgia.</p>

</body>
</html>


Eslatma: Shrift o'lchami va shrift oilasi qiymatlari talab qilinadi. Agar boshqa qiymatlardan biri etishmayotgan bo'lsa, ularning

standart qiymat ishlatiladi.

<kbd>qaytish</kbd>[Mundarijaga qaytish](#homepage)
  - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -


## CSS piktogrammalari

CSS-da HTML sahifasiga piktogramma qo'shishni osonlashtiradigan piktogramma kutubxonasi mavjud.


Qanday qilib piktogramma qo'shish kerak

Belgini oddiygina HTML sahifasiga Font Awesome kabi piktogramma kutubxonasi bilan qo'shish mumkin. Siz shunchaki nomini qo'shasiz

belgilangan ikonka sinfini har qanday ichki HTML elementiga (masalan, <i> yoki <span>). Olingan piktogrammalar kengaytirilishi mumkin

o'lchamini, rangini, soyasini va hokazolarni o'zgartirish uchun CSS uslublar vositalaridan foydalanib sozlashingiz mumkin bo'lgan vektorlar

piktogramma.

 

Shriftning ajoyib piktogrammalari

fontawesome.com saytiga o‘ting va tizimga kiring. HTML sahifasining <head> bo‘limiga qo‘shilishi kerak bo‘lgan kod shunday bo‘lishi mumkin.

quyida ko'rsatilganidek, ushbu veb-saytda olingan:

<script src="https://kit.fontawesome.com/yourcode.js" crossorigin="anonymous"></script>


Font-awesome-ni qanday boshlash haqida ko'proq bilish uchun bu yerga qarang:

https://www.w3schools.com/icons/fontawesome5_intro.asp

Ajoyib shriftdan foydalanish uchun sizga yuklab olish yoki o'rnatish kerak emas


Awesome shriftida mavjud bo'lgan barcha piktogrammalarga havolalarning to'liq ro'yxatini bu erda ko'rish mumkin:

https://www.w3schools.com/icons/icons_reference.asp


Awesome shriftini amalga oshirish misoli quyida ko'rsatilgan:


<!DOCTYPE html>
<html>
<head>
<title>Ajoyib shrift piktogrammalari</title>
<meta name="viewport" content="width=device-width, initial-scale=1">
<script src="https://kit.fontawesome.com/a076d05399.js" crossorigin="anonymous"></script>
<!--O'z kodingizni fontawesome.com--> saytidan oling
</head>
<tana>

<p>Ajoyib shrift belgilari:</p>
<i class="fas fa-cloud"></i>
<i class="fas fa-heart"></i>
<i class="fas fa-car"></i>
<i class="fas fa-fayl"></i>
<i class="fas fa-bars"></i>

<p>Uslubli shrift Ajoyib piktogramma (hajmi va rangi):</p>
<i class="fas fa-cloud" style="font-size:24px;"></i>
<i class="fas fa-cloud" style="font-size:36px;"></i>
<i class="fas fa-cloud" style="font-size:48px;color:red;"></i>
<i class="fas fa-cloud" style="font-size:60px;color:lightblue;"></i>

</body>
</html>




Bootstrap piktogrammalari

Bootstrap glifikalaridan foydalanish uchun HTML sahifangizning <head> boʻlimiga quyidagi qatorni qoʻshing:

<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css">

Eslatma: Yuklab olish yoki o'rnatish shart emas!


Quyidagi Boostrap belgisini amalga oshirish misoliga qarang:

<!DOCTYPE html>
<html>
<head>
<title>Bootstrap piktogrammalari</title>
<meta name="viewport" content="width=device-width, initial-scale=1">
<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css">
</head>
<body class="container">

<p>Ba'zi Bootstrap piktogrammalari:</p>
<i class="glyphicon glyphicon-cloud"></i>
<i class="glyphicon glyphicon-remove"></i>
<i class="glyphicon glyphicon-user"></i>
<i class="glyphicon glyphicon-convelope"></i>
<i class="glyphicon glyphicon-thumbs-up"></i>
<br><br>

<p>Uslubli Bootstrap piktogrammalari (hajmi va rangi):</p>
<i class="glyphicon glyphicon-cloud" style="font-size:24px;"></i>
<i class="glyphicon glyphicon-cloud" style="font-size:36px;"></i>
<i class="glyphicon glyphicon-cloud" style="font-size:48px;color:red;"></i>
<i class="glyphicon glyphicon-cloud" style="font-size:60px;color:lightblue;"></i>

</body>
</html>



Google ikonkalari

Google piktogrammalaridan foydalanish uchun HTML sahifangizning <head> boʻlimiga quyidagi qatorni qoʻshing:

<link rel="stylesheet" href="https://fonts.googleapis.com/icon?family=Material+Icons">

Eslatma: Yuklab olish yoki o'rnatish shart emas!

Quyidagi google belgisini amalga oshirish misoliga qarang:
<!DOCTYPE html>
<html>
<head>
<title>Google ikonkalari</title>
<meta name="viewport" content="width=device-width, initial-scale=1">
<link rel="stylesheet" href="https://fonts.googleapis.com/icon?family=Material+Icons">
</head>
<tana>

<p>Ba'zi Google piktogrammalari:</p>
<i class="material-icons">bulut</i>
<i class="material-icons">sevimli</i>
<i class="material-icons">ilova</i>
<i class="material-icons">kompyuter</i>
<i class="material-icons">trafik</i>
<br><br>

<p>Uslubli Google piktogrammalari (hajmi va rangi):</p>
<i class="material-icons" style="font-size:24px;">bulut</i>
<i class="material-icons" style="font-size:36px;">bulut</i>
<i class="material-icons" style="font-size:48px;color:red;">bulut</i>
<i class="material-icons" style="font-size:60px;color:lightblue;">bulut</i>

</body>
</html>


<kbd>qaytish</kbd>[Mundarijaga qaytish](#homepage)


--------

## CSS piktogrammalari

CSS-da HTML sahifasiga piktogramma qo'shishni osonlashtiradigan piktogramma kutubxonasi mavjud.


Qanday qilib piktogramma qo'shish kerak

Belgini oddiygina HTML sahifasiga Font Awesome kabi piktogramma kutubxonasi bilan qo'shish mumkin. Siz shunchaki nomini qo'shasiz

belgilangan ikonka sinfini har qanday ichki HTML elementiga (masalan, <i> yoki <span>). Olingan piktogrammalar kengaytirilishi mumkin

o'lchamini, rangini, soyasini va hokazolarni o'zgartirish uchun CSS uslublar vositalaridan foydalanib sozlashingiz mumkin bo'lgan vektorlar

piktogramma.

 

Shriftning ajoyib piktogrammalari

fontawesome.com saytiga o‘ting va tizimga kiring. HTML sahifasining <head> bo‘limiga qo‘shilishi kerak bo‘lgan kod shunday bo‘lishi mumkin.

quyida ko'rsatilganidek, ushbu veb-saytda olingan:

<script src="https://kit.fontawesome.com/yourcode.js" crossorigin="anonymous"></script>


Font-awesome-ni qanday boshlash haqida ko'proq bilish uchun bu yerga qarang:

https://www.w3schools.com/icons/fontawesome5_intro.asp

Ajoyib shriftdan foydalanish uchun sizga yuklab olish yoki o'rnatish kerak emas


Awesome shriftida mavjud bo'lgan barcha piktogrammalarga havolalarning to'liq ro'yxatini bu erda ko'rish mumkin:

https://www.w3schools.com/icons/icons_reference.asp


Awesome shriftini amalga oshirish misoli quyida ko'rsatilgan:


<!DOCTYPE html>
<html>
<head>
<title>Ajoyib shrift piktogrammalari</title>
<meta name="viewport" content="width=device-width, initial-scale=1">
<script src="https://kit.fontawesome.com/a076d05399.js" crossorigin="anonymous"></script>
<!--O'z kodingizni fontawesome.com--> saytidan oling
</head>
<tana>

<p>Ajoyib shrift belgilari:</p>
<i class="fas fa-cloud"></i>
<i class="fas fa-heart"></i>
<i class="fas fa-car"></i>
<i class="fas fa-fayl"></i>
<i class="fas fa-bars"></i>

<p>Uslubli shrift Ajoyib piktogramma (hajmi va rangi):</p>
<i class="fas fa-cloud" style="font-size:24px;"></i>
<i class="fas fa-cloud" style="font-size:36px;"></i>
<i class="fas fa-cloud" style="font-size:48px;color:red;"></i>
<i class="fas fa-cloud" style="font-size:60px;color:lightblue;"></i>

</body>
</html>




Bootstrap piktogrammalari

Bootstrap glifikalaridan foydalanish uchun HTML sahifangizning <head> boʻlimiga quyidagi qatorni qoʻshing:

<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css">

Eslatma: Yuklab olish yoki o'rnatish shart emas!


Quyidagi Boostrap belgisini amalga oshirish misoliga qarang:

<!DOCTYPE html>
<html>
<head>
<title>Bootstrap piktogrammalari</title>
<meta name="viewport" content="width=device-width, initial-scale=1">
<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css">
</head>
<body class="container">

<p>Ba'zi Bootstrap piktogrammalari:</p>
<i class="glyphicon glyphicon-cloud"></i>
<i class="glyphicon glyphicon-remove"></i>
<i class="glyphicon glyphicon-user"></i>
<i class="glyphicon glyphicon-convelope"></i>
<i class="glyphicon glyphicon-thumbs-up"></i>
<br><br>

<p>Uslubli Bootstrap piktogrammalari (hajmi va rangi):</p>
<i class="glyphicon glyphicon-cloud" style="font-size:24px;"></i>
<i class="glyphicon glyphicon-cloud" style="font-size:36px;"></i>
<i class="glyphicon glyphicon-cloud" style="font-size:48px;color:red;"></i>
<i class="glyphicon glyphicon-cloud" style="font-size:60px;color:lightblue;"></i>

</body>
</html>



Google ikonkalari

Google piktogrammalaridan foydalanish uchun HTML sahifangizning <head> boʻlimiga quyidagi qatorni qoʻshing:

<link rel="stylesheet" href="https://fonts.googleapis.com/icon?family=Material+Icons">

Eslatma: Yuklab olish yoki o'rnatish shart emas!

Quyidagi google belgisini amalga oshirish misoliga qarang:


<!DOCTYPE html>
<html>
<head>
<title>Google ikonkalari</title>
<meta name="viewport" content="width=device-width, initial-scale=1">
<link rel="stylesheet" href="https://fonts.googleapis.com/icon?family=Material+Icons">
</head>
<tana>

<p>Ba'zi Google piktogrammalari:</p>
<i class="material-icons">bulut</i>
<i class="material-icons">sevimli</i>
<i class="material-icons">ilova</i>
<i class="material-icons">kompyuter</i>
<i class="material-icons">trafik</i>
<br><br>

<p>Uslubli Google piktogrammalari (hajmi va rangi):</p>
<i class="material-icons" style="font-size:24px;">bulut</i>
<i class="material-icons" style="font-size:36px;">bulut</i>
<i class="material-icons" style="font-size:48px;color:red;">bulut</i>
<i class="material-icons" style="font-size:60px;color:lightblue;">bulut</i>

</body>
</html>


<kbd>qaytish</kbd>[Mundarijaga qaytish](#homepage)



---------

## HTML JADVALLARI
```
<table> tegi HTML jadvalini aniqladi.
<tr> jadval qatorini belgilaydi
<th> jadval sarlavhasini belgilaydi. Odatiy bo'lib qalin va markazlashtirilgan.
<td> jadval ma'lumotlari/hujayralarini belgilaydi.. Odatiy bo'lib, odatiy va chapga tekislangan. Ular matn, rasmlar, ro'yxatlar, boshqa jadvallar va boshqalar uchun ma'lumotlar konteynerlari.
```
* Oddiy HTML jadvali
```
  <table style="width:100%">
   <tr>
     <th>Ism</th>
     <th>Familiya</th>
     <th>Yosh</th>
   </tr>
   <tr>
     <td>Jill</td>
     <td>Smit</td>
     <td>50</td>
   </tr>
   <tr>
     <td>Havo</td>
     <td>Jekson</td>
     <td>94</td>
   </tr>
</jadval>
```
** Jadval quyidagicha ko'rinadi::
Ism familiyasi Yosh
Jill Smit 50
Momo Jekson 94
Jon Dou 80


* HTML jadvaliga chegara qo'shing:::
```
jadval, th, td {
   chegara: 1px qattiq qora;
}
```

** Yigʻilgan jadval chegarasi:: Barcha chegaralarni bir chegaraga yigʻish uchun chegarani yigʻish xususiyatini qoʻshing.
```
jadval, th, td {
   chegara: 1px qattiq qora;
   chegara-burilish: qulash;
}
```
** Add Cell Padding::: Hujayra va uning chegaralari orasidagi bo'shliqni belgilaydi. Agar ko'rsatilmagan bo'lsa, jadval kataklari to'ldirishsiz ko'rsatiladi. To'ldirishni o'rnatish uchun CSS padding xususiyatidan foydalaning:

```
th, td {
   to'ldirish: 15px;
}
```
** Chapga tekislangan sarlavhalar::Jadval sarlavhalari sukut bo'yicha qalin va markazlashtirilgan.

Jadval sarlavhalarini chapga tekislash uchun CSS matnni tekislash xususiyatidan foydalaning.
```
n {
   matnni tekislash: chapga;
}
```

** Chegara oralig‘ini qo‘shish:: Hujayralar orasidagi bo‘shliqni belgilaydi. CSS chegarasi oralig'i xususiyatidan foydalaning. Chegara oralig'i chegaralari yiqilgan jadvalga ta'sir qilmaydi
```
stol {
   chegara oralig'i: 5px;
}
```
** Ko'p ustunlarni o'z ichiga olgan hujayralar:: colspan atributidan foydalaning
```
  <table style="width:100%">
   <tr>
     <th>Ism</th>
     <th colspan="2">Telefon</th>
   </tr>
   <tr>
     <td>Bill Geyts</td>
     <td>55577854</td>
     <td>55577855</td>
   </tr>
</jadval>
```

** Bu shunday ko'rinadi: Telefon nomi
Bill Geyts 55577854 55577855


** Ko'p qatorli katakchani yarating:: rowspan dan foydalaning. rowspan=2 ikki qatorli tarkibni o'z ichiga olishi uchun ikkita satr <tr> elementini belgilashingizni bildiradi.

```
  <table style="width:100%">
   <tr>
     <th>Ism:</th>
     <td>Bill Geyts</td>
   </tr>
   <tr>
     <th rowspan="2">Telefon:</th>
     <td>55577854</td>
   </tr>
   <tr>
     <td>55577855</td>
   </tr>
</jadval>
```
** Jadvalga sarlavha qo'shing:: jadval tegidan keyin darhol kiritilgan <caption> tegidan foydalaning

```
  <table style="width:100%">
   <caption>Oylik tejash</caption>
   <tr>
     <th>Oy</th>
     <th>Tejamkorlik</th>
   </tr>
   <tr>
     <td>yanvar</td>
     <td>$100</td>
   </tr>
   <tr>
     <td>Fevral</td>
     <td>50$</td>
   </tr>
</jadval>
```
** Bitta jadval uchun maxsus uslubni belgilang. Jadvalga identifikator qo'shing va keyingi maxsus uslubni belgilang
```
<jadval id="t01">
   <tr>
     <th>Ism</th>
     <th>Familiya</th>
     <th>Yosh</th>
   </tr>
   <tr>
     <td>Havo</td>
     <td>Jekson</td>
     <td>94</td>
   </tr>
</jadval>


#t01 {
   kengligi: 100%;
   fon rangi: #f1f1c1;
}

```

siz qo'shimcha uslublarni qo'shishingiz mumkin:
```
#t01 tr:nth-child(hatto) {
   fon rangi: #eee;
}
#t01 tr:nth-child(toq) {
   fon rangi: #fff;
}
#t01 {
   rang: oq;
   fon rangi: qora;
}
```


* BOBLAR XULOSASI _HTML BOB XULOSALARI
    Jadvalni aniqlash uchun HTML ```<table>``` elementidan foydalaning
    Jadval qatorini aniqlash uchun HTML ``<tr>`` elementidan foydalaning
    Jadval ma'lumotlarini aniqlash uchun HTML ``<td>`` elementidan foydalaning
    Jadval sarlavhasini aniqlash uchun HTML ```<th>``` elementidan foydalaning
    Jadval sarlavhasini aniqlash uchun HTML ```<caption>``` elementidan foydalaning
    Chegarani aniqlash uchun CSS border xususiyatidan foydalaning
    Hujayra chegaralarini yopish uchun CSS border-collapse xususiyatidan foydalaning
    Hujayralarga toʻldirish qoʻshish uchun CSS padding xususiyatidan foydalaning
    Hujayra matnini tekislash uchun CSS text-align xususiyatidan foydalaning
    Hujayralar orasidagi masofani o'rnatish uchun CSS chegarasi oralig'i xususiyatidan foydalaning
    Hujayrani ko'p ustunli qilish uchun colspan atributidan foydalaning
    Hujayrani ko'p qatorli qilish uchun rowspan atributidan foydalaning
    Bitta jadvalni yagona aniqlash uchun id atributidan foydalaning


<kbd>qaytish</kbd>[Mundarijaga qaytish](#homepage)

--------

# HTML RO'YXATLARI

** tartibsiz roʻyxatda oʻqlar bor
** tartiblangan ro'yxatlar raqamlash yoki qandaydir ketma-ketlik belgilariga ega

* Tartibsiz html roʻyxati:: har biri ```<ul>``` tegi bilan boshlanadi va har bir ro`yxat elementi ```<li>``` tegi bilan boshlanadi
sukut bo'yicha, ro'yxat elementi o'q sifatida kichik qora doiralar bilan belgilanadi.
```
  <ul>
   <li>Qahva</li>
   <li>Choy</li>
   <li>Sut</li>
</ul>
```

<kbd>qaytish</kbd>[Mundarijaga qaytish](#homepage)

## Buyurtma berildi

* Tartiblangan HTML ro'yxati: <ol> tomonidan belgilanadi va har bir ro'yxat elementi <li> tegi bilan belgilanadi. Sukut bo'yicha ro'yxat elementlarini belgilash uchun raqamlar usd hisoblanadi.

```
  <ol>
   <li>Qahva</li>
   <li>Choy</li>
   <li>Sut</li>
</ol>
```

HTML tavsifi roʻyxatlari:: Roʻyxatdagi har bir atama tavsifi bilan atamalar roʻyxati. tavsif ro'yxati ```<dl>``` tegi bilan belgilanadi va har bir tavsif atamasi (nomi) ```<dt>``` xyz bilan belgilanadi va har bir tavsif ro`yxati atamasi ```< bilan belgilanadi. dd>```:
```
  <dl>
   <dt>Qahva</dt>
   <dd>- qora issiq ichimlik</dd>
   <dt>Sut</dt>
   <dd>- oq sovuq ichimlik</dd>
</dl>
```

* HTML ro'yxati teglari xulosasi
Teg tavsifi
```<ul>``` Tartibsiz ro`yxatni belgilaydi
```<ol>``` Tartiblangan ro`yxatni belgilaydi
```<li>``` Ro`yxat elementini belgilaydi
```<dl>``` Tavsif ro`yxatini belgilaydi
```<dt>``` Tavsiflar ro`yxatidagi atamani belgilaydi
```<dd>``` Tavsiflar ro`yxatidagi atamani tavsiflaydi

<kbd>qaytish</kbd>[Mundarijaga qaytish](#homepage)

## Buyurtmasiz
**HTML tartibsiz roʻyxatlar roʻyxati belgisi

Ro'yxat markerini tanlash uchun ro'yxat ob'ektlari bozori uslubini aniqlash uchun CSS list-style-type xususiyatidan foydalaning.

Qiymat tavsifi
disk Ro'yxat elementi markerini markerga o'rnatadi (standart)
doira Ro‘yxat elementi markerini aylanaga o‘rnatadi
kvadrat Ro'yxat elementi markerini kvadratga o'rnatadi
yo'q Ro'yxat elementlari belgilanmaydi

* Disk (to'ldirilgan doira)
```
<ul style="list-style-type:disc;">
   <li>Qahva</li>
   <li>Choy</li>
   <li>Sut</li>
</ul>
```

* Ochiq (to'ldirilmagan doira)
```
  <ul style="list-style-type:circle;">
   <li>Qahva</li>
   <li>Choy</li>
   <li>Sut</li>
</ul>
```

** Kvadrat (qora bilan to'ldirilgan)
```
  <ul style="list-style-type:square;">
   <li>Qahva</li>
   <li>Choy</li>
   <li>Sut</li>
</ul>
```

** Yo'q (marker yo'q)
```
  <ul style="list-style-type:none;">
   <li>Qahva</li>
   <li>Choy</li>
   <li>Sut</li>
</ul>
```

** Ichki HTML ro'yxati: ro'yxat ichidagi ro'yxat
```
  <ul>
   <li>Qahva</li>
   <li>Choy
     <ul>
       <li>Qora choy</li>
       <li>Yashil choy</li>
     </ul>
   </li>
   <li>Sut</li>
</ul>
```
** Roʻyxat elementi (```<li>```) yangi roʻyxatni va boshqa HTML elementlarini, masalan, rasmlar va havolalarni va hokazolarni oʻz ichiga olishi mumkin.

* CSS bilan gorizontal ro'yxat

Navigatsiya menyusini yaratish uchun siz roʻyxatlarni gorizontal tarzda belgilashingiz mumkin.

** Navigatsiya menyusini yaratish uchun roʻyxatni gorizontal tarzda oʻzgartirishingiz mumkin. Chapdagi float uslubi navigatsiya menyusini chapga o'rnatadi
```
  <!DOCTYPE html>
<html>
<head>
<uslub>
ul {
   ro'yxat uslubi turi: yo'q;
   chegara: 0;
   to'ldirish: 0;
   toshib ketish: yashirin;
   fon rangi: #333333;
}

li {
   float: chap;
}

li a {
   displey: blok;
   rang: oq;
   matnni tekislash: markaz;
   to'ldirish: 16px;
   matn-bezak: yo'q;
}

li a: suring {
   fon rangi: #111111;
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
```
** Bo'lim xulosasi
Bo'lim xulosasi

  Tartibsiz roʻyxatni aniqlash uchun HTML ```<ul>``` elementidan foydalaning
  Ro'yxat elementi markerini aniqlash uchun CSS list-style-type xususiyatidan foydalaning
  Roʻyxat elementini aniqlash uchun HTML ```<li>``` elementidan foydalaning
  Ro'yxatlarni joylashtirish mumkin
  Ro'yxat elementlari boshqa HTML elementlarini o'z ichiga olishi mumkin
  Roʻyxatni gorizontal koʻrsatish uchun CSS float:left xususiyatidan foydalaning

** HTML ro'yxati teglari xulosasi
```
HTML ro'yxati teglari
Teg tavsifi
<ul> Tartibsiz ro'yxatni belgilaydi
<ol> Tartiblangan ro'yxatni belgilaydi
<li> Ro'yxat elementini belgilaydi
<dl> Tavsif ro'yxatini belgilaydi
<dt> Ta'riflar ro'yxatidagi atamani belgilaydi
<dd> Ta'riflar ro'yxatidagi atamani tavsiflaydi
```
<kbd>qaytish</kbd>[Mundarijaga qaytish](#homepage)

HTML tartibi ro'yxati::
```<ol>``` teg raqamli yoki alifbo tartibida bo`lishi mumkin bo`lgan tartiblangan ro`yxatni belgilaydi.
Ro'yxat sukut bo'yicha raqamlar bilan belgilanadi

** Tartiblangan HTML ro'yxati - Type atributi
<ol> tegining type atributi yordamida siz ro'yxat elementi markerining turini belgilashingiz mumkin

```
Turi Tavsif
type="1" Ro'yxat elementlari raqamlar bilan raqamlanadi (standart)
type="A" Ro'yxat elementlari bosh harflar bilan raqamlanadi
type="a" Ro'yxat elementlari kichik harflar bilan raqamlanadi
type="I" Ro'yxat elementlari katta rim raqamlari bilan raqamlanadi
type="i" Ro'yxat elementlari kichik rim raqamlari bilan raqamlanadi
```


* Raqamlar
```
  <ol type="1">
   <li>Qahva</li>
   <li>Choy</li>
   <li>Sut</li>
</ol>
```


* Katta harflar:
```
  <ol type="A">
   <li>Qahva</li>
   <li>Choy</li>
   <li>Sut</li>
</ol>
```

* Kichik harflar:
```
  <ol type="a">
   <li>Qahva</li>
   <li>Choy</li>
   <li>Sut</li>
</ol>
```

* Katta Rim raqamlari:
```
<ol type="I">
   <li>Qahva</li>
   <li>Choy</li>
   <li>Sut</li>
</ol>
```
* Kichik Rim raqamlari:
```
<ol type="I">
   <li>Qahva</li>
   <li>Choy</li>
   <li>Sut</li>
</ol>
```
* Boshqaruv ro'yxatini hisoblash: 50 dan boshqa ma'lum bir raqamdan boshqariladigan ro'yxatni hisoblashni boshlash imkonini beradi
```
<ol start="50">
   <li>Qahva</li>
   <li>Choy</li>
   <li>Sut</li>
</ol>
```
<kbd>qaytish</kbd>[Mundarijaga qaytish](#homepage)

## BOSHQA
* Ichki HTML ro'yxatlari (ro'yxat ichidagi ro'yxat)
```
<ol>
   <li>Qahva</li>
   <li>Choy
     <ol>
       <li>Qora choy</li>
       <li>Yashil choy</li>
     </ol>
   </li>
   <li>Sut</li>
</ol>
```
* Bo'lim xulosasi:

Tartiblangan roʻyxatni aniqlash uchun HTML ```<ol>``` elementidan foydalaning
Raqamlash turini aniqlash uchun HTML turi atributidan foydalaning
Roʻyxat elementini aniqlash uchun HTML ```<li>``` elementidan foydalaning
Ro'yxatlarni joylashtirish mumkin
Ro'yxat elementlari boshqa HTML elementlarini o'z ichiga olishi mumkin

HTML ro'yxati teglari
```
<ul> Tartibsiz ro'yxatni belgilaydi
<ol> Tartiblangan ro'yxatni belgilaydi
<li> Ro'yxat elementini belgilaydi
<dl> Tavsif ro'yxatini belgilaydi
<dt> Ta'riflar ro'yxatidagi atamani belgilaydi
<dd> Ta'riflar ro'yxatidagi atamani tavsiflaydi
```

* Tavsif ro'yxatlari: Har bir atama tavsifi bilan atamalar ro'yxati.
```<dl>``` tegi ro`yxatni, ```<dt>``` atamani (ismni) belgilaydi va ```<dd>``` tegi har bir atamani tavsiflaydi:
```
<dl>
   <dt>Qahva</dt>
   <dd>- qora issiq ichimlik</dd>
   <dt>Sut</dt>
   <dd>- oq sovuq ichimlik</dd>
</dl>
```
* Tavsif ro'yxatining qisqacha mazmuni:
Ta'riflar ro'yxatini aniqlash uchun HTML ```<dl>``` elementidan foydalaning
Ta'rif atamasini aniqlash uchun HTML ```<dt>``` elementidan foydalaning
Ta'riflar ro'yxatidagi atamani tavsiflash uchun HTML ```<dd>``` elementidan foydalaning

HTML ro'yxati teglari
```
**Teg tavsifi
<ul> Tartibsiz ro'yxatni belgilaydi
<ol> Tartiblangan ro'yxatni belgilaydi
<li> Ro'yxat elementini belgilaydi
<dl> Tavsif ro'yxatini belgilaydi
<dt> Ta'riflar ro'yxatidagi atamani belgilaydi
<dd> Ta'riflar ro'yxatidagi atamani tavsiflaydi
```
<kbd>qaytish</kbd>[Mundarijaga qaytish](#homepage)