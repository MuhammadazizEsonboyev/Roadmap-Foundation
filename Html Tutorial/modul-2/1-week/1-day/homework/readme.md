## CSS uslubidagi rasmlar


CSS uslubidagi rasmlar


Yumaloq Tasvirlar

Dumaloq tasvirlarni yaratish uchun chegara-radius xususiyatidan foydalaning:


Dumaloq rasm quyida ko'rsatilgan:

<!DOCTYPE html>
<html>
<head>
<style>
img {
  border-radius: 8px;
}
</style>
</head>
<body>

<h2>Yumaloq Rasm</h2>

<p>Dumaloq tasvirlarni yaratish uchun chegara-radius xususiyatidan foydalaning:</p>

<img src="paris.jpg" alt="Paris" width="300" height="300">

</body>
</html>


 Quyida aylanali rasm ko'rsatilgan:

<!DOCTYPE html>
<html>
<head>
<style>
img {
  border-radius: 50%;
}
</style>
</head>
<body>

<h2>Dumaloq rasm</h2>

<p>Aylana tasvirlarni yaratish uchun chegara-radius xususiyatidan foydalaning:</p>

<img src="paris.jpg" alt="Paris" width="300" height="300">

</body>
</html>



Kichik Rasmlar

Kichik rasmlarni yaratish uchun chegara xususiyatidan foydalaning.


Thumbnail image quyida ko'rsatilgandek yaratilgan:

<!DOCTYPE html>
<html>
<head>
<style>
img {
  border: 1px solid #ddd;
  border-radius: 4px;
  padding: 5px;
  width: 150px;
}
</style>
</head>
<body>

<h2>Thumbnail Image</h2>

<p>Use the border property to create thumbnail images:</p>

<img src="paris.jpg" alt="Paris" style="width:150px">

</body>
</html>



Havola sifatida kichik rasm quyida ko'rsatilgan:


<!DOCTYPE html>
<html>
<head>
<style>
img {
  border: 1px solid #ddd;
  border-radius: 4px;
  padding: 5px;
  width: 150px;
}

img:hover {
  box-shadow: 0 0 2px 1px rgba(0, 140, 186, 0.5);
}
</style>
</head>
<body>

<h2>Havola sifatida kichik rasm</h2>

<p>Kichik rasmlarni yaratish uchun chegara xususiyatidan foydalaning. Tasvirni ankraj sifatida ishlatish uchun uni o'rab oling 

havola.</p>
<p>Effektni ko'rish uchun kursorni rasm ustiga olib boring va ustiga bosing.</p>

<a target="_blank" href="paris.jpg">
  <img src="paris.jpg" alt="Paris" style="width:150px">
</a>

</body>
</html>




Javob Beruvchi Tasvirlar

Ta'sirchan tasvirlar avtomatik ravishda ekran o'lchamiga mos ravishda sozlanadi.

Effektni ko'rish uchun brauzer oynasining o'lchamini o'zgartiring:


Agar siz rasmni kichraytirishni xohlasangiz, lekin hech qachon asl o'lchamidan kattaroq qilib kattalashtirmasangiz, qo'shing 

quyidagi (max-kengligi: 100%; balandligi: Avto;):


<!DOCTYPE html>
<html>
<head>
<style>
img {
  max-width: 100%;
  height: auto;
}
</style>
</head>
<body>

<h2>Javob Beruvchi Rasm</h2>

<p>Ta'sirchan tasvirlar avtomatik ravishda ekran o'lchamiga mos ravishda sozlanadi.</p>
<p>Effektni ko'rish uchun brauzer oynasining o'lchamini o'zgartiring:</p>

<img src="img_5terre_wide.jpg" alt="Cinque Terre" width="1000" height="300">

</body>
</html>




Rasmni markazga qo'ying

Rasmni markazlashtirish uchun chap va o'ng chegarani auto-ga o'rnating va uni blok elementiga aylantiring:

<!DOCTYPE html>
<html>
<head>
<style>
img {
  display: block;
  margin-left: auto;
  margin-right: auto;
}
</style>
</head>
<body>

<h2>Rasmni markazga qo'ying</h2>

<p>Rasmni markazlashtirish uchun chap va o'ng chegarani auto-ga o'rnating va uni blok elementiga aylantiring.</p>

<img src="paris.jpg" alt="Paris" style="width:50%">

</body>
</html>



Polaroid Rasmlari / Kartalari

Bu chegara ostiga matn qo'yilgan rasm. Quyidagi kodni ko'ring:

<!DOCTYPE html>
<html>
<head>
<style>
body {margin:25px;}

div.polaroid {
  width: 80%;
  background-color: white;
  box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
  margin-bottom: 25px;
}

div.container {
  text-align: center;
  padding: 10px 20px;
}
</style>
</head>
<body>

<h2>Javob Polaroid Tasvirlar / Kartalari</h2>

<div class="polaroid">
  <img src="img_5terre.jpg" alt="5 Terre" style="width:100%">
  <div class="container">
  <p>Cinque Terre</p>
  </div>
</div>

<div class="polaroid">
  <img src="lights600x400.jpg" alt="Norther Lights" style="width:100%">
  <div class="container">
  <p>Shimoliy Chiroqlar</p>
  </div>
</div>

</body>
</html>



Shaffof Tasvir

Shaffoflik xususiyati 0,0 - 1,0 dan qiymat olishi mumkin. Pastki qiymat, shaffofroq:


<!DOCTYPE html>
<html>
<head>
<style>
img {
  opacity: 0.5;
}
</style>
</head>
<body>

<h1>Rasm Shaffofligi</h1>

<p>Shaffoflik xususiyati elementning shaffofligini belgilaydi. Qiymat qanchalik past bo'lsa, shuncha ko'p 

shaffof:</p>

<p>50% shaffoflik bilan rasm:</p>
<img src="img_forest.jpg" alt="Forest" width="170" height="100">

</body>
</html>



Rasm Matni

Rasmdagi matnni qanday joylashtirish kerak:


Rasmning yuqori chap pozitsiyasi:

<!DOCTYPE html>
<html>
<head>
<style>
.container {
  position: relative;
}

.topleft {
  position: absolute;
  top: 8px;
  left: 16px;
  font-size: 18px;
}

img { 
  width: 100%;
  height: auto;
  opacity: 0.3;
}
</style>
</head>
<body>

<h2>Textli rasm</h2>

<p>Yuqori chap burchakdagi rasmga bir oz matn qo'shing:</p>

<div class="container">
  <img src="img_5terre_wide.jpg" alt="Cinque Terre" width="1000" height="300">
  <div class="topleft">Top Left</div>
</div>

</body>
</html>


Rasmning yuqori o'ng pozitsiyasi:

<!DOCTYPE html>
<html>
<head>
<style>
.container {
  position: relative;
}

.topright {
  position: absolute;
  top: 8px;
  right: 16px;
  font-size: 18px;
}

img { 
  width: 100%;
  height: auto;
  opacity: 0.3;
}
</style>
</head>
<body>

<h2>Matni rasm</h2>

<p>Yuqori o'ng burchakdagi rasmga bir oz matn qo'shing:</p>

<div class="container">
  <img src="img_5terre_wide.jpg" alt="Cinque Terre" width="1000" height="300">
  <div class="topright">Yuqori O'ng</div>
</div>

</body>
</html>


Pastki chap rasm holati:

<!DOCTYPE html>
<html>
<head>
<style>
.container {
  position: relative;
}

.bottomleft {
  position: absolute;
  bottom: 8px;
  left: 16px;
  font-size: 18px;
}

img { 
  width: 100%;
  height: auto;
  opacity: 0.3;
}
</style>
</head>
<body>

<h2>Matni rasm</h2>

<p>Pastki chap burchakdagi rasmga bir oz matn qo'shing:</p>

<div class="container">
  <img src="img_5terre_wide.jpg" alt="Cinque Terre" width="1000" height="300">
  <div class="bottomleft">Pasgi chap</div>
</div>

</body>
</html>



Pastki o'ng rasm holati:


<!DOCTYPE html>
<html>
<head>
<style>
.container {
  position: relative;
}

.bottomright {
  position: absolute;
  bottom: 8px;
  right: 16px;
  font-size: 18px;
}

img { 
  width: 100%;
  height: auto;
  opacity: 0.3;
}
</style>
</head>
<body>

<h2>Matni rasm</h2>

<p>Pastki chap burchakdagi rasmga bir oz matn qo'shing:</p>

<div class="container">
  <img src="img_5terre_wide.jpg" alt="Cinque Terre" width="1000" height="300">
  <div class="bottomright">Pasgi o'ng</div>
</div>

</body>
</html>




Markaziy rasm holati:

<!DOCTYPE html>
<html>
<head>
<style>
.container {
  position: relative;
}

.center {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  font-size: 18px;
}

img { 
  width: 100%;
  height: auto;
  opacity: 0.3;
}
</style>
</head>
<body>

<h2>Matnli rasm</h2>

<p>Rasmdagi matnni markazlashtiring:</p>

<div class="container">
  <img src="img_5terre_wide.jpg" alt="Cinque Terre" width="1000" height="300">
  <div class="center">Markazlashtirilgan</div>
</div>

</body>
</html>




Rasm Filtrlari

CSS filtri xususiyati elementga vizual effektlarni (loyqalik va to'yinganlik kabi) qo'shadi.

Eslatma: filtr xususiyati Internet Explorer yoki Edge 12-da mavjud emas.



Misol

Barcha rasmlarning rangini qora va oq rangga o'zgartiring (100% gray):
img {
  filter: grayscale(100%);
} 


<!DOCTYPE html>
<html>
<head>
<style>
img {
  width: 33%;
  height: auto;
  float: left; 
  max-width: 235px;
}

.blur {filter: blur(4px);}
.brightness {filter: brightness(250%);}
.contrast {filter: contrast(180%);}
.grayscale {filter: grayscale(100%);}
.huerotate {filter: hue-rotate(180deg);}
.invert {filter: invert(100%);}
.opacity {filter: opacity(50%);}
.saturate {filter: saturate(7);}
.sepia {filter: sepia(100%);}
.shadow {filter: drop-shadow(8px 8px 10px green);}
</style>
</head>
<body>

<h2>Image Filters</h2>

<p><strong>Note:</strong>Filtr xususiyati Internet Explorer yoki Edge 12-da qo'llab-quvvatlanmaydi.</p>

<img src="pineapple.jpg" alt="Pineapple" width="300" height="300">
<img class="blur" src="pineapple.jpg" alt="Pineapple" width="300" height="300">
<img class="brightness" src="pineapple.jpg" alt="Pineapple" width="300" height="300">
<img class="contrast" src="pineapple.jpg" alt="Pineapple" width="300" height="300">
<img class="grayscale" src="pineapple.jpg" alt="Pineapple" width="300" height="300">
<img class="huerotate" src="pineapple.jpg" alt="Pineapple" width="300" height="300">
<img class="invert" src="pineapple.jpg" alt="Pineapple" width="300" height="300">
<img class="opacity" src="pineapple.jpg" alt="Pineapple" width="300" height="300">
<img class="saturate" src="pineapple.jpg" alt="Pineapple" width="300" height="300">
<img class="sepia" src="pineapple.jpg" alt="Pineapple" width="300" height="300">
<img class="shadow" src="pineapple.jpg" alt="Pineapple" width="300" height="300">

</body>
</html>


Rasm Hover Qoplamasi

Hover-da qoplama effektini yarating:


Matndagi Fade bilan rasm:


<!DOCTYPE html>
<html>
<head>
<style>
.container {
  position: relative;
  width: 50%;
}

.image {
  display: block;
  width: 100%;
  height: auto;
}

.overlay {
  position: absolute;
  top: 0;
  bottom: 0;
  left: 0;
  right: 0;
  height: 100%;
  width: 100%;
  opacity: 0;
  transition: .5s ease;
  background-color: #008CBA;
}

.container:hover .overlay {
  opacity: 1;
}

.text {
  color: white;
  font-size: 20px;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  -ms-transform: translate(-50%, -50%);
}
</style>
</head>
<body>

<h2>Qoplamada so'nish</h2>

<div class="container">
  <img src="img_avatar.png" alt="Avatar" class="image">
  <div class="overlay">
    <div class="text">Salom Dunyo</div>
  </div>
</div>

</body>
</html>



O'chirilgan rasm-qutida:

<!DOCTYPE html>
<html>
<head>
<style>
.container {
  position: relative;
  width: 50%;
}

.image {
  opacity: 1;
  display: block;
  width: 100%;
  height: auto;
  transition: .5s ease;
  backface-visibility: hidden;
}

.middle {
  transition: .5s ease;
  opacity: 0;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  -ms-transform: translate(-50%, -50%)
}

.container:hover .image {
  opacity: 0.3;
}

.container:hover .middle {
  opacity: 1;
}

.text {
  background-color: #4CAF50;
  color: white;
  font-size: 16px;
  padding: 16px 32px;
}
</style>
</head>
<body>

<h2>Fade in a Box</h2>

<div class="container">
  <img src="img_avatar.png" alt="Avatar" class="image" style="width:100%">
  <div class="middle">
    <div class="text">John Doe</div>
  </div>
</div>
  
</body>
</html>



Yuqoridan siljigan matnli rasm:


<!DOCTYPE html>
<html>
<head>
<style>
.container {
  position: relative;
  width: 50%;
}

.image {
  display: block;
  width: 100%;
  height: auto;
}

.overlay {
  position: absolute;
  bottom: 100%;
  left: 0;
  right: 0;
  background-color: #008CBA;
  overflow: hidden;
  width: 100%;
  height: 0;
  transition: .5s ease;
}

.container:hover .overlay {
  bottom: 0;
  height: 100%;
}

.text {
  white-space: nowrap; 
  color: white;
  font-size: 20px;
  position: absolute;
  overflow: hidden;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  -ms-transform: translate(-50%, -50%);
}
</style>
</head>
<body>

<h2>Yuqoridan tepaga suring</h2>

<div class="container">
  <img src="img_avatar.png" alt="Avatar" class="image">
  <div class="overlay">
    <div class="text">Salom Dunyo</div>
  </div>
</div>
 
</body>
</html>



Pastki qismdan siljigan qoplamali rasm:

<!DOCTYPE html>
<html>
<head>
<style>
.container {
  position: relative;
  width: 50%;
}

.image {
  display: block;
  width: 100%;
  height: auto;
}

.overlay {
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
  background-color: #008CBA;
  overflow: hidden;
  width: 100%;
  height: 0;
  transition: .5s ease;
}

.container:hover .overlay {
  height: 100%;
}

.text {
  white-space: nowrap; 
  color: white;
  font-size: 20px;
  position: absolute;
  overflow: hidden;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  -ms-transform: translate(-50%, -50%);
}
</style>
</head>
<body>

<h2>Pastdan yuqoriga suring</h2>

<div class="container">
  <img src="img_avatar.png" alt="Avatar" class="image">
  <div class="overlay">
    <div class="text">Salom Dunyo</div>
  </div>
</div>

</body>
</html>


Chapdan siljigan qoplamali rasm:

<!DOCTYPE html>
<html>
<head>
<style>
.container {
  position: relative;
  width: 50%;
}

.image {
  display: block;
  width: 100%;
  height: auto;
}

.overlay {
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
  background-color: #008CBA;
  overflow: hidden;
  width: 0;
  height: 100%;
  transition: .5s ease;
}

.container:hover .overlay {
  width: 100%;
}

.text {
  white-space: nowrap; 
  color: white;
  font-size: 20px;
  position: absolute;
  overflow: hidden;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  -ms-transform: translate(-50%, -50%);
}
</style>
</head>
<body>

<h2>Chapdan qoplamaga suring</h2>

<div class="container">
  <img src="img_avatar.png" alt="Avatar" class="image">
  <div class="overlay">
    <div class="text">Salom dunyo</div>
  </div>
</div>

</body>
</html>



O'ngdan siljigan qoplamali rasm:


<!DOCTYPE html>
<html>
<head>
<style>
.container {
  position: relative;
  width: 50%;
}

.image {
  display: block;
  width: 100%;
  height: auto;
}

.overlay {
  position: absolute;
  bottom: 0;
  left: 100%;
  right: 0;
  background-color: #008CBA;
  overflow: hidden;
  width: 0;
  height: 100%;
  transition: .5s ease;
}

.container:hover .overlay {
  width: 100%;
  left: 0;
}

.text {
  white-space: nowrap; 
  color: white;
  font-size: 20px;
  position: absolute;
  overflow: hidden;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  -ms-transform: translate(-50%, -50%);
}
</style>
</head>
<body>

<h2>O'ngdan tepaga suring</h2>

<div class="container">
  <img src="img_avatar.png" alt="Avatar" class="image">
  <div class="overlay">
    <div class="text">Salom Dunyo</div>
  </div>
</div>

</body>
</html>




Sichqoncha ko'rsatgichini uning ustiga siljitganda aylanadigan rasm yarating:

<!DOCTYPE html>
<html>
<head>
<style>
img:hover {
  transform: scaleX(-1);
}
</style>
</head>
<body>

<h2>Rasmni aylantirish</h2>
<p>Sichqonchani rasm ustiga siljiting.</p>

<img src="paris.jpg" alt="Paris" width="400" height="300">

</body>
</html>




Ta'sirchan Rasmlar Galereyasi

CSS rasm galereyasini yaratish uchun ishlatilishi mumkin. Ushbu misol rasmlarni qayta tartibga solish uchun media so'rovlaridan foydalanadi 

turli xil ekran o'lchamlari. Effektni ko'rish uchun brauzer oynasining o'lchamini o'zgartiring:


<!DOCTYPE html>
<html>
<head>
<style>
div.gallery {
  border: 1px solid #ccc;
}

div.gallery:hover {
  border: 1px solid #777;
}

div.gallery img {
  width: 100%;
  height: auto;
}

div.desc {
  padding: 15px;
  text-align: center;
}

* {
  box-sizing: border-box;
}

.responsive {
  padding: 0 6px;
  float: left;
  width: 24.99999%;
}

@media only screen and (max-width: 700px) {
  .responsive {
    width: 49.99999%;
    margin: 6px 0;
  }
}

@media only screen and (max-width: 500px) {
  .responsive {
    width: 100%;
  }
}

.clearfix:after {
  content: "";
  display: table;
  clear: both;
}
</style>
</head>
<body>

<h2>Ta'sirchan Rasmlar Galereyasi</h2>

<h4>Effektni ko'rish uchun brauzer oynasining o'lchamini o'zgartiring.</h4>

<div class="responsive">
  <div class="gallery">
    <a target="_blank" href="img_5terre.jpg">
      <img src="img_5terre.jpg" alt="Cinque Terre" width="600" height="400">
    </a>
    <div class="desc">Bu erda rasmning tavsifini qo'shing</div>
  </div>
</div>


<div class="responsive">
  <div class="gallery">
    <a target="_blank" href="img_forest.jpg">
      <img src="img_forest.jpg" alt="Forest" width="600" height="400">
    </a>
    <div class="desc">Bu erda rasmning tavsifini qo'shing</div>
  </div>
</div>

<div class="responsive">
  <div class="gallery">
    <a target="_blank" href="img_lights.jpg">
      <img src="img_lights.jpg" alt="Northern Lights" width="600" height="400">
    </a>
    <div class="desc">Bu erda rasmning tavsifini qo'shing</div>
  </div>
</div>

<div class="responsive">
  <div class="gallery">
    <a target="_blank" href="img_mountains.jpg">
      <img src="img_mountains.jpg" alt="Mountains" width="600" height="400">
    </a>
    <div class="desc">Bu erda rasmning tavsifini qo'shing</div>
  </div>
</div>

<div class="clearfix"></div>

<div style="padding:6px;">
  <p>Ushbu misol turli xil ekran o'lchamidagi rasmlarni qayta tartibga solish uchun media so'rovlaridan foydalanadi: kattaroq ekranlar uchun 

kengligi 700PX dan ortiq, u to'rtta tasvirni yonma-yon ko'rsatadi, 700PX dan kichik ekranlar uchun ikkitasini ko'rsatadi 

tasvirlar yonma-yon. 500px dan kichik ekranlar uchun tasvirlar vertikal ravishda to'planadi (100%).</p>
  <p>Media so'rovlari va sezgir veb-dizayn haqida keyinroq CSS qo'llanmamizda bilib olasiz.</p>
</div>

</body>
</html>



Rasm Modali (Kengaytirilgan)

Bu CSS va JavaScript-ning birgalikda ishlashini namoyish etish uchun misol.

Birinchidan, modal oyna (dialog oynasi) yaratish uchun CSS-dan foydalaning va uni sukut bo'yicha yashiring.

Keyin, modal Oynani ko'rsatish va modal ichidagi tasvirni ko'rsatish uchun JavaScript-dan foydalaning 

rasmni bosish:


<!DOCTYPE html>
<html>
<head>
<style>
#myImg {
  border-radius: 5px;
  cursor: pointer;
  transition: 0.3s;
}

#myImg:hover {opacity: 0.7;}

/* The Modal (background) */
.modal {
  display: none; /* Hidden by default */
  position: fixed; /* Stay in place */
  z-index: 1; /* Sit on top */
  padding-top: 100px; /* Location of the box */
  left: 0;
  top: 0;
  width: 100%; /* Full width */
  height: 100%; /* Full height */
  overflow: auto; /* Enable scroll if needed */
  background-color: rgb(0,0,0); /* Fallback color */
  background-color: rgba(0,0,0,0.9); /* Black w/ opacity */
}

/* Modal Content (image) */
.modal-content {
  margin: auto;
  display: block;
  width: 80%;
  max-width: 700px;
}

/* Caption of Modal Image */
#caption {
  margin: auto;
  display: block;
  width: 80%;
  max-width: 700px;
  text-align: center;
  color: #ccc;
  padding: 10px 0;
  height: 150px;
}

/* Add Animation */
.modal-content, #caption {  
  animation-name: zoom;
  animation-duration: 0.6s;
}

@keyframes zoom {
  from {transform: scale(0.1)} 
  to {transform: scale(1)}
}

/* The Close Button */
.close {
  position: absolute;
  top: 15px;
  right: 35px;
  color: #f1f1f1;
  font-size: 40px;
  font-weight: bold;
  transition: 0.3s;
}

.close:hover,
.close:focus {
  color: #bbb;
  text-decoration: none;
  cursor: pointer;
}

/* 100% Image Width on Smaller Screens */
@media only screen and (max-width: 700px){
  .modal-content {
    width: 100%;
  }
}
</style>
</head>
<body>

<h2>Rasm Modali</h2>

<p>Bu erda biz sukut bo'yicha yashiringan modal (dialog oynasi) yaratish uchun CSS-dan foydalanamiz.</p>
<p>Modalni ishga tushirish va modal ichidagi joriy tasvirni ko'rsatish uchun JavaScript-dan foydalanamiz 

ustiga bosing. Shuni ham unutmangki, biz rasmning "alt" atributidagi qiymatni rasm sarlavhasi matni sifatida ishlatamiz 

model.</p>
<p>Agar siz kodni darhol tushunmasangiz, tashvishlanmang. CSS - ni tugatgandan so'ng, bizning-ga o'ting 

JavaScript Tutorial ko'proq ma'lumot olish uchun.</p>

<img id="myImg" src="img_lights.jpg" alt="Northern Lights, Norway" width="300" height="200">

<!-- The Modal -->
<div id="myModal" class="modal">
  <span class="close">&times;</span>
  <img class="modal-content" id="img01">
  <div id="caption"></div>
</div>

<script>
// Get the modal
var modal = document.getElementById('myModal');

// Get the image and insert it inside the modal - use its "alt" text as a caption
var img = document.getElementById('myImg');
var modalImg = document.getElementById("img01");
var captionText = document.getElementById("caption");
img.onclick = function(){
  modal.style.display = "block";
  modalImg.src = this.src;
  captionText.innerHTML = this.alt;
}

// Get the <span> element that closes the modal
var span = document.getElementsByClassName("close")[0];

// When the user clicks on <span> (x), close the modal
span.onclick = function() { 
  modal.style.display = "none";
}
</script>

</body>
</html>

<kbd>qaytish</kbd>[Back to table of contents](#homepage)\

## CSS ob'ektiga mos


CSS ob'ektga mos xususiyat


CSS object-fit xususiyati <img> yoki <video> o'lchamini unga mos ravishda qanday o'zgartirish kerakligini belgilash uchun ishlatiladi 

konteyner.


Ushbu xususiyat tarkibni konteynerni turli yo'llar bilan to'ldirishni aytadi; "bu jihatni saqlab qolish" kabi 

nisbat"yoki" cho'zing va iloji boricha ko'proq joy oling".


200*300 pikselli konteynerga mos keladigan tasvirni siqish (asl tomonlar nisbati yo'q qilingan holda)

<!DOCTYPE html>
<html>
<head>
<style>
img {
  width:200px;
  height:300px;
}
</style>
</head>
<body>

<h2>Image</h2>
<img src="paris.jpg" alt="Paris" width="400" height="300">

</body>
</html>

Object-fit sizga tomonlar nisbati bo'yicha afzalliklaringizni o'zgartirishga yordam beradi



Object-fit xususiyati quyidagi qiymatlardan birini olishi mumkin:

    fill - Bu sukut bo'yicha. Berilgan o'lchamni to'ldirish uchun rasm hajmi o'zgartiriladi. Agar kerak bo'lsa, rasm bo'ladi

moslash uchun cho'zing yoki siqib qo'ying
    contain - Rasm tomonlar nisbatini saqlaydi, lekin o'lchamlari berilgan o'lchamga mos ravishda o'zgartiriladi
    cover - Rasm tomonlar nisbatini saqlaydi va berilgan o'lchamni to'ldiradi. Rasm mos ravishda kesiladi
    none - Rasm o'lchami o'zgartirilmagan
    scale-down - rasm none yoki contactning eng kichik versiyasiga qadar kichraytirilgan



Object-fit-dan foydalanish: cover;

Agar biz object-fit-dan foydalansak: cover; rasm tomonlarning nisbatlarini saqlaydi va berilgan o'lchamni to'ldiradi. Rasm bo'ladi 

moslash uchun kesib oling:


<!DOCTYPE html>
<html>
<head>
<style>
img {
  width: 200px;
  height: 300px;
  object-fit: cover;
}
</style>
</head>
<body>

<h2>object-fit dan foydalanish: cover</h2>

<img src="paris.jpg" alt="Paris" width="400" height="300">

</body>
</html>



Object-fit dan foydalanish: contain;

Agar biz foydalansak object-fit: o'z ichiga oladi; rasm tomonlar nisbatini saqlaydi, lekin berilgan o'lchamga mos ravishda o'zgartiriladi 

hajmi:

<!DOCTYPE html>
<html>
<head>
<style>
img {
  width: 200px;
  height: 300px;
  object-fit: contain;
}
</style>
</head>
<body>

<h2>Object-fit dan foydalanish: contain</h2>

<img src="paris.jpg" alt="Paris" width="400" height="300">

</body>
</html>



object-fit dan foydalanish: fill;

Agar biz object-fit: fill dan foydalansak; berilgan o'lchamni to'ldirish uchun rasm o'lchami o'zgartiriladi. Agar kerak bo'lsa, rasm bo'ladi 

moslash uchun cho'zing yoki siqib qo'ying:


<!DOCTYPE html>
<html>
<head>
<style>
img {
  width: 200px;
  height: 300px;
  object-fit: fill;
}
</style>
</head>
<body>

<h2>Object-fit-dan foydalanish: to'ldirish</h2>

<img src="paris.jpg" alt="Paris" width="400" height="300">

</body>
</html>



Ob'ektdan foydalanish-mos: yo'q;

Agar biz object-fit-dan foydalansak: yo'q; rasm hajmi o'zgartirilmagan:

<!DOCTYPE html>
<html>
<head>
<style>
img {
  width: 200px;
  height: 300px;
  object-fit: none;
}
</style>
</head>
<body>

<h2>Ob'ektdan foydalanish-mos: yo'q</h2>

<img src="paris.jpg" alt="Paris" width="400" height="300">

</body>
</html>


Object-fit foydalanish: scale-pastga;

Agar biz object-fit-dan foydalansak: masshtab-pastga; rasm eng kichik versiyasiga qadar kichraytirilgan yo'q yoki o'z ichiga oladi:


<!DOCTYPE html>
<html>
<head>
<style>
img {
  width: 200px;
  height: 300px;
  object-fit: scale-down;
}
</style>
</head>
<body>

<h2>Object-fit foydalanish: scale-pastga</h2>

<img src="paris.jpg" alt="Paris" width="400" height="300">

</body>
</html>



Yana Bir Misol

Bu erda bizda ikkita rasm bor va biz ularning brauzer oynasining 50% va 100% kengligini to'ldirishini xohlaymiz 

balandligi.

Quyidagi misolda biz object-fit-dan foydalanmaymiz, shuning uchun brauzer oynasining o'lchamini o'zgartirganda 

tasvirlar yo'q qilinadi:


<!DOCTYPE html>
<html>
<body>

<h2>Object-fit-dan foydalanmaslik</h2>

<p>Bu erda biz "object-fit" dan foydalanmaymiz, shuning uchun brauzer oynasining o'lchamini o'zgartirganda, rasmlarning tomonlar nisbati 

yo'q qilinadi:</p>

<div style="width:100%;height:400px;">
  <img src="rock600x400.jpg" alt="Norway" style="float:left;width:50%;height:100%;">
  <img src="paris.jpg" alt="Paris" style="float:left;width:50%;height:100%;">
</div>

</body>
</html>


Keyingi misolda biz object-fit: cover; dan foydalanamiz, shuning uchun brauzer oynasining o'lchamini o'zgartirganda 

tasvirlar saqlanadi:


<!DOCTYPE html>
<html>
<body>

<h2>Object-fit-dan foydalanish</h2>

<p>Bu erda biz "object-fit: cover;" dan foydalanamiz, shuning uchun brauzer oynasining o'lchamini o'zgartirganda, rasmlarning tomonlar nisbati 

saqlangan:</p>

<div style="width:100%;height:400px;">
  <img src="rock600x400.jpg" alt="Norway" style="float:left;width:50%;height:100%;object-fit:cover;">
  <img src="paris.jpg" alt="Paris" style="float:left;width:50%;height:100%;object-fit:cover;">
</div>

</body>
</html>




CSS ob'ekt-fit ko'proq misollar

Quyidagi misol bitta misolda object-fit xususiyatining barcha mumkin bo'lgan qiymatlarini ko'rsatadi:


<!DOCTYPE html>
<html>
<head>
<style>
.fill {object-fit: fill;}
.contain {object-fit: contain;}
.cover {object-fit: cover;}
.scale-down {object-fit: scale-down;}
.none {object-fit: none;}
</style>
</head>
<body>

<h1>Object-fit xususiyati</h1>

<h2>Ob'ektga mos kelmaydi:</h2>
<img src="paris.jpg" alt="Paris" style="width:200px;height:300px">

<h2>ob'ektni moslash: to'ldirish (bu standart):</h2>
<img class="fill" src="paris.jpg" alt="Paris" style="width:200px;height:300px">

<h2>ob'ekt-fit: o'z ichiga oladi:</h2>
<img class="contain" src="paris.jpg" alt="Paris" style="width:200px;height:300px">

<h2>ob'ektga mos: qopqoq:</h2>
<img class="cover" src="paris.jpg" alt="Paris" style="width:200px;height:300px">

<h2>ob'ektga mos: masshtab pastga:</h2>
<img class="scale-down" src="paris.jpg" alt="Paris" style="width:200px;height:300px">

<h2>ob'ekt-mos: yo'q:</h2>
<img class="none" src="paris.jpg" alt="Paris" style="width:200px;height:300px">

</body>
</html>



CSS ob'ekti - * xususiyatlari

Quyidagi jadvalda CSS ob'ekti-* xususiyatlari keltirilgan:
Mulk Tavsifi
object-fit qanday qilib belgilaydi <rasm> yoki <video> uning konteyneriga mos ravishda o'lchamini o'zgartirish kerak
ob'ekt pozitsiyasi qanday qilib belgilaydi < img > yoki < video > bilan joylashtirilishi kerak x/y koordinatalari uning ichida "o'z tarkib qutisi"

<kbd>qaytish</kbd>[Back to table of contents](#homepage)

## CSS ob'ektining joylashuvi

CSS ob'ekt-pozitsiya xususiyati

CSS object-position xususiyati uning ichida < img> yoki < video> qanday joylashishini aniqlash uchun ishlatiladi 

konteyner.



Object-position xususiyatidan foydalanish

Aytaylik, rasmning ko'rsatilgan qismi biz xohlagan tarzda joylashtirilmagan. Tasvirni joylashtirish uchun biz 

object-position xususiyatidan foydalanadi.

Bu erda biz tasvirni buyuk eski bino ichida bo'lishi uchun joylashtirish uchun object-position xususiyatidan foydalanamiz 

markaz:


<!DOCTYPE html>
<html>
<head>
<style>
img {
  width: 200px;
  height: 300px;
  object-fit: cover;
  object-position: 80% 100%;
}
</style>
</head>
<body>

<h2>CSS ob'ektining joylashuvi</h2>

<p>Bu erda biz tasvirni buyuk eski bino ichida bo'lishi uchun joylashtirish uchun object-position xususiyatidan foydalanamiz 

markaz:</p>

<img src="paris.jpg" alt="Paris" width="400" height="300">

</body>
</html>



Bu erda biz tasvirni mashhur ko'z minorasi joylagan qilib joylash uchun ob'ekt-pozitsiya xususiyatdan foydalanamiz 

Markaziy:

<!DOCTYPE html>
<html>
<head>
<style>
img {
  width: 200px;
  height: 300px;
  object-fit: cover;
  object-position: 15% 100%;
}
</style>
</head>
<body>

<h2>Ob'ekt pozitsiyasidan foydalanish</h2>

<p>Bu erda biz tasvirni mashhur Eyfel minorasi joylashgan qilib joylashtirish uchun object-position xususiyatidan foydalanamiz 

markaz:</p>

<img src="paris.jpg" alt="Paris" width="400" height="300">

</body>
</html>



CSS ob'ekti - * xususiyatlari

Quyidagi jadvalda CSS ob'ekti-* xususiyatlari keltirilgan:
Mulk Tavsifi
object-fit qanday qilib belgilaydi <image> yoki <video> uning konteyneriga mos ravishda o'lchamini o'zgartirish kerak
ob'ekt pozitsiyasi <img> yoki < video> ichida x/y koordinatalari bilan qanday joylashishi kerakligini belgilaydi 

uning "o'z tarkib qutisi"

<kbd>qaytish</kbd>[Back to table of contents](#homepage)

## CSS tugmalari

Ushbu bob CSS-dagi uslub tugmalari haqida. Asosiy tugma uslubi quyida ko'rsatilgan:

<!DOCTYPE html>
<html>
<head>
<style>
.button {
  background-color: #4CAF50;
  border: none;
  color: white;
  padding: 15px 32px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 16px;
  margin: 4px 2px;
  cursor: pointer;
}
</style>
</head>
<body>

<h2>CSS tugmalari</h2>

<button>Andoza Tugma</button>
<a href="#" class="button">Bog'lanish Tugmasi</a>
<button class="button">Tugma</button>
<input type="button" class="button" value="Input Button">

</body>
</html>



Tugma ranglari

Tugmaning fon rangini o'zgartirish uchun fon-rang xususiyatidan foydalaning:


<!DOCTYPE html>
<html>
<head>
<style>
.button {
  background-color: #4CAF50; /* Green */
  border: none;
  color: white;
  padding: 15px 32px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 16px;
  margin: 4px 2px;
  cursor: pointer;
}

.button2 {background-color: #008CBA;} /* Blue */
.button3 {background-color: #f44336;} /* Red */ 
.button4 {background-color: #e7e7e7; color: black;} /* Gray */ 
.button5 {background-color: #555555;} /* Black */
</style>
</head>
<body>

<h2>Tugma ranglari</h2>

<p>Fon rangi xususiyati bilan tugmachaning fon rangini o'zgartiring:</p>

<button class="button">Yashil</button>
<button class="button button2">Ko'k</button>
<button class="button button3">Qizil</button>
<button class="button button4">kulrang</button>
<button class="button button5">Qora</button>

</body>
</html>


Tugma o'lchamlari:

Tugma shrift hajmini o'zgartirish uchun font-size xususiyatidan foydalaning:


<!DOCTYPE html>
<html>
<head>
<style>
.button {
  background-color: #4CAF50; /* Green */
  border: none;
  color: white;
  padding: 15px 32px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  margin: 4px 2px;
  cursor: pointer;
}

.button1 {font-size: 10px;}
.button2 {font-size: 12px;}
.button3 {font-size: 16px;}
.button4 {font-size: 20px;}
.button5 {font-size: 24px;}
</style>
</head>
<body>

<h2>Tugma o'lchamlari:</h2>

<p>Font-size xususiyati bilan tugmachaning shrift hajmini o'zgartiring:</p>

<button class="button button1">10px</button>
<button class="button button2">12px</button>
<button class="button button3">16px</button>
<button class="button button4">20px</button>
<button class="button button5">24px</button>

</body>
</html>


Tugmani to'ldirishni o'zgartirish uchun to'ldirish xususiyatidan foydalaning:

<!DOCTYPE html>
<html>
<head>
<style>
.button {
  background-color: #4CAF50; /* Green */
  border: none;
  color: white;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 16px;
  margin: 4px 2px;
  cursor: pointer;
}

.button1 {padding: 10px 24px;}
.button2 {padding: 12px 28px;}
.button3 {padding: 14px 40px;}
.button4 {padding: 32px 16px;}
.button5 {padding: 16px;}
</style>
</head>
<body>

<h2>Tugmani To'ldirish</h2>

<p>Tugmani to'ldirishni to'ldirish xususiyati bilan o'zgartiring:</p>

<button class="button button1">10px 24px</button>
<button class="button button2">12px 28px</button>
<button class="button button3">14px 40px</button>
<button class="button button4">32px 16px</button>
<button class="button button5">16px</button>

</body>
</html>



Yumaloq Tugmalar
Tugmaga yumaloq burchaklarni qo'shish uchun chegara-radius xususiyatidan foydalaning:


<!DOCTYPE html>
<html>
<head>
<style>
.button {
  background-color: #4CAF50; /* Green */
  border: none;
  color: white;
  padding: 20px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 16px;
  margin: 4px 2px;
  cursor: pointer;
}

.button1 {border-radius: 2px;}
.button2 {border-radius: 4px;}
.button3 {border-radius: 8px;}
.button4 {border-radius: 12px;}
.button5 {border-radius: 50%;}
</style>
</head>
<body>

<h2>Yumaloq Tugmalar</h2>

<p>Border-radius xususiyatiga ega tugmachaga yumaloq burchaklarni qo'shing:</p>

<button class="button button1">2px</button>
<button class="button button2">4px</button>
<button class="button button3">8px</button>
<button class="button button4">12px</button>
<button class="button button5">50%</button>

</body>
</html>



Rangli Tugma Chegaralari

Tugmaga rangli chegara qo'shish uchun chegara xususiyatidan foydalaning:

<!DOCTYPE html>
<html>
<head>
<style>
.button {
  background-color: #4CAF50; /* Green */
  border: none;
  color: white;
  padding: 15px 32px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 16px;
  margin: 4px 2px;
  cursor: pointer;
}

.button1 {
  background-color: white; 
  color: black; 
  border: 2px solid #4CAF50;
}

.button2 {
  background-color: white; 
  color: black; 
  border: 2px solid #008CBA;
}

.button3 {
  background-color: white; 
  color: black; 
  border: 2px solid #f44336;
}

.button4 {
  background-color: white;
  color: black;
  border: 2px solid #e7e7e7;
}

.button5 {
  background-color: white;
  color: black;
  border: 2px solid #555555;
}
</style>
</head>
<body>

<h2>Rangli Tugma Chegaralari</h2>

<p>Tugmaga chegara qo'shish uchun chegara xususiyatidan foydalaning:</p>

<button class="button button1">Yashil</button>
<button class="button button2">Ko'k</button>
<button class="button button3">Qizil</button>
<button class="button button4">Kulurang</button>
<button class="button button5">Qora</button>

</body>
</html>




Hoverable Tugmalari

Sichqonchani ustiga siljitganda tugma uslubini o'zgartirish uchun: hover selektoridan foydalaning.

Maslahat: "hover" effektining tezligini aniqlash uchun o'tish davomiyligi xususiyatidan foydalaning:



<!DOCTYPE html>
<html>
<head>
<style>
.button {
  background-color: #4CAF50; /* Green */
  border: none;
  color: white;
  padding: 16px 32px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 16px;
  margin: 4px 2px;
  transition-duration: 0.4s;
  cursor: pointer;
}

.button1 {
  background-color: white; 
  color: black; 
  border: 2px solid #4CAF50;
}

.button1:hover {
  background-color: #4CAF50;
  color: white;
}

.button2 {
  background-color: white; 
  color: black; 
  border: 2px solid #008CBA;
}

.button2:hover {
  background-color: #008CBA;
  color: white;
}

.button3 {
  background-color: white; 
  color: black; 
  border: 2px solid #f44336;
}

.button3:hover {
  background-color: #f44336;
  color: white;
}

.button4 {
  background-color: white;
  color: black;
  border: 2px solid #e7e7e7;
}

.button4:hover {background-color: #e7e7e7;}

.button5 {
  background-color: white;
  color: black;
  border: 2px solid #555555;
}

.button5:hover {
  background-color: #555555;
  color: white;
}
</style>
</head>
<body>

<h2>Hoverable Tugmalari</h2>

<p>sichqonchani uning ustiga siljitganda tugma uslubini o'zgartirish uchun :hover selektoridan foydalaning.</p>
<p><strong>maslahat:</strong> "hover"tezligini aniqlash uchun o'tish davomiyligi xususiyatidan foydalaning 

ta'siri:</p>

<button class="button button1">Yashil</button>
<button class="button button2">Ko'k</button>
<button class="button button3">Qizil</button>
<button class="button button4">Kulurang</button>
<button class="button button5">Qora</button>

</body>
</html>



Soya Tugmalari

Tugmaga soyalar qo'shish uchun box-soya xususiyatidan foydalaning:

<!DOCTYPE html>
<html>
<head>
<style>
.button {
  background-color: #4CAF50; /* Green */
  border: none;
  color: white;
  padding: 15px 32px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 16px;
  margin: 4px 2px;
  cursor: pointer;
  -webkit-transition-duration: 0.4s; /* Safari */
  transition-duration: 0.4s;
}

.button1 {
  box-shadow: 0 8px 16px 0 rgba(0,0,0,0.2), 0 6px 20px 0 rgba(0,0,0,0.19);
}

.button2:hover {
  box-shadow: 0 12px 16px 0 rgba(0,0,0,0.24),0 17px 50px 0 rgba(0,0,0,0.19);
}
</style>
</head>
<body>

<h2>Soya Tugmalari</h2>

<p>Tugmaga soyalar qo'shish uchun box-soya xususiyatidan foydalaning:</p>

<button class="button button1">Soya Tugmalari</button>
<button class="button button2">Hoverdagi soya</button>

</body>
</html>



O'chirilgan Tugmalar

Tugmaga shaffoflikni qo'shish uchun opacity xususiyatidan foydalaning ("o'chirilgan" ko'rinishni yaratadi).

Maslahat: bundan tashqari, bir "yo'q mashinalar" namoyish etadi "emas-ruxsat", bir qiymati bilan kursor mulkni qo'shishingiz mumkin 

sichqoncha tugmachasini bosganingizda" belgisi:


<!DOCTYPE html>
<html>
<head>
<style>
.button {
  background-color: #4CAF50; /* Green */
  border: none;
  color: white;
  padding: 15px 32px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 16px;
  margin: 4px 2px;
  cursor: pointer;
}

.disabled {
  opacity: 0.6;
  cursor: not-allowed;
}
</style>
</head>
<body>

<h2>O'chirilgan Tugma</h2>

<p>Tugmaga shaffoflikni qo'shish uchun shaffoflik xususiyatidan foydalaning (uni o'chirib qo'ying):</p>

<button class="button">Oddiy Tugma</button>
<button class="button disabled">O'chirilgan Tugma</button>

</body>
</html>



Tugma Kengligi

Odatiy bo'lib, tugmachaning o'lchami uning matn tarkibi bilan belgilanadi (uning mazmuni kabi keng). Kenglikdan foydalaning 

tugma kengligini o'zgartirish xususiyati:


<!DOCTYPE html>
<html>
<head>
<style>
.button {
  background-color: #4CAF50; /* Green */
  border: none;
  color: white;
  padding: 15px 32px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 16px;
  margin: 4px 2px;
  cursor: pointer;
}

.button1 {width: 250px;}
.button2 {width: 50%;}
.button3 {width: 100%;}
</style>
</head>
<body>

<h2>Tugma Kengliklarini O'rnating</h2>

<p>Tugma kengligini o'zgartirish uchun kenglik xususiyatidan foydalaning:</p>

<button class="button button1">250px</button><br>
<button class="button button2">50%</button><br>
<button class="button button3">100%</button>

<p><strong>Tip:</strong> Ruxsat etilgan kenglikni o'rnatmoqchi bo'lsangiz va sezgir tugmalar uchun foizdan foydalansangiz, piksellardan foydalaning 

(masalan, uning asosiy elementi 50%). Effektni ko'rish uchun brauzer oynasining o'lchamini o'zgartiring.</p>

</body>
</html>


Tugma guruhlari (navigatsiya paneliga o'xshaydi)

Chegaralarni olib tashlang va float qo'shing:tugmalar guruhini yaratish uchun har bir tugmaga chap:



<!DOCTYPE html>
<html>
<head>
<style>
.btn-group .button {
  background-color: #4CAF50; /* Green */
  border: none;
  color: white;
  padding: 15px 32px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 16px;
  cursor: pointer;
  float: left;
}

.btn-group .button:hover {
  background-color: #3e8e41;
}
</style>
</head>
<body>

<h2>Tugma Guruhlari</h2>

<p>Tugmalar guruhini yaratish uchun chekkalarni olib tashlang va tugmachalarni suzib oling:</p>

<div class="btn-group">
  <button class="button">Tugma</button>
  <button class="button">Tugma</button>
  <button class="button">Tugma</button>
  <button class="button">Tugma</button>
</div>

<p style="clear:both"><br>Keyin floatlarni tozalashni unutmang, aks holda bu p element ham yonida suzadimi 

tugmalar.</p>

</body>
</html>



Chegarali tugmalar guruhi (chegaralari bo'lgan navbarga o'xshash)

Chegarali tugmalar guruhini yaratish uchun chegara xususiyatidan foydalaning:

<!DOCTYPE html>
<html>
<head>
<style>
.btn-group .button {
  background-color: #4CAF50; /* Green */
  border: 1px solid green;
  color: white;
  padding: 15px 32px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 16px;
  cursor: pointer;
  float: left;
}

.btn-group .button:not(:last-child) {
  border-right: none; /* Prevent double borders */
}

.btn-group .button:hover {
  background-color: #3e8e41;
}
</style>
</head>
<body>

<h2>Chegaralangan Tugmalar Guruhi</h2>

<p>Chegarali tugmalar guruhini yaratish uchun chegaralarni qo'shing:</p>

<div class="btn-group">
  <button class="button">Tugma</button>
  <button class="button">Tugma</button>
  <button class="button">Tugma</button>
  <button class="button">Tugma</button>
</div>

<p style="clear:both"><br>Keyin floatlarni tozalashni unutmang, aks holda bu p element ham yonida suzadimi 

tugmalar.</p>

</body>
</html>


Vertikal Tugmalar Guruhi

Displeydan foydalaning:float o'rniga bloklash: yonma-yon emas, bir-birining ostidagi tugmalarni guruhlash uchun chapda:

<!DOCTYPE html>
<html>
<head>
<style>
.btn-group .button {
  background-color: #4CAF50; /* Green */
  border: 1px solid green;
  color: white;
  padding: 15px 32px;
  text-align: center;
  text-decoration: none;
  font-size: 16px;
  cursor: pointer;
  width: 150px;
  display: block;
}

.btn-group .button:not(:last-child) {
  border-bottom: none; /* Prevent double borders */
}

.btn-group .button:hover {
  background-color: #3e8e41;
}
</style>
</head>
<body>

<h2>Vertikal Tugmalar Guruhi</h2>

<div class="btn-group">
  <button class="button">Tugma</button>
  <button class="button">Tugma</button>
  <button class="button">Tugma</button>
  <button class="button">Tugma</button>
</div>

</body>
</html>



Rasmdagi tugma:


<!DOCTYPE html>
<html>
<head>
<style>
.container {
  position: relative;
  width: 100%;
  max-width: 400px;
}
Rasmdagi tugmani qo'shing:
.container img {
  width: 100%;
  height: auto;
}Rasmdagi tugmani qo'shing:


.container .btn {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  -ms-transform: translate(-50%, -50%);
  background-color: #f1f1f1;
  color: black;
  font-size: 16px;
  padding: 16px 30px;
  border: none;
  cursor: pointer;
  border-radius: 5px;
  text-align: center;
}

.container .btn:hover {
  background-color: black;
  color: white;
}
</style>
</head>
<body>

<h2>Rasmdagi tugma:</h2>

<p>Rasmdagi tugmani qo'shing:</p>

<div class="container">
  <img src="img_lights.jpg" alt="Snow" style="width:100%">
  <button class="btn">Tugma</button>
</div>

</body>
</html>



Animatsion Tugmalar
Misol

Hover-ga o'q qo'shing:


<!DOCTYPE html>
<html>
<head>
<style>
.button {
  display: inline-block;
  border-radius: 4px;
  background-color: #f4511e;
  border: none;
  color: #FFFFFF;
  text-align: center;
  font-size: 28px;
  padding: 20px;
  width: 200px;
  transition: all 0.5s;
  cursor: pointer;
  margin: 5px;
}

.button span {
  cursor: pointer;
  display: inline-block;
  position: relative;
  transition: 0.5s;
}

.button span:after {
  content: '\00bb';
  position: absolute;
  opacity: 0;
  top: 0;
  right: -20px;
  transition: 0.5s;
}

.button:hover span {
  padding-right: 25px;
}

.button:hover span:after {
  opacity: 1;
  right: 0;
}
</style>
</head>
<body>

<h2>Animatsion Tugmalar</h2>

<button class="button" style="vertical-align:middle"><span>Hover </span></button>

</body>
</html>







  Bosish ustiga" bosilgan " effekt qo'shing:

<!DOCTYPE html>
<html>
<head>
<style>
.button {
  display: inline-block;
  padding: 15px 25px;
  font-size: 24px;
  cursor: pointer;
  text-align: center;
  text-decoration: none;
  outline: none;
  color: #fff;
  background-color: #4CAF50;
  border: none;
  border-radius: 15px;
  box-shadow: 0 9px #999;
}

.button:hover {background-color: #3e8e41}

.button:active {
  background-color: #3e8e41;
  box-shadow: 0 5px #666;
  transform: translateY(4px);
}
</style>
</head>
<body>

<h2>Animatsion Tugma - "Bosilgan Effekt"</h2>

<button class="button">Meni Bosing</button>

</body>
</html>




Hover ustida Fade:

<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>
.button {
  background-color: #f4511e;
  border: none;
  color: white;
  padding: 16px 32px;
  text-align: center;
  font-size: 16px;
  margin: 4px 2px;
  opacity: 0.6;
  transition: 0.3s;
  display: inline-block;
  text-decoration: none;
  cursor: pointer;
}

.button:hover {opacity: 1}
</style>
</head>
<body>

<h2>Animatsiyali tugma-Fade kuchga kiradi</h2>

<button class="button">Kursorni Ustimga Olib Boring</button>

</body>
</html>



Bosish ustiga" ripple " effektini qo'shing:


<!DOCTYPE html>
<html>
<head>
<style>
.button {
  position: relative;
  background-color: #4CAF50;
  border: none;
  font-size: 28px;
  color: #FFFFFF;
  padding: 20px;
  width: 200px;
  text-align: center;
  transition-duration: 0.4s;
  text-decoration: none;
  overflow: hidden;
  cursor: pointer;
}

.button:after {
  content: "";
  background: #f1f1f1;
  display: block;
  position: absolute;
  padding-top: 300%;
  padding-left: 350%;
  margin-left: -20px !important;
  margin-top: -120%;
  opacity: 0;
  transition: all 0.8s
}

.button:active:after {
  padding: 0;
  margin: 0;
  opacity: 1;
  transition: 0s
}
</style>
</head>
<body>

<h2>Animatsion Tugma-Ripple Effekti</h2>

<button class="button">Meni Bosing</button>

</body>
</html>

<kbd>qaytish</kbd>[Back to table of contents](#homepage)

## CSS Pagination


Ushbu bob sizga CSS-da sezgir paginatsiyani qanday yaratishni ko'rsatib beradi.



Oddiy Sahifalash

Agar sizda ko'plab sahifalarga ega veb-saytingiz bo'lsa, har bir sahifaga qandaydir sahifalash qo'shishingiz mumkin:


<!DOCTYPE html>
<html>
<head>
<style>
.pagination {
  display: inline-block;
}

.pagination a {
  color: black;
  float: left;
  padding: 8px 16px;
  text-decoration: none;
}
</style>
</head>
<body>

<h2>Oddiy Sahifalash</h2>

<div class="pagination">
  <a href="#">&laquo;</a>
  <a href="#">1</a>
  <a href="#">2</a>
  <a href="#">3</a>
  <a href="#">4</a>
  <a href="#">5</a>
  <a href="#">6</a>
  <a href="#">&raquo;</a>
</div>

</body>
</html>



Faol va Hoverable Pagination

Joriy sahifani an bilan belgilang .faol sinf va har birining rangini o'zgartirish uchun :hover selektoridan foydalaning 

sichqonchani ularning ustiga siljitganda sahifa havolasi:


<!DOCTYPE html>
<html>
<head>
<style>
.pagination {
  display: inline-block;
}

.pagination a {
  color: black;
  float: left;
  padding: 8px 16px;
  text-decoration: none;
}

.pagination a.active {
  background-color: #4CAF50;
  color: white;
}

.pagination a:hover:not(.active) {background-color: #ddd;}
</style>
</head>
<body>

<h2>faol va Hoverable Pagination </h2>

<p>sichqonchani raqamlar ustiga suring.</p>

<div class="pagination">
  <a href="#">&laquo;</a>
  <a href="#">1</a>
  <a class="active" href="#">2</a>
  <a href="#">3</a>
  <a href="#">4</a>
  <a href="#">5</a>
  <a href="#">6</a>
  <a href="#">&raquo;</a>
</div>

</body>
</html>




Dumaloq faol va boshqariladigan tugmalar

Agar siz yumaloq "faol" va "hover" tugmachasini xohlasangiz, chegara-radius xususiyatini qo'shing:

<!DOCTYPE html>
<html>
<head>
<style>
.pagination {
  display: inline-block;
}

.pagination a {
  color: black;
  float: left;
  padding: 8px 16px;
  text-decoration: none;
}

.pagination a.active {
  background-color: #4CAF50;
  color: white;
  border-radius: 5px;
}

.pagination a:hover:not(.active) {
  background-color: #ddd;
  border-radius: 5px;
}
</style>
</head>
<body>

<h2>Dumaloq faol va Hover tugmalari</h2>

<div class="pagination">
  <a href="#">&laquo;</a>
  <a href="#">1</a>
  <a href="#" class="active">2</a>
  <a href="#">3</a>
  <a href="#">4</a>
  <a href="#">5</a>
  <a href="#">6</a>
  <a href="#">&raquo;</a>
</div>

</body>
</html>



Hoverable O'tish Effekti

Hover-da o'tish effektini yaratish uchun o'tish xususiyatini sahifa havolalariga qo'shing:

<!DOCTYPE html>
<html>
<head>
<style>
.pagination {
  display: inline-block;
}

.pagination a {
  color: black;
  float: left;
  padding: 8px 16px;
  text-decoration: none;
  transition: background-color .3s;
}

.pagination a.active {
  background-color: #4CAF50;
  color: white;
}

.pagination a:hover:not(.active) {background-color: #ddd;}
</style>
</head>
<body>

<h2>Hoverga o'tish effekti</h2>

<p>Sichqonchani raqamlar ustiga siljiting.</p>

<div class="pagination">
  <a href="#">&laquo;</a>
  <a href="#">1</a>
  <a href="#" class="active">2</a>
  <a href="#">3</a>
  <a href="#">4</a>
  <a href="#">5</a>
  <a href="#">6</a>
  <a href="#">&raquo;</a>
</div>

</body>
</html>




Chegaralangan Paginatsiya

Paginatsiyaga chegaralarni qo'shish uchun chegara xususiyatidan foydalaning:


<!DOCTYPE html>
<html>
<head>
<style>
.pagination {
  display: inline-block;
}

.pagination a {
  color: black;
  float: left;
  padding: 8px 16px;
  text-decoration: none;
  transition: background-color .3s;
  border: 1px solid #ddd;
}

.pagination a.active {
  background-color: #4CAF50;
  color: white;
  border: 1px solid #4CAF50;
}

.pagination a:hover:not(.active) {background-color: #ddd;}
</style>
</head>
<body>

<h2>Chegaralar bilan sahifalash</h2>

<div class="pagination">
  <a href="#">&laquo;</a>
  <a href="#">1</a>
  <a href="#" class="active">2</a>
  <a href="#">3</a>
  <a href="#">4</a>
  <a href="#">5</a>
  <a href="#">6</a>
  <a href="#">&raquo;</a>
</div>

</body>
</html>



Yumaloq Chegaralar

Maslahat: sahifadagi birinchi va oxirgi havolaga yumaloq chegaralarni qo'shing:


<!DOCTYPE html>
<html>
<head>
<style>
.pagination {
  display: inline-block;
}

.pagination a {
  color: black;
  float: left;
  padding: 8px 16px;
  text-decoration: none;
  border: 1px solid #ddd;
}

.pagination a.active {
  background-color: #4CAF50;
  color: white;
  border: 1px solid #4CAF50;
}

.pagination a:hover:not(.active) {background-color: #ddd;}

.pagination a:first-child {
  border-top-left-radius: 5px;
  border-bottom-left-radius: 5px;
}

.pagination a:last-child {
  border-top-right-radius: 5px;
  border-bottom-right-radius: 5px;
}
</style>
</head>
<body>

<h2>Dumaloq chegaralar bilan sahifalash</h2>

<div class="pagination">
  <a href="#">&laquo;</a>
  <a href="#">1</a>
  <a class="active" href="#">2</a>
  <a href="#">3</a>
  <a href="#">4</a>
  <a href="#">5</a>
  <a href="#">6</a>
  <a href="#">&raquo;</a>
</div>

</body>
</html>



Havolalar Orasidagi Bo'shliq

Maslahat: agar sahifa havolalarini guruhlashni xohlamasangiz, margin xususiyatini qo'shing:


<!DOCTYPE html>
<html>
<head>
<style>
.pagination {
  display: inline-block;
}

.pagination a {
  color: black;
  float: left;
  padding: 8px 16px;
  text-decoration: none;
  transition: background-color .3s;
  border: 1px solid #ddd;
  margin: 0 4px;
}

.pagination a.active {
  background-color: #4CAF50;
  color: white;
  border: 1px solid #4CAF50;
}

.pagination a:hover:not(.active) {background-color: #ddd;}
</style>
</head>
<body>

<h2>Chegaralar bilan sahifalash;</h2>

<div class="pagination">
  <a href="#">&laquo;</a>
  <a href="#">1</a>
  <a href="#" class="active">2</a>
  <a href="#">3</a>
  <a href="#">4</a>
  <a href="#">5</a>
  <a href="#">6</a>
  <a href="#">&raquo;</a>
</div>

</body>
</html>



Paginatsiya Hajmi

Shrift o'lchami xususiyati bilan sahifalash hajmini o'zgartiring:

<!DOCTYPE html>
<html>
<head>
<style>
.pagination {
  display: inline-block;
}

.pagination a {
  color: black;
  float: left;
  padding: 8px 16px;
  text-decoration: none;
  transition: background-color .3s;
  border: 1px solid #ddd;
  font-size: 22px;
}

.pagination a.active {
  background-color: #4CAF50;
  color: white;
  border: 1px solid #4CAF50;
}

.pagination a:hover:not(.active) {background-color: #ddd;}
</style>
</head>
<body>

<h2>Paginatsiya Hajmi</h2>

<p>Paginatsiyani kichikroq yoki kattaroq qilish uchun shrift o'lchami xususiyatini o'zgartiring.</p>

<div class="pagination">
  <a href="#">&laquo;</a>
  <a href="#">1</a>
  <a href="#" class="active">2</a>
  <a href="#">3</a>
  <a href="#">4</a>
  <a href="#">5</a>
  <a href="#">6</a>
  <a href="#">&raquo;</a>
</div>

</body>
</html>



Markazlashtirilgan Sahifalash

Sahifalashni markazlashtirish uchun konteyner elementini (<div> kabi) uning atrofiga matnni tekislash:markaz bilan o'rab qo'ying


<!DOCTYPE html>
<html>
<head>
<style>
.center {
  text-align: center;
}

.pagination {
  display: inline-block;
}

.pagination a {
  color: black;
  float: left;
  padding: 8px 16px;
  text-decoration: none;
  transition: background-color .3s;
  border: 1px solid #ddd;
  margin: 0 4px;
}

.pagination a.active {
  background-color: #4CAF50;
  color: white;
  border: 1px solid #4CAF50;
}

.pagination a:hover:not(.active) {background-color: #ddd;}
</style>
</head>
<body>

<h2>Markazlashtirilgan Sahifalash</h2>

<div class="center">
  <div class="pagination">
  <a href="#">&laquo;</a>
  <a href="#">1</a>
  <a href="#" class="active">2</a>
  <a href="#">3</a>
  <a href="#">4</a>
  <a href="#">5</a>
  <a href="#">6</a>
  <a href="#">&raquo;</a>
  </div>
</div>

</body>
</html>

