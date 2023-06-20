## HTML MEDIA
PART 5: HTML MEDIA

HTML Multimedia:

Multimedia on the web is sound, music, videos, movies, and animations.

Multimedia files have formats and different extensions like: .wav, .mp3, .mp4, .mpg, .wmv, and .avi.

* Videoformats

Format 	File 	Description
MPEG 	.mpg
.mpeg 	MPEG. Developed by the Moving Pictures Expert Group. The first popular video format on the web. Not supported anymore in HTML.


AVI 	.avi 	AVI (Audio Video Interleave). Developed by Microsoft. Commonly used in video cameras and TV hardware. Plays well on Windows computers, but not in web browsers.

WMV 	.wmv 	WMV (Windows Media Video). Developed by Microsoft. Commonly used in video cameras and TV hardware. Plays well on Windows computers, but not in web browsers.


QuickTime 	.mov 	QuickTime. Developed by Apple. Commonly used in video cameras and TV hardware. Plays well on Apple computers, but not in web browsers.


RealVideo 	.rm
.ram 	RealVideo. Developed by Real Media to allow video streaming with low bandwidths. Does not play in web browsers.


Flash 	.swf
.flv 	Flash. Developed by Macromedia. Often requires an extra component (plug-in) to play in web browsers.


Ogg 	.ogg 	Theora Ogg. Developed by the Xiph.Org Foundation. Supported by HTML.


WebM 	.webm 	WebM. Developed by Mozilla, Opera, Adobe, and Google. Supported by HTML.

MPEG-4
or MP4 	.mp4 	MP4. Developed by the Moving Pictures Expert Group. Commonly used in video cameras and TV hardware. Supported by all browsers and  recommended by YouTube.  


Note: Only MP4, WebM, and Ogg video are supported by the HTML standard.



* Common Audio formats:Only MP3, WAV, and Ogg audio are supported by the HTML standard. MP3 is the best format for compressed recorded music. The term MP3 has become synonymous with digital music. If your website is about recorded music, MP3 is the choice.


Format 	File 	Description

MIDI 	.mid
.midi 	MIDI (Musical Instrument Digital Interface). Main format for all electronic music devices like synthesizers and PC sound cards. MIDI files do not contain sound, but digital notes that can be played by electronics. Plays well on all computers and music hardware, but not in web browsers.


RealAudio 	.rm
.ram 	RealAudio. Developed by Real Media to allow streaming of audio with low bandwidths. Does not play in web browsers.


WMA 	.wma 	WMA (Windows Media Audio). Developed by Microsoft. Plays well on Windows computers, but not in web browsers.


AAC 	.aac 	AAC (Advanced Audio Coding). Developed by Apple as the default format for iTunes. Plays well on Apple computers, but not in web browsers.


WAV 	.wav 	WAV. Developed by IBM and Microsoft. Plays well on Windows, Macintosh, and Linux operating systems. Supported by HTML.


Ogg 	.ogg 	Ogg. Developed by the Xiph.Org Foundation. Supported by HTML.


MP3 	.mp3 	MP3 files are actually the sound part of MPEG files. MP3 is the most popular format for music players. Combines good compression (small files) with high quality. Supported by all browsers.

MP4 	.mp4 	MP4 is a video format, but can also be used for audio. Supported by all browsers.
<kbd>return</kbd>[Back to table of contents](#homepage)


---------


## HTML VIDEO

```<video>``` elementi videoni sahifada ko`rsatish uchun ishlatiladi.

```
<video kengligi="320" balandligi="240" boshqaruv elementlari>
   <source src="movie.mp4" type="video/mp4">
   <source src="movie.ogg" type="video/ogg">
   Brauzeringiz video tegini qo'llab-quvvatlamaydi.
</video>
```

"nazorat" atributi o'ynash, to'xtatib turish va ovoz balandligi kabi video boshqaruvlarini qo'shadi. Kenglik va balandlik atributlarini kiritish yaxshidir. Bularni o‘rnatmasdan turib, video yuklanganda sahifa tartibsiz yoki beqaror harakatlanishi mumkin.

```<source>``` elementi brauzer tanlashi mumkin bo`lgan muqobil video fayllarni belgilash imkonini beradi. Brauzer sukut bo'yicha birinchi tan olingan formatni tanlaydi. Video teglari orasidagi matn, agar brauzer <video> elementini qo'llab-quvvatlamasagina ko'rsatiladi.

* HTML ```<video>``` Avtomatik ijro

* Avtomatik ijro atributi videoni avtomatik ravishda boshlaydi.
```
<video kengligi="320" balandligi="240" avtomatik ijro>
   <source src="movie.mp4" type="video/mp4">
   <source src="movie.ogg" type="video/ogg">
   Brauzeringiz video tegini qo'llab-quvvatlamaydi.
</video>
```
Autoplay atributi iPad va iPhone kabi mobil qurilmalarda ishlamaydi.

* HTML video formatlari

Uchta qo'llab-quvvatlanadigan video formatlari mavjud: MP4, WebM va Ogg. Turli formatlar uchun brauzerni qo'llab-quvvatlash:
Brauzer MP4 WebM Ogg
Edge HA HA HA
Chrome HA HA HA
Firefox HA HA HA
Safari HA HA YO'Q
Opera HA HA HA


* HTML video - Media turlari
Fayl formati media turi
MP4 video/mp4
WebM video/webm
Ogg video/ogg

* HTML video - usullar, xususiyatlar va hodisalar

HTML DOM <video> elementi uchun usullar, xususiyatlar va hodisalarni belgilaydi.

Bu sizga videolarni yuklash, ijro etish va to‘xtatib turish, shuningdek, davomiylik va ovoz balandligini sozlash imkonini beradi.

Shuningdek, video o'ynay boshlaganda, to'xtatilganda va hokazolarda sizni xabardor qiladigan DOM hodisalari mavjud.


* HTML-da videoni qanday sozlash haqida batafsil ma'lumot uchun HTML video audio DOM ma'lumotnomasiga qarang

Xulosa
HTML video teglar
Teg tavsifi
```
<video> Video yoki filmni belgilaydi
<source> <video> va <audio> kabi media elementlari uchun bir nechta media resurslarini belgilaydi
<track> Media pleerlardagi matn treklarini belgilaydi
```
<kbd>qaytish</kbd>[Mundarijaga qaytish](#homepage)

------



## HTML AUDIO

HTML ```<audio>``` elementi

```<audio>``` elementi audio faylni ijro etish uchun ishlatiladi.
```
<audio boshqaruvlari>
   <source src="horse.ogg" type="audio/ogg">
   <source src="horse.mp3" type="audio/mpeg">
Brauzeringiz audio elementni qo'llab-quvvatlamaydi.
</audio>
```

* HTML Audio - u qanday ishlaydi

Controls atributi ijro, pauza va ovoz balandligi kabi audio boshqaruv elementlarini qo‘shadi.

```<source>``` elementi brauzer tanlashi mumkin bo`lgan muqobil audio fayllarni belgilash imkonini beradi. Brauzer birinchi tan olingan formatdan foydalanadi.

```<audio>``` va ```</audio>``` teglari orasidagi matn faqat ```<audio>``` elementini qo`llab-quvvatlamaydigan brauzerlarda ko`rsatiladi.


Qo'llab-quvvatlanadigan uchta audio format mavjud: MP3, WAV, OGG.


Opera, Firefox va Chrome barcha audio formatlarini qo'llab-quvvatlaydi. Edge/Internet Explorer faqat MP3-ni, Safari esa faqat MP3 va WAV-ni qo'llab-quvvatlaydi.


HTML Audio - Media turlari
Fayl formati media turi
MP3 audio/mpeg
OGG audio/ogg
WAV audio/wav


* HTML Audio - usullar, xususiyatlar va hodisalar

HTML DOM ```<audio>``` elementi uchun usullar, xususiyatlar va hodisalarni belgilaydi.

Bu sizga audiolarni yuklash, ijro etish va pauza qilish, shuningdek, davomiylik va ovoz balandligini belgilash imkonini beradi.

Bundan tashqari, audio o'ynay boshlaganda, to'xtatilganda va hokazolarda sizga xabar beradigan DOM hodisalari mavjud.

Toʻliq DOM maʼlumotnomasi uchun w3c HTML Audio/Video DOM maʼlumotnomasiga oʻting.

HTML audio teglar
Teg tavsifi
```<audio>``` Ovoz tarkibini belgilaydi
```<manba>``` <video> va <audio> kabi media elementlari uchun bir nechta media resurslarini belgilaydi
<kbd>qaytish</kbd>[Mundarijaga qaytish](#homepage)


-------


## HTML YOUTUBE

HTML YouTube videolari

Bu HTML-da videolarni o'ynashning eng oson usuli, chunki u turli formatlarga o'tkazish zaruriyatini yo'q qiladi. Konvertatsiya muammosini bartaraf qilish uchun YouTube-ga veb-saytingizda videolarni o'ynashga ruxsat berilishi mumkin.


* YouTube video identifikatori

Videoni saqlaganingizda (yoki o'ynaganingizda) YouTube identifikatorni (masalan, tgbNymZ7vqY) ko'rsatadi.

Siz ushbu identifikatordan foydalanishingiz va HTML kodidagi videongizga murojaat qilishingiz mumkin.

* YouTube'ni HTML formatida o'ynatish

Videongizni veb-sahifada ijro etish uchun quyidagilarni bajaring:
Videoni YouTube-ga yuklang
Video identifikatoriga e'tibor bering
Veb-sahifangizda <iframe> elementini aniqlang
src atributi video URL manziliga ishora qilsin
Pleyerning o'lchamini belgilash uchun kenglik va balandlik atributlaridan foydalaning
URL manziliga boshqa parametrlarni qo'shing (pastga qarang)

```
<iframe kengligi="420" balandligi="345" src="https://www.youtube.com/embed/tgbNymZ7vqY">
</iframe>
```

* YouTube avtomatik ijro + ovozsiz

YouTube URL manziliga autoplay=1 qo‘shish orqali foydalanuvchi sahifaga tashrif buyurganida videongizni avtomatik o‘ynay boshlashiga ruxsat berishingiz mumkin.

Eslatma: Videoni avtomatik boshlash tashrif buyuruvchini bezovta qilishi va natijada foydadan ko'ra ko'proq zarar keltirishi mumkin!

Chrome 2018-yilda qattiqroq avtomatik ijro qilish siyosatlarini qo‘shdi. Chromium brauzerlari hamma hollarda avtomatik ijro qilishga ruxsat bermaydi. Biroq, ovozsiz avtomatik ijroga har doim ruxsat beriladi.

Videongiz avtomatik ijro etilishi uchun (lekin ovozi oʻchirilgan) uchun avtomatik ijro=1dan keyin ovozni oʻchirish=1 qoʻshing.

```
<iframe width="420" height="345" src="https://www.youtube.com/embed/tgbNymZ7vqY?autoplay=1&mute=1">
</iframe>
```
```
  <iframe width="420" height="345" src="https://www.youtube.com/embed/tgbNymZ7vqY?playlist=tgbNymZ7vqY&loop=1">
</iframe>
```

```
<iframe width="420" height="345" src="https://www.youtube.com/embed/tgbNymZ7vqY?playlist=tgbNymZ7vqY&loop=1">
</iframe>
```

* YouTube boshqaruvlari

Video pleerda boshqaruv elementlarini ko‘rsatish uchun boshqaruv elementlarini qo‘shing=0.

Qiymat 0: Pleyer boshqaruvlari ko'rsatilmaydi.

Qiymat 1 (standart): Pleyer boshqaruvlari ekrani.

```
<iframe width="420" height="345" src="https://www.youtube.com/embed/tgbNymZ7vqY?controls=0">
</iframe>
```
<kbd>qaytish</kbd>[Mundarijaga qaytish](#homepage)


---------


## CSS Inline-blok

CSS Layout - displey: inline-block;

Displey: inline-block Qiymat:

Displeydan farqli o'laroq:inline; yuqori va pastki chekkalarga/to'ldirishlarga rioya qilmaydi, displey: inline-block

yuqori va pastki chetlariga/to'ldiruvchiga hurmat ko'rsatadi, shuningdek, elementga kenglik va balandlikni o'rnatish imkonini beradi.

Displey bilan solishtirganda:blok; displey:inline-blok elementdan keyin qator uzilishini qo'shmaydi, shuning uchun

element boshqa elementlarning yonida joylashishi mumkin. E'tibor bering, displey:inline; oraliq uchun standart hisoblanadi. ga qarang

displey orasidagi farqning tasviri: inline; , displey: inline-block; , va displey:blok;


<!DOCTYPE html>
<html>
<head>
<uslub>
span.a {
   displey: inline; /* oraliq uchun standart */
   kengligi: 100px;
   balandligi: 100px;
   to'ldirish: 5px;
   chegara: 1px to'liq ko'k;
   fon rangi: sariq;
}

span.b {
   displey: inline-block;
   kengligi: 100px;
   balandligi: 100px;
   to'ldirish: 5px;
   chegara: 1px to'liq ko'k;
   fon rangi: sariq;
}

span.c {
   displey: blok;
   kengligi: 100px;
   balandligi: 100px;
   to'ldirish: 5px;
   chegara: 1px to'liq ko'k;
   fon rangi: sariq;
}
</style>
</head>
<tana>

<h1>Displey xususiyati</h1>

<h2>displey: inline</h2>
<div>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum consequat scelerisque elit sit amet

natija. To'g'ri keladi. <span class="a">Aliquam</span> <span class="a">venenatis</span> gravida

nisl sit amet facilisis. Nullam cursus fermentum velit sed laoreet. </div>

<h2>displey: inline-block</h2>
<div>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum consequat scelerisque elit sit amet

natija. To'g'ri keladi. <span class="b">Aliquam</span> <span class="b">venenatis</span> gravida

nisl sit amet facilisis. Nullam cursus fermentum velit sed laoreet. </div>

<h2>displey: blokirovka</h2>
<div>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum consequat scelerisque elit sit amet

natija. To'g'ri keladi. <span class="c">Aliquam</span> <span class="c">venenatis</span> gravida

nisl sit amet facilisis. Nullam cursus fermentum velit sed laoreet. </div>

</body>
</html>


Navigatsiya havolalarini yaratish uchun inline-blokdan foydalanish;

Display:inline-block ning keng tarqalgan qo'llanilishi ro'yxat elementlarini vertikal emas, balki gorizontal ravishda ko'rsatishdir.

Gorizontal navigatsiya havolalariga misol uchun quyida ko'ring:


<!DOCTYPE html>
<html>
<head>
<uslub>
.nav {
   fon rangi: sariq;
   ro'yxat uslubi turi: yo'q;
   matnni tekislash: markaz;
   chegara: 0;
   to'ldirish: 0;
}

.nav li {
   displey: inline-block;
   shrift o'lchami: 20px;
   to'ldirish: 20px;
}
</style>
</head>
<tana>

<h1>Gorizontal navigatsiya havolalari</h1>
<p>Sukut bo'yicha ro'yxat elementlari vertikal ravishda ko'rsatiladi. Ushbu misolda biz ko'rsatish uchun displey: inline-block dan foydalanamiz

ularni gorizontal (yonma-yon).</p>
<p>Eslatma: Agar brauzer oynasining oʻlchamini oʻzgartirsangiz, u ham oʻzgarganda havolalar avtomatik ravishda buziladi

gavjum.</p>

<ul class="nav">
   <li><a href="#home">Uy</a></li>
   <li><a href="#about">Biz haqimizda</a></li>
   <li><a href="#clients">Bizning mijozlarimiz</a></li>
   <li><a href="#contact">Biz bilan bog‘laning</a></li>
</ul>

</body>
</html>

<kbd>qaytish</kbd>[Mundarijaga qaytish](#homepage)


--------


## CSS kombinatorlari

HTML-sahifadagi selektorlar orasidagi munosabat kombinatorlar orqali tushuntiriladi.

CSS selektorida bir nechta bitta selektor bo'lishi mumkin va biz ularning orasiga kombinatorni kiritishimiz mumkin

oddiy selektorlar. To'rtta noyob kombinator va ularning CSS-dagi ko'rinishi (qavslar ichida) quyidagilarni o'z ichiga oladi:



     avlod selektori (bo'sh joy)
     bola tanlagichi (>)
     qo'shni aka-uka selektori (+)
     umumiy aka-uka selektori (~)



Nasl selektori ( );

Nasl selektori bir xil ko'rsatilgan elementning avlodlari bo'lgan barcha elementlarga mos keladi. Bu

bo'sh joy yordamida belgilangan. Masalan, quyidagi kodda <div> ichidagi <p> elementlari

elementlar tanlanadi:


<!DOCTYPE html>
<html>
<head>
<uslub>
div p {
   fon rangi: sariq;
}
</style>
</head>
<tana>

<h2>Nasl selektori</h2>
<p>Asl selektor belgilangan elementning avlodi boʻlgan barcha elementlarga mos keladi.</p>

<div>
   <p>Div.dagi 1-xat.</p>
   <p>Div.dagi 2-xatboshi.</p>
   <section><p>3-banddagi boʻlim.</p></section>
</div>

<p>4-paragraf. Bo'limda emas.</p>
<p>5-paragraf. Bo'linmada emas.</p>

</body>
</html>


Bolalar tanlovchisi (>)

Child selektor belgilangan elementning bolalari bo'lgan barcha elementlarni tanlaydi. yordamida belgilanadi

belgisidan kattaroqdir. Quyidagi kodda, masalan, <div> ning bolalari bo'lgan barcha <p> elementlari

element tanlangan:



<!DOCTYPE html>
<html>
<head>
<uslub>
div > p {
   fon rangi: sariq;
}
</style>
</head>
<tana>

<h2>Child Selector</h2>
<p>Bola tanlovchi (>) belgilangan elementning bolalari bo'lgan barcha elementlarni tanlaydi.</p>

<div>
   <p>Div.dagi 1-xat.</p>
   <p>Div.dagi 2-xatboshi.</p>
   <section><p>3-paragraf bo'limda.</p></section> <!-- Bola emas, balki avlod -->
   <p>Div.dagi 4-band.</p>
</div>

<p>5-paragraf. Bo'linmada emas.</p>
<p>6-paragraf. Bo'linmada emas.</p>

</body>
</html>



E'tibor bering, to'g'ridan-to'g'ri ota-ona ostida bo'lmagan, lekin sub-ota-onaga ega bo'lgan elementlar boshqasining farzandi emas, balki avloddir.




Qo'shni birodarlar selektori (+);


Qo'shni birodar selektori boshqa muayyan elementdan keyin joylashgan elementni tanlash uchun ishlatiladi.

Bu erda qo'shni "darhol ergash" degan ma'noni anglatadi. Qardosh elementlar bir xil ota-onaga ega bo'lishi kerak. Qo'shni uka

selektor ortiqcha (+) belgisi bilan belgilanadi. Quyidagi misolda faqat birinchi <p> elementlar mavjud

<div> elementlari tanlanganidan keyin "darhol" joylashtiriladi.

<!DOCTYPE html>
<html>
<head>
<uslub>
div + p {
   fon rangi: sariq;
}
</style>
</head>
<tana>

<h2>Qoʻshni aka-uka selektori</h2>

<p>+ selektori toʻgʻridan-toʻgʻri boshqa muayyan elementdan keyin keladigan elementni tanlash uchun ishlatiladi.</p>
<p>Quyidagi misol div elementlaridan keyin darhol joylashtirilgan birinchi p elementni tanlaydi:</p>

<div>
   <p>Div.dagi 1-xat.</p>
   <p>Div.dagi 2-xatboshi.</p>
</div>

<p>3-xatboshi. Bo'limdan keyin.</p>
<p>4-paragraf. Bo'limdan keyin.</p>

<div>
   <p>Bo'limdagi 5-band.</p>
   <p>Bo'limdagi 6-band.</p>
</div>

<p>7-xatboshi. Bo'limdan keyin.</p>
<p>8-paragraf. Bo'limdan keyin.</p>

</body>
</html>


Umumiy birodarlar selektori (~);

Umumiy aka-uka selektori belgilangan elementning “keyingi birodarlari” bo‘lgan “barcha” elementlarni tanlaydi. Bu

tilda belgisi (~) bilan belgilanadi. Tanadagi barcha elementlar <html> ning birodarlari ekanligini unutmang. Misolda

quyida, <div> elementlarining keyingi birodarlari bo'lgan barcha <p> elementlar tanlangan:



<!DOCTYPE html>
<html>
<head>
<uslub>
div ~ p {
   fon rangi: sariq;
}
</style>
</head>
<tana>

<h2>Umumiy birodarlar selektori</h2>
<p>Umumiy selektor (~) belgilangan elementning keyingi birodarlari bo‘lgan barcha elementlarni tanlaydi.</p>

<p>1-xatboshi.</p>

<div>
   <p>2-xatboshi.</p>
</div>

<p>3-xatboshi.</p>
<code>Ba'zi kodlar.</code>
<p>4-xatboshi.</p>

</body>
</html>

Barcha CSS Combinator selektorlari
Selektor misoli Misol tavsifi
element elementi div p <div> elementlari ichidagi barcha <p> elementlarni tanlaydi
element>element div > p Asosiy element <div> element bo'lgan barcha <p> elementlarni tanlaydi
element+element div + p Darhol joylashtirilgan birinchi <p> elementni tanlaydi

<div> elementlari
element1~element2 p ~ ul Oldindan <p> elementi joylashgan har bir <ul> elementni tanlaydi


<kbd>qaytish</kbd>[Mundarijaga qaytish](#homepage)


-------



## CSS psevdo-sinfi

Pseudo-klass elementning maxsus holatini aniqlash uchun ishlatiladi. Masalan, siz psedo-klassdan foydalanishingiz mumkin

uslub:

-foydalanuvchi uning ustiga sichqonchani bosganda element
- tashrif buyurilgan va tashrif buyurilmagan havolalar boshqacha
-fokusni oladigan element


Pseudo-klasslar uchun umumiy sintaksis:

selektor: psevdo-sinf {
   mulk: qiymat;
}

muqobil ravishda selektor sinfini belgilashingiz mumkin.

selector.class:psevdo-sinf {
   mulk: qiymat;
}





Anchor psevdo-sinflari;

Ular havolalarni turli yo'llar bilan ko'rsatish uchun ishlatiladi. Havolalarni ko'rsatishning ba'zi usullari uchun quyidagi rasmga qarang

sichqonchaning harakatiga asoslanib (tashrif buyurilgan, sichqonchaning ustiga turgan, tashrif buyurilmagan, bosish paytida):


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


Eslatma: a:hover samarali bo'lishi uchun CSS ta'rifida a:link va a:visited dan keyin kelishi KERAK! a: faol

Samarali bo'lishi uchun CSS ta'rifida a: hoverdan keyin kelishi KERAK! Pseudo-sinf nomlari katta emas-

sezgir.



Pseudo-sinflar va CSS sinflari;

Pseudo-sinflar CSS sinflari bilan birlashtirilishi mumkin. Bu psevdo sinflarni maxsus qo'llash imkonini beradi

elementlar. Quyidagi misolda kursorni havola ustiga olib borib, havola rangini o‘zgartiradi:


<!DOCTYPE html>
<html>
<head>
<uslub>
a. ta'kidlash: suring {
   rang: #ff0000;
}
</style>
</head>
<tana>

<h2>Pseudo-sinflar va CSS sinflari</h2>
<p>Quyidagi birinchi havola ustiga kursorni olib kelsangiz, uning rangi o‘zgaradi:</p>

<p><a class="highlight" href="css_syntax.asp">CSS sintaksisi</a></p>
<p><a href="default.asp">CSS qo‘llanmasi</a></p>

</body>
</html>




Kursorni <div> ustiga olib boring;

Quyidagi misolda <div> elementida :hover pseudo-classdan qanday foydalanish ko'rsatilgan:

<!DOCTYPE html>
<html>
<head>
<uslub>
div {
   fon rangi: yashil;
   rang: oq;
   to'ldirish: 25px;
   matnni tekislash: markaz;
}

div: suring {
   fon rangi: ko'k;
}
</style>
</head>
<tana>

<p>Fon rangini oʻzgartirish uchun sichqonchani quyidagi div elementi ustiga bosing:</p>

<div>Sichqoncha ustimda</div>

</body>
</html>



Simple Tooltip Hover;

Bu sizga <div> elementi ustiga olib borish orqali <p> elementini (masalan, asboblar maslahati) ko'rsatish imkonini beradi. Siz ham foydalanishingiz mumkin

boshqa tanlovchilar uchun. Quyidagi rasmga qarang:

<!DOCTYPE html>
<html>
<head>
<uslub>
p {
   ko'rsatish: yo'q;
   fon rangi: sariq;
   to'ldirish: 20px;
}

div: hover p {
   displey: blok;
}
</style>
</head>
<tana>

<div>P elementini ko'rsatish uchun kursorni mening ustimga olib boring
   <p>Tada! Mana men!</p>
</div>

</body>
</html>



CSS - :birinchi bola psevdo-sinfi

:first-child psevdo-sinfi boshqa elementning birinchi bolasi bo'lgan belgilangan elementga mos keladi.


Birinchi <p> elementni moslang::

Quyidagi misolda selektor har qanday elementning birinchi bolasi bo'lgan har qanday <p> elementga mos keladi:



<!DOCTYPE html>
<html>
<head>
<uslub>
p: birinchi farzand {
   rang: ko'k;
}
</style>
</head>
<tana>

<p>Bu qandaydir matn.</p>
<p>Bu qandaydir matn.</p>

</body>
</html>



Barcha <p> elementlardagi birinchi <i> elementni moslang::

Quyidagi misolda selektor barcha <p> elementlardagi birinchi <i> elementga mos keladi:

<!DOCTYPE html>
<html>
<head>
<uslub>
p i:birinchi farzand {
   rang: ko'k;
}
</style>
</head>
<tana>

<p>Men <i>kuchli</i> odamman. Men <i>kuchli</i> odamman.</p>
<p>Men <i>kuchli</i> odamman. Men <i>kuchli</i> odamman.</p>

</body>
</html>



Barcha birinchi kichik <p> elementlardagi barcha <i> elementlarni moslang::

Quyidagi misolda selektor boshqa elementning birinchi farzandi bo'lgan <p> elementlardagi barcha <i> elementlarga mos keladi.

element:


<!DOCTYPE html>
<html>
<head>
<uslub>
p:birinchi farzand men {
   rang: ko'k;
}
</style>
</head>
<tana>

<p>Men <i>kuchli</i> odamman. Men <i>kuchli</i> odamman.</p>
<p>Men <i>kuchli</i> odamman. Men <i>kuchli</i> odamman.</p>

</body>
</html>


CSS - :lang psevdo-sinfi::

:lang pseudo klassi turli tillar uchun maxsus qoidalarni belgilash imkonini beradi. Misoldagi :lang

quyida lang= "yo'q" bo'lgan <q> elementlar uchun tirnoq belgilari aniqlanadi (bu holatda qo'shtirnoq ishlatiladi

~Matn bu yerda~:


<!DOCTYPE html>
<html>
<head>
<uslub>
q:lang (yo'q) {
   tirnoq: "~" "~";
}
</style>
</head>
<tana>

<p>Ba'zi matn <q lang="no">Xatboshidagi iqtibos</q> Ba'zi matn.</p>
<p>Ushbu misolda :lang q element uchun qo'shtirnoqlarni lang="no" bilan belgilaydi:</p>

</body>
</html>


Pseudo-klassning ba'zi qo'shimcha misollari:

Giperhavolalarga turli uslublar qo'shish:::

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

<h2>Stillash havolalari</h2>

<p>Sichqonchani havolalar ustiga bosing va ularning tartibini oʻzgartirishini tomosha qiling:</p>

<p><b><a class="one" href="default.asp" target="_blank">Ushbu havola rangini o'zgartiradi</a></b></p>
<p><b><a class="two" href="default.asp" target="_blank">Ushbu havola shrift hajmini o'zgartiradi</a></b></p>
<p><b><a class="three" href="default.asp" target="_blank">Bu havola fon rangini o'zgartiradi</a></b></p>
<p><b><a class="four" href="default.asp" target="_blank">Ushbu havola font-family-ni o'zgartiradi</a></b></p>
<p><b><a class="five" href="default.asp" target="_blank">Ushbu havola matn bezaklarini o'zgartiradi</a></b></p>

</body>
</html>



Fokusdan foydalanish:::

:focus pseudo-klassi sahifada ish olib borilayotgan vaqtda uning qismini uslublash uchun ishlatiladi. Masalan, siz

Fokusdagi shakllar paneli uchun psevdo-sinfdan foydalangan holda ma'lum uslubni belgilashi mumkin (hozirda to'ldirilmoqda):


<!DOCTYPE html>
<html>
<head>
<uslub>
kiritish: fokus {
   fon rangi: sariq;
}
</style>
</head>
<tana>

<form action="/action_page.php" method="get">
   Ism: <input type="text" name="fname"><br>
   Familiya: <input type="text" name="lname"><br>
   <input type="submit" value="yuborish">
</form>

</body>
</html>





Bu erda qo'shimcha Pseudo-sinflar va ulardan foydalanishga yordam beradigan maslahatlar:



Barcha CSS psevdo sinflari

Selektor misoli Misol tavsifi
:active a:active Faol havolani tanlaydi
:checked input:checked Har bir belgilangan <input> elementini tanlaydi
:disabled input:disabled Har bir o'chirilgan <input> elementini tanlaydi
:empty p:empty Bolalari bo'lmagan har bir <p> elementni tanlaydi
:enabled input:enabled Har bir yoqilgan <input> elementini tanlaydi
:first-child p:first-child Ota-onasining birinchi farzandi bo'lgan har bir <p> elementni tanlaydi
:birinchi turdagi p:birinchi turi o'zining birinchi <p> elementi bo'lgan har bir <p> elementni tanlaydi.

ota-ona
:focus input:focus Fokusga ega <input> elementini tanlaydi
:hover a:hover Sichqoncha ustidagi havolalarni tanlaydi
:in-range input:in-range Belgilangan diapazondagi qiymatga ega <input> elementlarini tanlaydi
:invalid input:invalid Noto'g'ri qiymatga ega barcha <input> elementlarini tanlaydi
:lang(language) p:lang(it) bilan boshlanadigan lang atribut qiymatiga ega har bir <p> elementni tanlaydi.

"bu"
:last-child p:last-child Ota-onasining oxirgi bolasi bo'lgan har bir <p> elementni tanlaydi
:last-of-type p:last-of-pe ota-onasining oxirgi <p> elementi bo'lgan har bir <p> elementni tanlaydi.
:link a:link Barcha tashrif buyurilmagan havolalarni tanlaydi
:not(selektor) :not(p) <p> elementi boʻlmagan har bir elementni tanlaydi
:nth-child(n) p:nth-child(2) ota-onasining ikkinchi farzandi bo'lgan har bir <p> elementni tanlaydi
:nth-so'nggi-child(n) p:nth-last-child(2) O'zining ikkinchi bolasi bo'lgan har bir <p> elementni tanlaydi

ota-ona, oxirgi boladan hisoblash
:nth-oxirgi-tur(n) p:nth-oxirgi-tur(2) Ikkinchi <p> elementi boʻlgan har bir <p> elementni tanlaydi.


uning ota-onasi, oxirgi bolasidan boshlab hisoblash
:nth-of-type(n) p:nth-of-type(2) ikkinchi <p> elementi bo‘lgan har bir <p> elementni tanlaydi.

uning ota-onasi
: only-of-type p: only-of-type ota-onasining yagona <p> elementi bo‘lgan har bir <p> elementni tanlaydi.
:only-child p:only-child Ota-onasining yagona farzandi bo'lgan har bir <p> elementni tanlaydi
:ixtiyoriy kiritish:ixtiyoriy “kerakli” atributsiz <input> elementlarini tanlaydi
:out-of-range input:out-of-range Belgilangan diapazondan tashqaridagi qiymatga ega <input> elementlarini tanlaydi.
:faqat o‘qish uchun kiritish:faqat o‘qish uchun “faqat o‘qish” atributi ko‘rsatilgan <input> elementlarini tanlaydi.
:o'qish-yozish kiritish:o'qish-yozish "faqat o'qish" atributiga ega bo'lmagan <input> elementlarini tanlaydi
:required input:required "kerakli" atributi ko'rsatilgan <input> elementlarini tanlaydi
:root root Hujjatning ildiz elementini tanlaydi
:target #news:target Joriy faol #news elementini tanlaydi (uni o'z ichiga olgan URL manziliga bosing)

langar nomi)
:valid input:valid To'g'ri qiymatga ega barcha <input> elementlarini tanlaydi
:visited a:visited Barcha tashrif buyurilgan havolalarni tanlaydi



Barcha CSS psevdo elementlari

Selektor misoli Misol tavsifi
::so'ng p::after Har bir <p> elementdan keyin tarkibni kiriting
:: p::befor dan oldin Har bir <p> elementdan oldin tarkibni kiriting
::birinchi harf p::birinchi harf Har bir <p> elementining birinchi harfini tanlaydi
::first-line p::first-line Har bir <p> elementining birinchi qatorini tanlaydi
::selection p::selection Elementning foydalanuvchi tomonidan tanlangan qismini tanlaydi

<kbd>qaytish</kbd>[Mundarijaga qaytish](#homepage)



----------


## CSS psevdoelementi

CSS pseudo-elementi elementning muayyan qismlarini uslublash uchun ishlatiladi, masalan:
Elementning birinchi harfi yoki satrini shakllantirish; yoki
Kontentni boshqa element tarkibidan oldin yoki keyin kiritish.



Pseudoelementlarning sintaksisi:

selektor :: pseudo-element {
   mulk: qiymat;
}




::birinchi qator psevdoelement ;;

::birinchi qator psevdoelementi matnning birinchi qatoriga maxsus uslub qo‘shish uchun ishlatiladi. Misolda

quyida barcha <p> elementlardagi matnning birinchi qatori formatlanadi:


<!DOCTYPE html>
<html>
<head>
<uslub>
p :: birinchi qator {
   rang: #ff0000;
   shrift-variant: kichik bosh harflar;
}
</style>
</head>
<tana>

<p>Matnning birinchi qatoriga maxsus effekt qoʻshish uchun ::birinchi qator psevdoelementidan foydalanishingiz mumkin. Biroz

ko'proq matn. Va bundan ham ko'proq va ko'proq va ko'proq va ko'proq va ko'proq va ko'proq va ko'proq va yana ko'proq va yana ko'proq va yana ko'proq va ko'proq

va boshqalar, va yana koʻp va boshqalar.</p>

</body>
</html>


E'tibor bering, ::birinchi qator psevdoelementi faqat blok darajasidagi elementlarga qo'llanilishi mumkin. Quyidagi

xossalari ::birinchi qator pseudoelement:shrift xususiyatlari, rang xususiyatlari, fon uchun amal qiladi

xususiyatlar, so‘z oralig‘i, harflar oralig‘i, matnni bezash, vertikal tekislash, matnni o‘zgartirish va satr balandligi;

aniq.

::birinchi qatorning qo'sh nuqta belgisi CSS3 da qo'llaniladigan standartdir (CSS 1 va 2 dan farqli o'laroq, bu erda bitta

yo'g'on ichak ishlatilgan, ya'ni: birinchi qator). Bu psevdoelementlar va psevdosinflarni ajratishga yordam beradi. Uchun

orqaga qarab muvofiqlik, bitta rangli sintaksis CSS2 va CSS1 psevdo-elementlarida qabul qilinadi.



The ::birinchi harf Pseudo-element ;;

::birinchi harf psevdoelementi matnning birinchi harfiga maxsus uslub qo'shish uchun ishlatiladi. Misol

quyida barcha <p> matnning birinchi harfini formatlash uchun ::birinchi harf psevdo elementidan qanday foydalanish ko'rsatilgan.

elementlar:

<!DOCTYPE html>
<html>
<head>
<uslub>
p :: birinchi harf {
   rang: #ff0000;
   shrift o'lchami: xx-katta;
}
</style>
</head>
<tana>

<p>Matnning birinchi belgisiga maxsus effekt qo'shish uchun ::birinchi harf psevdoelementidan foydalanishingiz mumkin!

</p>

</body>
</html>



Esda tuting: ::birinchi harfli psevdo element faqat blok darajasidagi elementlarga qo'llanilishi mumkin. Quyidagi

xususiyatlar ::birinchi harf psevdoelement:shrift xususiyatlari, rang xususiyatlari, fonga tegishli

xususiyatlar, chekka xossalari, to‘ldirish xususiyatlari, chegara xususiyatlari, matnni bezash, vertikal tekislash (faqat

agar "float" "yo'q" bo'lsa), matnni o'zgartirish, chiziq balandligi, float va aniq.



Pseudo-elementlar va CSS sinflari::

Pseudo-elementlar CSS sinflari bilan ham birlashtirilishi mumkin. Bu ma'lum bir <p> ni tanlashingizni ta'minlaydi

barcha <p> elementlarga psevdo-element uslubini qo'llash o'rniga element. Bu holda, birinchi harfi

class="intro" yozilgan paragraflar qizil rangda va kattaroq hajmda ko'rsatiladi. Quyidagi rasmga qarang:

<!DOCTYPE html>
<html>
<head>
<uslub>
p.intro::birinchi harf {
   rang: #ff0000;
   shrift hajmi: 200%;
}
</style>
</head>
<tana>

<p class="intro">Bu kirish.</p>
<p>Bu biroz matnli paragraf. Hatto biroz ko'proq matn.</p>

</body>
</html>


Bir nechta psevdoelementlar::

Bir nechta psevdoelementlar ham birlashtirilishi mumkin. Quyidagi misolda paragrafning birinchi harfi bo'ladi

qizil, XX-katta shrift o'lchamida. Birinchi qatorning qolgan qismi ko'k va kichik harflarda bo'ladi. Qolganlari

paragraf standart shrift hajmi va rangi bo'ladi. Quyidagi rasmga qarang:


<!DOCTYPE html>
<html>
<head>
<uslub>
p :: birinchi harf {
   rang: #ff0000;
   shrift o'lchami: xx-katta;
}

p :: birinchi qator {
   rang: #0000ff;
   shrift-variant: kichik bosh harflar;
}
</style>
</head>
<tana>

<p>Birinchi harfga maxsus effekt qo'shish uchun ::birinchi harf va ::birinchi qator psevdoelementlarini birlashtira olasiz.

harf va matnning birinchi qatori!</p>

</body>
</html>



CSS - Pseudo-element:: dan oldingi ::

Pseudo-elementdan oldin :: element mazmunidan oldin ba'zi tarkibni kiritish uchun ishlatilishi mumkin. In

quyidagi misol va rasm (smiley.gif) har bir <h1> elementi mazmunidan oldin kiritiladi:


<!DOCTYPE html>
<html>
<head>
<uslub>
h1 :: oldin {
   kontent: url (smiley.gif);
}
</style>
</head>
<tana>

<h1>Bu sarlavha</h1>
<p>::befor psevdoelement kontentni element mazmunidan oldin kiritadi.</p>

<h1>Bu sarlavha</h1>

</body>
</html>




CSS - Pseudo-elementdan keyin ::


::after pseudo-element element mazmunidan keyin ba'zi tarkibni kiritish uchun ishlatilishi mumkin. Misol

quyida har bir <h1> elementidan keyin rasm qo'shilishi ko'rsatilgan:


<!DOCTYPE html>
<html>
<head>
<uslub>
h1 :: keyin {
   kontent: url (smiley.gif);
}
</style>
</head>
<tana>

<h1>Bu sarlavha</h1>
<p>::after pseudo-element element mazmunidan keyin tarkibni kiritadi.</p>

<h1>Bu sarlavha</h1>

</body>
</html>


CSS - :: marker Pseudo-element

::marker psevdoelementi elementlar roʻyxati markerlarini tanlaydi (uslublar). Quyidagi misol uslubni ko'rsatadi

::marker pseudo-elementdan foydalangan holda elementlar ro'yxati markerlari:


<!DOCTYPE html>
<html>
<head>
<uslub>
:: marker {
   rang: qizil;
   shrift o'lchami: 23px;
}
</style>
</head>
<tana>

<ul>
   <li>Qahva</li>
   <li>Choy</li>
   <li>Sut</li>
</ul>

<ol>
   <li>Birinchi</li>
   <li>Ikkinchi</li>
   <li>Uchinchi</li>
</ol>

</body>
</html>


Eslatma: Bu yerda sinfga qarab uslub yaratishingiz shart emas, :: marker uslubi barcha markerlarga qo'llaniladi.




CSS - ::selection Pseudo-element::


:: tanlov psevdo-elementi foydalanuvchi tomonidan tanlangan element qismiga mos keladi. Xususiyatlari

::tanlovga qo'llanilishi mumkin bo'lganlar quyidagilardan iborat: rang, fon, kursor va kontur. dagi uslublar

Quyidagi misol tanlangan matnni sariq fonda qizil qiladi:


<!DOCTYPE html>
<html>
<head>
<uslub>
::-moz-selection { /* Firefox uchun kod */
   rang: qizil;
   fon: sariq;
}

:: tanlash {
   rang: qizil;
   fon: sariq;
}
</style>
</head>
<tana>

<h1>Ushbu sahifadagi matnni tanlang:</h1>

<p>Bu paragraf.</p>
<div>Bu div elementidagi ba'zi matn.</div>

<p><strong>Eslatma:</strong> Firefox muqobil ::-moz-selection xususiyatini qo‘llab-quvvatlaydi.</p>

</body>
</html>




Barcha CSS psevdo elementlari
Selektor misoli Misol tavsifi
::after p::after Har bir <p> elementi mazmunidan keyin biror narsa kiriting
:: p::befor dan oldin Har bir <p> elementi mazmunidan oldin biror narsani kiriting
::birinchi harf p::birinchi harf Har bir <p> elementining birinchi harfini tanlaydi
::first-line p::first-line Har bir <p> elementining birinchi qatorini tanlaydi
::marker ::marker Ro'yxat elementlarining markerlarini tanlaydi
::selection p::selection Elementning foydalanuvchi tomonidan tanlangan qismini tanlaydi
Barcha CSS psevdo sinflari
Selektor misoli Misol tavsifi
:active a:active Faol havolani tanlaydi
:checked input:checked Har bir belgilangan <input> elementini tanlaydi
:disabled input:disabled Har bir o'chirilgan <input> elementini tanlaydi
:empty p:empty Bolalari bo'lmagan har bir <p> elementni tanlaydi
:enabled input:enabled Har bir yoqilgan <input> elementini tanlaydi
:first-child p:first-child Ota-onasining birinchi farzandi bo'lgan har bir <p> elementni tanlaydi
:birinchi turdagi p:birinchi turi o'zining birinchi <p> elementi bo'lgan har bir <p> elementni tanlaydi.

ota-ona
:focus input:focus Fokusga ega <input> elementini tanlaydi
:hover a:hover Sichqoncha ustidagi havolalarni tanlaydi
:in-range input:in-range Belgilangan diapazondagi qiymatga ega <input> elementlarini tanlaydi
:invalid input:invalid Noto'g'ri qiymatga ega barcha <input> elementlarini tanlaydi
:lang(language) p:lang(it) bilan boshlanadigan lang atribut qiymatiga ega har bir <p> elementni tanlaydi.

"bu"
:last-child p:last-child Ota-onasining oxirgi bolasi bo'lgan har bir <p> elementni tanlaydi
:last-of-type p:last-of-pe ota-onasining oxirgi <p> elementi bo'lgan har bir <p> elementni tanlaydi.
:link a:link Barcha tashrif buyurilmagan havolalarni tanlaydi
:not(selektor) :not(p) <p> elementi boʻlmagan har bir elementni tanlaydi
:nth-child(n) p:nth-child(2) ota-onasining ikkinchi farzandi bo'lgan har bir <p> elementni tanlaydi
:nth-so'nggi-child(n) p:nth-last-child(2) O'zining ikkinchi bolasi bo'lgan har bir <p> elementni tanlaydi

ota-ona, oxirgi boladan hisoblash
:nth-oxirgi-tur(n) p:nth-oxirgi-tur(2) Ikkinchi <p> elementi boʻlgan har bir <p> elementni tanlaydi.

uning ota-onasi, oxirgi bolasidan boshlab hisoblash
:nth-of-type(n) p:nth-of-type(2) ikkinchi <p> elementi bo‘lgan har bir <p> elementni tanlaydi.

uning ota-onasi
: only-of-type p: only-of-type ota-onasining yagona <p> elementi bo‘lgan har bir <p> elementni tanlaydi.
:only-child p:only-child Ota-onasining yagona farzandi bo'lgan har bir <p> elementni tanlaydi
:ixtiyoriy kiritish:ixtiyoriy “kerakli” atributsiz <input> elementlarini tanlaydi
:out-of-range input:out-of-range Belgilangan diapazondan tashqaridagi qiymatga ega <input> elementlarini tanlaydi.
:faqat o‘qish uchun kiritish:faqat o‘qish uchun “faqat o‘qish” atributi ko‘rsatilgan <input> elementlarini tanlaydi.
:o'qish-yozish kiritish:o'qish-yozish "faqat o'qish" atributiga ega bo'lmagan <input> elementlarini tanlaydi
:required input:required "kerakli" atributi ko'rsatilgan <input> elementlarini tanlaydi
:root root Hujjatning ildiz elementini tanlaydi
:target #news:target Joriy faol #news elementini tanlaydi (uni o'z ichiga olgan URL manziliga bosing)

langar nomi)
:valid input:valid To'g'ri qiymatga ega barcha <input> elementlarini tanlaydi
:visited a:visited Barcha tashrif buyurilgan havolalarni tanlaydi


<kbd>qaytish</kbd>[Mundarijaga qaytish](#homepage)


----------



## CSS shaffofligi


Shaffoflik xususiyati elementning shaffofligi yoki shaffofligini aniqlaydi.\


Shaffof rasm
Tasvirning shaffofligi 0 dan 1 gacha, 0 esa to'liq shaffof, 1,0 esa to'liq shaffof emas. Qarang

quyidagi misol kodi:


<!DOCTYPE html>
<html>
<head>
<uslub>
img {
   shaffoflik: 0,5;
}
</style>
</head>
<tana>

<h1>Tasvir shaffofligi</h1>
<p>Opaklik xususiyati elementning shaffofligini belgilaydi. Qiymat qanchalik past bo'lsa, shuncha ko'p

shaffof:</p>

<p>50% shaffoflikdagi rasm:</p>
<img src="img_forest.jpg" alt="O'rmon" kengligi="170" balandligi="100">

</body>
</html>



Shaffof Hover effekti

Rasmning shaffofligini o'zgartirish uchun :hover selektori bilan birga shaffoflik xususiyatidan foydalanish odatiy holdir.

sichqoncha ustiga o'tish. Sichqonchani bosish orqali tasvirning shaffofligini qanday o'zgartirish mumkinligi haqidagi rasmga qarang:


<!DOCTYPE html>
<html>
<head>
<uslub>
img {
   shaffoflik: 0,5;
}

img: suring {
   shaffoflik: 1,0;
}
</style>
</head>
<tana>

<h1>Tasvir shaffofligi</h1>
<p>Opaklik xususiyati ko'pincha sichqonchaning shaffofligini o'zgartirish uchun :hover selektori bilan birga ishlatiladi.

ustidan:</p>
<img src="img_forest.jpg" alt="O'rmon" kengligi="170" balandligi="100">
<img src="img_mountains.jpg" alt="Tog'lar" kengligi="170" balandligi="100">
<img src="img_5terre.jpg" alt="Italiya" kengligi="170" balandligi="100">

</body>
</html>



Yuqoridagi misolga e'tibor bering: CSS uslubi foydalanuvchi sichqonchani suratlardan birining ustiga olib kelganida nima sodir bo'lishini ko'rsatadi. Va ichida

Ushbu misolda, foydalanuvchi sichqonchani uning ustiga bosganda tasvir shaffof bo'lmasligini xohlaymiz. Buning uchun CSS shunday

shaffoflik: 1; kursorni o'rnatgandan so'ng va pseudo-klass mos ravishda o'rnatiladi.




Shaffof quti

Elementga shaffoflikni qo'shishda foydalaniladigan shaffoflik xususiyati ham asosiy elementlar tomonidan meros qilib olinadi. Bu

matnni o'qish uchun juda shaffof qilishi mumkin. Quyidagi rasmga qarang:


<!DOCTYPE html>
<html>
<head>
<uslub>
div {
   fon rangi: #4CAF50;
   to'ldirish: 10px;
}

div.first {
   shaffoflik: 0,1;
}

div.second {
   shaffoflik: 0,3;
}

div.uchinchi {
   shaffoflik: 0,6;
}
</style>
</head>
<tana>

<h1>Shaffof quti</h1>
<p>Element foniga shaffoflik qoʻshish uchun shaffoflik xususiyatidan foydalanilganda, uning barcha asosiy qismi

elementlar ham shaffof bo'ladi. Bu to'liq shaffof element ichidagi matnni qiyinlashtirishi mumkin

o'qing:</p>

<div class="first"><p>shaffoflik 0,1</p></div>
<div class="second"><p>shaffoflik 0,3</p></div>
<div class="third"><p>shaffoflik 0,6</p></div>
<div><p>shaffoflik 1 (standart)</p></div>

</body>
</html>


RGBA yordamida shaffoflik:::

RGBA dan foydalanish noshaffoflikni pastki elementlarga qo'llashni oldini oladi. Rangni RGBA sifatida belgilaganingizdan so'ng,

shaffoflik faqat fon rangi uchun o'rnatiladi, matn uchun emas.

<!DOCTYPE html>
<html>
<head>
<uslub>
div {
   fon: rgb(76, 175, 80);
   to'ldirish: 10px;
}

div.first {
   fon: rgba(76, 175, 80, 0,1);
}

div.second {
   fon: rgba(76, 175, 80, 0,3);
}

div.uchinchi {
   fon: rgba(76, 175, 80, 0,6);
}
</style>
</head>
<tana>

<h1>Shaffof quti</h1>
<p>Opaklik bilan:</p>
<div style="opacity:0.1;"><p>10% shaffoflik</p></div>
<div style="opacity:0.3;"><p>30% shaffoflik</p></div>
<div style="opacity:0.6;"><p>60% shaffoflik</p></div>
<div><p>shaffoflik 1</p></div>

<p>RGBA rang qiymatlari bilan:</p>
<div class="first"><p>10% shaffoflik</p></div>
<div class="second"><p>30% shaffoflik</p></div>
<div class="third"><p>60% shaffoflik</p></div>
<div><p>standart</p></div>

<p>Opaklik xususiyatidan foydalanganda matn qanday shaffof boʻlishiga, shuningdek fon rangiga eʼtibor bering.</p>

</body>
</html>

Shaffof qutidagi matn :::

CSS-da biz shaffof qutida ham matn yaratishimiz mumkin. Jarayon quyidagilarni o'z ichiga oladi: Birinchidan, <div> elementini yaratish

(sinf = "fon") fon tasviri va chegara bilan.

Keyin birinchi <div> ichida yana bir <div> (class="transbox") yaratamiz.

<div class="transbox"> fon rangiga ega va chegarasi - div shaffof.

Shaffof <div> ichida biz <p> elementiga bir oz matn qo'shamiz. Quyidagi misolda qanday kiritish kerakligi ko'rsatilgan

shaffof quti ichidagi matn:
 

<!DOCTYPE html>
<html>
<head>
<uslub>
div.fon {
   fon: url(klematis.jpg) takrorlash;
   chegara: 2px qattiq qora;
}

div.transbox {
   chegara: 30px;
   fon rangi: #ffffff;
   chegara: 1px qattiq qora;
   shaffoflik: 0,6;
}

div.transbox p {
   marja: 5%;
   shrift vazni: qalin;
   rang: #000000;
}
</style>
</head>
<tana>

<div class="fon">
   <div class="transbox">
     <p>Bu shaffof qutiga joylashtirilgan matn.</p>
   </div>
</div>

</body>
</html>


<kbd>qaytish</kbd>[Mundarijaga qaytish](#homepage)