## HTML CHARSE
HTML belgilar to'plami atributi:
HTML sahifani to'g'ri ko'rsatish uchun veb-brauzer sahifada ishlatiladigan belgilar to'plamini bilishi kerak.

```
<meta charset="UTF-8">
```
agar siz belgilar to'plamini ko'rsatmasangiz, "UTF-8" HTMLda standart hisoblanadi.


UTF-8 belgilar: Siz ularni klaviaturada yoza olmaysiz, lekin ular har doim raqamlar (shaxs raqamlari) yordamida ko'rsatilishi mumkin.

* Quyidagi xatboshidagi ```<p>``` ikkalasi ham bir xil
```
<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
</head>
<tana>

<p>Men A B C</p> ko'rsataman
<p>Men &#65; &#66; &#67;</p>

</body>
</html>
```
* A, B, C mos ravishda 65, 66 va 67

Brauzerga utf-8 belgisini ko'rsatayotganingizni tan olishi uchun &# dan boshlashingiz va uni nuqtali vergul (;) bilan tugatishingiz kerak.

Emojilar ham utf-8 belgilaridir.

* Siz boshqa belgilar kabi kulgichlarni oʻlchashingiz mumkin
```
<p style="font-size:48px">
&#128512; &#128516; &#128525; &#128151;
</p>
```
* HTML kodlash (belgilar to'plami)

Brauzer uni to'g'ri ko'rsatish uchun foydalanadigan belgilar to'plamini bilishi kerak.

** HTML kodlash bobidan parchalar
ASCII dan UTF-8 ga

ASCII belgilarni kodlashning birinchi standarti edi. ASCII Internetda ishlatilishi mumkin bo'lgan 128 xil belgini aniqladi: raqamlar (0-9), ingliz harflari (A-Z) va ba'zi maxsus belgilar kabi ! $ + - ( ) @ < > .

ISO-8859-1 HTML 4 uchun standart belgilar toʻplami edi. Bu belgilar toʻplami 256 xil belgilar kodini qoʻllab-quvvatlagan. HTML 4 ham UTF-8 ni qo'llab-quvvatladi.

ANSI (Windows-1252) asl Windows belgilar to'plami edi. ANSI ISO-8859-1 bilan bir xil, faqat ANSIda 32 ta qoʻshimcha belgilar mavjud.

HTML5 spetsifikatsiyasi veb-ishlab chiquvchilarni dunyodagi deyarli barcha belgilar va belgilarni qamrab oluvchi UTF-8 belgilar to'plamidan foydalanishga undaydi!

** HTML belgilar to'plami atributi
uni HTML sahifasining <meta> tegida ko'rsatasiz.

```
<meta charset="UTF-8">
```
<kbd>qaytish</kbd>[Mundarijaga qaytish](#homepage)


-------



## HTML shakllari

* Foydalanuvchi nomi va parolni o'z ichiga olgan va serverlar kiritilgan ma'lumotlarni qayta ishlagandan so'ng shaklni ma'lum bir sahifaga yo'naltiruvchi shaklni to'ldirish.
```
<h2>HTML shakllari</h2>

<form action="/action_page.php">
   <label for="fname">Ism:</label><br>
   <input type="text" id="fname" name="fname" value="Jon"><br>
   <label for="lname">Familiya:</label><br>
   <input type="text" id="lname" name="lname" value="Doe"><br><br>
   <input type="submit" value="yuborish">
</form>

<p>Agar siz “Yuborish” tugmasini bossangiz, forma maʼlumotlari “/action_page.php” deb nomlangan sahifaga yuboriladi.</p>
```

* ```<form>``` elementi

HTML ```<form>``` elementi foydalanuvchi kiritishi uchun HTML formasini yaratish uchun ishlatiladi:
```
<form>

shakl elementlari

</form>
```

Shakl elementi barcha turdagi kiritish elementlari uchun konteynerga o'xshaydi, masalan: matn maydonlari, tasdiqlash qutilari, radio tugmalari, yuborish tugmalari va boshqalar.


* ```<input>``` elementi: eng ko`p qo`llaniladigan shakl elementi bo`lib, uni 'type' atributida ko`rsatish mumkin.
```
Turi Tavsif
<input type="text"> Bir qatorli matn kiritish maydonini ko'rsatadi
<input type="radio"> Radio tugmani ko'rsatadi (ko'p variantlardan birini tanlash uchun)
<input type="checkbox"> Belgilash katakchasini ko'rsatadi (ko'p variantlardan nol yoki undan ko'pni tanlash uchun)
<input type="submit"> Yuborish tugmachasini ko'rsatadi (shaklni yuborish uchun)
<input type="button"> Bosiladigan tugmani ko'rsatadi
```

* Matn maydonlari: ```<kiritish turi="matn"> ```

Bu matn kiritish uchun bitta qatorli kiritish maydonini belgilaydi. Shaklning o'zi ko'rinmaydi va belgilar soni sukut bo'yicha 20 belgidan iborat.
```
<form>
   <label for="fname">Ism:</label><br>
   <input type="text" id="fname" name="fname"><br>
   <label for="lname">Familiya:</label><br>
   <input type="text" id="lname" name="lname">
</form>
```
```<label>``` tegi ko`p shakl elementlari uchun yorliqni belgilaydi.

```<label>``` elementi ekranni o`qiydigan foydalanuvchilar uchun foydalidir, chunki foydalanuvchi asosiy e`tiborni kiritish elementiga qaratganda ekran o`quvchi yorliqni baland ovozda o`qiydi.

```<label>``` elementi juda kichik hududlarni (masalan, radio tugmalar yoki belgilash katakchalari) bosishda qiynalayotgan foydalanuvchilarga ham yordam beradi - chunki foydalanuvchi ```<label>``` elementidagi matnni bosganda , u radio tugmachasini/tasdiqlash qutisini almashtiradi.

```<label>``` tegining for atributi ularni bir-biriga bog`lash uchun <input> elementining id atributiga teng bo`lishi kerak.
* Radio Buttons
```
<input type="radio"> defines the radio button which lets use select ONLY one among a few choices.
```
* see sample radio buttons below:
```
<form>
  <input type="radio" id="male" name="gender" value="male">
  <label for="male">Male</label><br>
  <input type="radio" id="female" name="gender" value="female">
  <label for="female">Female</label><br>
  <input type="radio" id="other" name="gender" value="other">
  <label for="other">Other</label>
</form> 
```

* Checkboxes: Enables users select zero or more among a limited no of choices 
```
<input type="checkbox"> defines a checkbox
```
NB: the value attribute  can indicate the default option
 
* See example of form below:
```
<form>
  <input type="checkbox" id="vehicle1" name="vehicle1" value="Bike">
  <label for="vehicle1"> I have a bike</label><br>
  <input type="checkbox" id="vehicle2" name="vehicle2" value="Car">
  <label for="vehicle2"> I have a car</label><br>
  <input type="checkbox" id="vehicle3" name="vehicle3" value="Boat">
  <label for="vehicle3"> I have a boat</label>
</form> 
```

* The Submit Button
```
<input type="submit"> defines the button for submitting form data to a form-handler. 
```
Example of a form with a submit button below: 
```
<form action="/action_page.php">
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname" value="John"><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname" value="Doe"><br><br>
  <input type="submit" value="Submit">
</form> 
```

* he Name Attribute for ```<input>```
* Each input field must have a name to be submitted. If the value of the name attribute is omitted, the input field value will not be sent at all. 

<kbd>return</kbd>[Back to table of contents](#homepage)

## HTML formasi atributlari

* HTML formasi atributi: turli atributlar muhokamasi

Harakat atributi: ariza topshirilganda bajarilishi kerak bo'lgan harakatni belgilaydi. Shakl ma'lumotlari odatda yuborish tugmasi bosilganda serverdagi faylga yuboriladi. Agar harakat atributini o'tkazib yuborsangiz, amal joriy sahifaga o'rnatiladi.

* Shakl ma'lumotlarini forma ma'lumotlarini boshqaradigan server tomonidagi skriptni o'z ichiga olgan action_page.php nomli faylga yuborish uchun:
```
<form action="/action_page.php">
   <label for="fname">Ism:</label><br>
   <input type="text" id="fname" name="fname" value="Jon"><br>
   <label for="lname">Familiya:</label><br>
   <input type="text" id="lname" name="lname" value="Doe"><br><br>
   <input type="submit" value="yuborish">
</form>
```

* Maqsad atributi
Bu shaklni yuborgandan so'ng olingan javobni qayerda ko'rsatishni ko'rsatdi.

Maqsad atributining mumkin bo'lgan qiymatlari uchun pastga qarang

Qiymat tavsifi
```
_blank Javob yangi oyna yoki yorliqda ko'rsatiladi
_self Javob joriy oynada ko'rsatiladi (standart)
_parent Javob ota-ramada ko'rsatiladi
_top Javob oynaning to'liq qismida ko'rsatiladi
framename Javob nomli iframe-da ko'rsatiladi
```
* Maqsad atributidan foydalanishga misol:
```
<p>Ushbu shaklni yuborishda natija brauzerning yangi sahifasida ochiladi:</p>

<form action="/action_page.php" target="_blank">
   <label for="fname">Ism:</label><br>
   <input type="text" id="fname" name="fname" value="Jon"><br>
   <label for="lname">Familiya:</label><br>
   <input type="text" id="lname" name="lname" value="Doe"><br><br>
   <input type="submit" value="yuborish">
</form>
```

* Metod atributi

Bu usul atributi shakl ma'lumotlarini yuborishda ishlatiladigan HTTP usulini belgilaydi.

* Get usuli: ```<form action="/action_page.php" method="get"> ```
* Xabar berish usuli: ```<form action="/action_page.php" method="post"> ```

* Maslahat: Agar forma maʼlumotlarida maxfiy yoki shaxsiy maʼlumotlar boʻlsa, har doim POST-dan foydalaning!

GET bo'yicha eslatmalar:
Shakl ma'lumotlarini URL manziliga nom/qiymat juftliklarida qo'shadi
Nozik ma'lumotlarni yuborish uchun HECH QACHON GET dan foydalanmang! (yuborilgan shakl ma'lumotlari URL manzilida ko'rinadi!)
URL uzunligi cheklangan (2048 belgi)
Foydalanuvchi natijani belgilamoqchi bo'lgan shakllarni yuborish uchun foydalidir
GET xavfsiz bo'lmagan ma'lumotlar uchun yaxshi, masalan, Google so'rovlari qatorlari

POST haqida eslatmalar:
Form ma'lumotlarini HTTP so'rovining asosiy qismiga qo'shadi (yuborilgan shakl ma'lumotlari URLda ko'rsatilmaydi)
POST-da o'lcham cheklovlari yo'q va katta hajmdagi ma'lumotlarni yuborish uchun ishlatilishi mumkin.
POST bilan yuborilgan arizalarni xatcho‘p qilib bo‘lmaydi

Maslahat: Agar forma ma'lumotlarida maxfiy yoki shaxsiy ma'lumotlar bo'lsa, har doim POST dan foydalaning!

* Avtomatik to'ldirish atributi
Shaklda avtomatik toʻldirishni yoqish yoki oʻchirish kerakligini belgilaydi. Avtomatik to‘ldirish yoqilgan bo‘lsa, brauzerda bir xil brauzerda avval kiritilgan qiymatlar asosida qiymatlarni avtomatik ravishda to‘ldirish imkonini beradi.
```
<form action="/action_page.php" autocomplete="on">
```

Novalidate atributi
Bu mantiqiy atribut bo'lib, ariza ma'lumotlari (kiritish) yuborilganda tasdiqlanmasligi kerak.
```
<form action="/action_page.php" novalidate>
```
* Barcha <form> atributlari ro'yxati

```
Atribut tavsifi
accept-charset Shaklni yuborish uchun ishlatiladigan belgilar kodlashlarini belgilaydi
harakat Shakl topshirilganda forma ma'lumotlarini qaerga yuborish kerakligini belgilaydi
avtoto'ldirish Shaklda avtomatik to'ldirishni yoqish yoki o'chirish kerakligini belgilaydi
enctype Form ma'lumotlarini serverga yuborishda qanday kodlash kerakligini belgilaydi (faqat method="post" uchun)
Metod Form ma'lumotlarini yuborishda foydalanish uchun HTTP usulini belgilaydi
nom Shakl nomini bildiradi
novalidate Shakl topshirilganda tasdiqlanmasligi kerakligini bildiradi
rel Bog'langan manba va joriy hujjat o'rtasidagi munosabatni belgilaydi
maqsad Shaklni yuborgandan so'ng olingan javobni qayerda ko'rsatishni belgilaydi
```
<kbd>qaytish</kbd>[Mundarijaga qaytish](#homepage)


------
## HTML formasi atributlari

* HTML formasi atributi: turli atributlar muhokamasi

Harakat atributi: ariza topshirilganda bajarilishi kerak bo'lgan harakatni belgilaydi. Shakl ma'lumotlari odatda yuborish tugmasi bosilganda serverdagi faylga yuboriladi. Agar harakat atributini o'tkazib yuborsangiz, amal joriy sahifaga o'rnatiladi.

* Shakl ma'lumotlarini forma ma'lumotlarini boshqaradigan server tomonidagi skriptni o'z ichiga olgan action_page.php nomli faylga yuborish uchun:
```
<form action="/action_page.php">
   <label for="fname">Ism:</label><br>
   <input type="text" id="fname" name="fname" value="Jon"><br>
   <label for="lname">Familiya:</label><br>
   <input type="text" id="lname" name="lname" value="Doe"><br><br>
   <input type="submit" value="yuborish">
</form>
```

* Maqsad atributi
Bu shaklni yuborgandan so'ng olingan javobni qayerda ko'rsatishni ko'rsatdi.

Maqsad atributining mumkin bo'lgan qiymatlari uchun pastga qarang

Qiymat tavsifi
```
_blank Javob yangi oyna yoki yorliqda ko'rsatiladi
_self Javob joriy oynada ko'rsatiladi (standart)
_parent Javob ota-ramada ko'rsatiladi
_top Javob oynaning to'liq qismida ko'rsatiladi
framename Javob nomli iframe-da ko'rsatiladi
```
* Maqsad atributidan foydalanishga misol:
```
<p>Ushbu shaklni yuborishda natija brauzerning yangi sahifasida ochiladi:</p>

<form action="/action_page.php" target="_blank">
   <label for="fname">Ism:</label><br>
   <input type="text" id="fname" name="fname" value="Jon"><br>
   <label for="lname">Familiya:</label><br>
   <input type="text" id="lname" name="lname" value="Doe"><br><br>
   <input type="submit" value="yuborish">
</form>
```

* Metod atributi

Bu usul atributi shakl ma'lumotlarini yuborishda ishlatiladigan HTTP usulini belgilaydi.

* Get usuli: ```<form action="/action_page.php" method="get"> ```
* Xabar berish usuli: ```<form action="/action_page.php" method="post"> ```

* Maslahat: Agar forma maʼlumotlarida maxfiy yoki shaxsiy maʼlumotlar boʻlsa, har doim POST-dan foydalaning!

GET bo'yicha eslatmalar:
Shakl ma'lumotlarini URL manziliga nom/qiymat juftliklarida qo'shadi
Nozik ma'lumotlarni yuborish uchun HECH QACHON GET dan foydalanmang! (yuborilgan shakl ma'lumotlari URL manzilida ko'rinadi!)
URL uzunligi cheklangan (2048 belgi)
Foydalanuvchi natijani belgilamoqchi bo'lgan shakllarni yuborish uchun foydalidir
GET xavfsiz bo'lmagan ma'lumotlar uchun yaxshi, masalan, Google so'rovlari qatorlari

POST haqida eslatmalar:
Form ma'lumotlarini HTTP so'rovining asosiy qismiga qo'shadi (yuborilgan shakl ma'lumotlari URLda ko'rsatilmaydi)
POST-da o'lcham cheklovlari yo'q va katta hajmdagi ma'lumotlarni yuborish uchun ishlatilishi mumkin.
POST bilan yuborilgan arizalarni xatcho‘p qilib bo‘lmaydi

Maslahat: Agar forma ma'lumotlarida maxfiy yoki shaxsiy ma'lumotlar bo'lsa, har doim POST dan foydalaning!

* Avtomatik to'ldirish atributi
Shaklda avtomatik toʻldirishni yoqish yoki oʻchirish kerakligini belgilaydi. Avtomatik to‘ldirish yoqilgan bo‘lsa, brauzerda bir xil brauzerda avval kiritilgan qiymatlar asosida qiymatlarni avtomatik ravishda to‘ldirish imkonini beradi.
```
<form action="/action_page.php" autocomplete="on">
```

Novalidate atributi
Bu mantiqiy atribut bo'lib, ariza ma'lumotlari (kiritish) yuborilganda tasdiqlanmasligi kerak.
```
<form action="/action_page.php" novalidate>
```
* Barcha <form> atributlari ro'yxati

```
Atribut tavsifi
accept-charset Shaklni yuborish uchun ishlatiladigan belgilar kodlashlarini belgilaydi
harakat Shakl topshirilganda forma ma'lumotlarini qaerga yuborish kerakligini belgilaydi
avtoto'ldirish Shaklda avtomatik to'ldirishni yoqish yoki o'chirish kerakligini belgilaydi
enctype Form ma'lumotlarini serverga yuborishda qanday kodlash kerakligini belgilaydi (faqat method="post" uchun)
Metod Form ma'lumotlarini yuborishda foydalanish uchun HTTP usulini belgilaydi
nom Shakl nomini bildiradi
novalidate Shakl topshirilganda tasdiqlanmasligi kerakligini bildiradi
rel Bog'langan manba va joriy hujjat o'rtasidagi munosabatni belgilaydi
maqsad Shaklni yuborgandan so'ng olingan javobni qayerda ko'rsatishni belgilaydi
```
<kbd>qaytish</kbd>[Mundarijaga qaytish](#homepage)


--------
## HTML forma elementlari
HTML ```<form>``` elementlari

HTML <form> elementi quyidagi shakl elementlaridan bir yoki bir nechtasini o'z ichiga olishi mumkin:

```
<kiritish>
<label>
<tanlash>
<textarea>
<tugmasi>
<maydon to'plami>
<legend>
<datalist>
<chiqish>
<opsiya>
<optgroup>
```

* ```<input>``` elementi
Kirish elementi eng ko'p ishlatiladigan shakl elementlaridan biridir. Tur atributiga qarab turli yo'llar bilan ko'rsatilishi mumkin
```
<label for="fname">Ism:</label>
<input type="text" id="fname" name="fname">
```
* ```<label>``` elementi

```<label>``` elementi bir nechta forma elementlari uchun tegni belgilaydi. Foydalanuvchi kirishga e'tibor qaratganda ekranni o'qiydiganlarga yorliqni o'qishga yordam beradi.
Shuningdek, u foydalanuvchilarga kichik hududlar yonidagi matnni (masalan, belgilash katakchalari va tugmalar) bosishda yordam beradi.

```<label>``` tegining 'for' atributi ularni birlashtirish uchun <input> elementining 'id' atributiga teng bo'lishi kerak.

* ```<select>``` elementi

Ushbu element ochiladigan ro'yxatni belgilaydi:
```
<label for="cars">Mashinani tanlang:</label>
<select id="cars" name="cars">
   <option value="volvo">Volvo</option>
   <option value="saab">Saab</option>
   <option value="fiat">Fiat</option>
   <option value="audi">Audi</option>
</select>
```
* Variant elementlari tanlanishi mumkin bo'lgan variantni belgilaydi. Birinchi element sukut bo'yicha tanlanadi. Oldindan tanlangan qilish uchun opsiyaga "tanlangan" atributini qo'shing.
```
<option value="fiat" selected>Fiat</option>
```
* Ko'rinadigan qiymatlar: ko'rinadigan qiymatlar sonini belgilash uchun o'lcham atributidan foydalaning (agar sizda ko'rinadigan qiymatdan ko'proq bo'lsa, kichik aylantirish paneli kiritiladi)
```
<label for="cars">Mashinani tanlang:</label>
<select id="cars" name="cars" size="3">
   <option value="volvo">Volvo</option>
   <option value="saab">Saab</option>
   <option value="fiat">Fiat</option>
   <option value="audi">Audi</option>
</select>
```

* Bir nechta tanlovga ruxsat berish: "bir nechta" atributi foydalanuvchiga bir nechta qiymatlarni tanlash imkonini beradi. Buni ishlatish uchun bir nechta variantni tanlash uchun Ctrl (Windows) / Buyruq (Mac) tugmasini bosib ushlab turishingiz kerak.
```
<label for="cars">Mashinani tanlang:</label>
<select id="cars" name="cars" size="4" bir nechta>
   <option value="volvo">Volvo</option>
   <option value="saab">Saab</option>
   <option value="fiat">Fiat</option>
   <option value="audi">Audi</option>
</select>
```

* ```<textarea>``` elementi
```<textarea>``` elementi ko`p qatorli kiritish maydonini (matn maydoni) belgilaydi:
Satrlar atributi matn maydonidagi satrlarning ko'rinadigan sonini belgilaydi.

Cols atributi matn maydonining ko'rinadigan kengligini belgilaydi.

Yuqoridagi HTML kodi brauzerda shunday ko'rsatiladi:
```
<textarea name="xabar" rows="10" cols="30">
Mushuk bog'da o'ynadi.
</textarea>
```
CSS-dan matn maydoni hajmini aniqlash uchun ham foydalanish mumkin.
```
<textarea name="message" style="width:200px; height:600px;">
Mushuk bog'da o'ynadi.
</textarea>
```

* ```<tugmasi>``` elementi
Bosiladigan tugmani belgilaydi.
```
<button type="button" onclick="alert('Salom Dunyo!')">Menga bosing!</button>
```
Eslatma: Har doim tugma elementi uchun type atributini belgilang. Turli xil brauzerlar tugma elementi uchun har xil standart turlardan foydalanishi mumkin.

* ```<fieldset>``` va ```<legend>``` elementlari

```<fieldset>``` elementi formadagi bog`liq ma`lumotlarni guruhlash uchun ishlatiladi.

```<legend>``` elementi <fieldset> elementi uchun sarlavhani belgilaydi.

```
<form action="/action_page.php">
   <maydon to'plami>
     <legend>Shaxsiy:</legend>
     <label for="fname">Ism:</label><br>
     <input type="text" id="fname" name="fname" value="Jon"><br>
     <label for="lname">Familiya:</label><br>
     <input type="text" id="lname" name="lname" value="Doe"><br><br>
     <input type="submit" value="yuborish">
   </fieldset>
</form>
```

* ```<datalist>``` elementi
```<input>``` elementi uchun oldindan belgilangan variantlar ro`yxatini belgilaydi (matnni kiritganingizdan so`ng tanlashingiz mumkin bo`lgan ro`yxat opsiyalarini avtomatik to`ldirish kabi ishlaydi) Bu oddiy shakl kiritish elementi bilan ishlatilishi mumkin --tajriba.

Foydalanuvchilar ma'lumotlarni kiritishda oldindan belgilangan variantlarning ochiladigan ro'yxatini ko'radilar.

```<input>``` elementining ro`yxat atributi <datalist> elementining id atributiga murojaat qilishi kerak

Safari ning oldingi 12.1 versiyasida maʼlumotlar roʻyxati tegi qoʻllab-quvvatlanmaydi
```
<form action="/action_page.php">
   <input list="brauzerlar">
   <datalist id="brauzerlar">
     <option value="Internet Explorer">
     <option value="Firefox">
     <option value="Chrome">
     <option value="Opera">
     <option value="Safari">
   </datalist>
</form>
```

* ```<output>``` elementi
Hisoblash natijasini takrorlang (masalan, skript tomonidan bajarilgan)

```
<form action="/action_page.php"
   oninput="x.value=parseInt(a.value)+parseInt(b.value)">
   0
   <kiritish turi="diapazon" id="a" nomi="a" qiymati="50">
   100+
   <kiritish turi="raqam" id="b" nomi="b" qiymati="50">
   =
   <output name="x" for="a b"></output>
   <br><br>
   <kiritish turi="yuborish">
</form>
```

** HTML forma elementlari
```
Teg tavsifi
<form> Foydalanuvchi kiritish uchun HTML formasini belgilaydi
<input> Kirish boshqaruvini belgilaydi
<textarea> Ko'p qatorli kiritish boshqaruvini belgilaydi (matn maydoni)
<label> <input> elementi uchun tegni belgilaydi
<fieldset> Shakldagi tegishli elementlarni guruhlaydi
<legend> <fieldset> elementi uchun sarlavhani belgilaydi
<tanlash> Ochiladigan ro'yxatni belgilaydi
<optgroup> Ochiladigan ro'yxatda tegishli variantlar guruhini belgilaydi
<option> Ochiladigan roʻyxatdagi variantni belgilaydi
<button> Bosiladigan tugmani belgilaydi
<datalist> Kirish boshqaruvlari uchun oldindan belgilangan variantlar ro'yxatini belgilaydi
<output> Hisoblash natijasini aniqlaydi
```
<kbd>qaytish</kbd>[Mundarijaga qaytish](#homepage)


------


## HTML kiritish turlari
* HTML kiritish turlari
Standart "matn"
```
<kiritish turi="tugma">
<kiritish turi="checkbox">
<kiritish turi="rang">
<kiritish turi="sana">
<input type="datetime-local">
<kiritish turi="elektron pochta">
<kiritish turi="fayl">
<kiritish turi="yashirin">
<kiritish turi="tasvir">
<kiritish turi="oy">
<kiritish turi="raqam">
<kiritish turi="parol">
<kirish turi="radio">
<kiritish turi="diapazon">
<kiritish turi="qayta tiklash">
<kiritish turi="qidiruv">
<kiritish turi="yuborish">
<kiritish turi="tel">
<kiritish turi="matn">
<kiritish turi="vaqt">
<kiritish turi="url">
<kiritish turi="hafta">
```
Maslahat: type atributining standart qiymati "matn" dir.


* Matnni kiritish turi (standart kenglik = 20 belgi)
```<input type="matn">``` bir qatorli matn kiritish maydonini belgilaydi:

```
<form>
   <label for="fname">Ism:</label><br>
   <input type="text" id="fname" name="fname"><br>
   <label for="lname">Familiya:</label><br>
   <input type="text" id="lname" name="lname">
</form>
```

* Parolni kiritish turi
```
<input type="password"> parol maydonini belgilaydi.Parol maydonidagi belgilar niqoblangan (yulduzcha yoki doira shaklida ko'rsatilgan)

  <form>
   <label for="username">Foydalanuvchi nomi:</label><br>
   <input type="text" id="username" name="foydalanuvchi nomi"><br>
   <label for="pwd">Parol:</label><br>
   <input type="parol" id="pwd" name="pwd">
</form>
```


* kiritish turi Yuborish
```<input type="submit">``` forma ma`lumotlarini forma ishlov beruvchisiga yuborish tugmachasini belgilaydi.

Shakl ishlov beruvchisi odatda kiritilgan ma'lumotlarni qayta ishlash uchun skriptga ega bo'lgan server sahifasidir.

Shakl ishlovchisi shaklning harakat atributida ko'rsatilgan:

Yuborish tugmasining qiymat atributini o‘tkazib yuborsangiz, tugma standart matnni oladi (odatda “So‘rovni yuborish”)
```
  <form action="/action_page.php">
   <label for="fname">Ism:</label><br>
   <input type="text" id="fname" name="fname" value="Jon"><br>
   <label for="lname">Familiya:</label><br>
   <input type="text" id="lname" name="lname" value="Doe"><br><br>
   <input type="submit" value="yuborish">
</form>
```

* Kirish turini tiklash

```<input type="reset">``` barcha shakl qiymatlarini standart qiymatlariga qaytaradigan qayta o'rnatish tugmachasini belgilaydi.: Shuningdek, tugmada ko'rinadigan narsalarni sozlash uchun siz qayta o'rnatish tugmasiga qiymat atributini qo'shishingiz mumkin.
```
<form action="/action_page.php">
   <label for="fname">Ism:</label><br>
   <input type="text" id="fname" name="fname" value="Jon"><br>
   <label for="lname">Familiya:</label><br>
   <input type="text" id="lname" name="lname" value="Doe"><br><br>
   <input type="submit" value="yuborish">
   <kiritish turi="qayta tiklash">
</form>
```

* Kirish turi radio
-Foydalanuvchiga cheklangan miqdordagi tanlovlardan birini tanlash imkonini beruvchi radio tugmani belgilaydi:
```
<form>
   <input type="radio" id="erkak" nomi="jins" qiymati="erkak">
   <label for="male">Erkak</label><br>
   <input type="radio" id="ayol" nomi="jins" qiymati="ayol">
   <label for="female">Ayol</label><br>
   <input type="radio" id="other" name="gender" value="boshqa">
   <label for="other">Boshqa</label>
</form>
```

* Kirish turini belgilash katagi

```<input type="checkbox">``` belgilash katakchasini belgilaydi.

Belgilash katakchalari foydalanuvchiga cheklangan miqdordagi tanlovdan NO yoki KO'PROQ variantlarni tanlash imkonini beradi.
```
<form>
   <input type="checkbox" id="vehicle1" name="vehicle1" value="velosiped">
   <label for="vehicle1"> Mening velosipedim bor</label><br>
   <input type="checkbox" id="vehicle2" name="vehicle2" value="Avtomobil">
   <label for="vehicle2"> Mening mashinam bor</label><br>
   <input type="checkbox" id="vehicle3" name="vehicle3" value="qayiq">
   <label for="vehicle3"> Mening qayig‘im bor</label>
</form>
```
* Kirish turi tugmasi
```<input type="button">``` tugmani belgilaydi:

  ```<input type="button" onclick="alert('Salom Dunyo!')" value="Menga bosing!">```



* Kirish turi Rang
```<input type="color">``` rang bo`lishi kerak bo`lgan kiritish maydonlari uchun ishlatiladi.

Brauzer qo'llab-quvvatlashiga qarab, kiritish maydonida rang tanlash vositasi paydo bo'lishi mumkin.

type="color" Internet Explorer 11 yoki Safari 9.1 (yoki undan oldingi) da qo'llab-quvvatlanmaydi.

Qiymat atributi rang uchun oldindan tanlangan qiymatni belgilaydi.
```
<form>
   <label for="favcolor">Sevimli rangingizni tanlang:</label>
   <input type="color" id="favcolor" name="favcolor" value="#ff0000">
   <input type="submit" value="yuborish">
</form>
```


* Kirish turi sanasi

```<input type="date">``` sanani o`z ichiga olishi kerak bo`lgan kiritish maydonlari uchun ishlatiladi.

Brauzer qo'llab-quvvatlashiga qarab, sanani tanlagich kiritish maydonida paydo bo'lishi mumkin.

type="date" Safari yoki Internet Explorer 11 (yoki undan oldingi) da qo'llab-quvvatlanmaydi
```
<form>
   <label for="birthday">Tug'ilgan kun:</label>
   <input type="sana" id="tug'ilgan kun" name="tug'ilgan kun">
   <input type="submit" value="yuborish">
</form>
```

Shuningdek, sanalarga cheklovlar qo'shish uchun "min" va "maks" atributlarini qo'shishingiz mumkin
```
<form action="/action_page.php">
   <label for="datemax">1980-01-01 dan oldingi sanani kiriting:</label>
   <input type="date" id="datemax" name="datemax" max="1979-12-31"><br><br>

   <label for="datemin">2000-01-01 dan keyingi sanani kiriting:</label>
   <input type="date" id="datemin" name="datemin" min="2000-01-02"><br><br>
  
   <input type="submit" value="yuborish">
</form>
```


* Kirish turi Datetime-mahalliy

```<input type="datetime-local">``` vaqt mintaqasisiz sana va vaqtni kiritish maydonini belgilaydi.

Brauzer qo'llab-quvvatlashiga qarab, sanani tanlagich kiritish maydonida paydo bo'lishi mumkin.
```
<form action="/action_page.php">
   <label for="birthdaytime">Tug'ilgan kun (sana va vaqt):</label>
   <input type="datetime-local" id="birthdaytime" name="birthdaytime">
   <input type="submit" value="yuborish">
</form>
```

* Elektron pochtani kiritish turi

```<input type="email">``` elektron pochta manzili bo`lishi kerak bo`lgan kiritish maydonlari uchun ishlatiladi.

Brauzer qo'llab-quvvatlashiga qarab, elektron pochta manzili yuborilganda avtomatik ravishda tasdiqlanishi mumkin.

Ba'zi smartfonlar elektron pochta turini taniydi va elektron pochta kiritishiga mos kelish uchun klaviaturaga ".com" ni qo'shadi

```
<form action="/action_page.php">
   <label for="email">E-pochta manzilingizni kiriting:</label>
   <input type="email" id="email" name="email">
   <input type="submit" value="yuborish">
</form>
```

* Kirish turi fayli
```<input type="file">``` faylni tanlash maydonini va fayllarni yuklash uchun "Browse" tugmasini belgilaydi.
```
<form action="/action_page.php">
   <label for="myfile">Faylni tanlang:</label>
   <input type="file" id="myfile" name="mening fayl"><br><br>
   <input type="submit" value="yuborish">
</form>
```

* Kirish turi oy
```<input type="month">``` foydalanuvchiga oy va yilni tanlash imkonini beradi.

Brauzer qo'llab-quvvatlashiga qarab, sanani tanlagich kiritish maydonida paydo bo'lishi mumkin.
```
<form action="/action_page.php">
   <label for="bdaymonth">Tug‘ilgan kun (oy va yil):</label>
   <input type="oy" id="bdaymonth" name="bdaymonth">
   <input type="submit" value="yuborish">
</form>
```

* Kirish turi Raqam
```<input type="raqam">``` raqamli kiritish maydonini belgilaydi.

Shuningdek, qanday raqamlar qabul qilinishiga cheklovlar o'rnatishingiz mumkin.

Odatda diapazonlar orasidagi qiymatlarni kamaytirish va oshirish uchun yuqoriga va pastga tugmalarini qo'shadi

Quyidagi misolda 1 dan 5 gacha qiymat kiritishingiz mumkin bo'lgan raqamli kiritish maydoni ko'rsatilgan:
```
<form action="/action_page.php">
   <label for="quantity">Miqdor (1 va 5 orasida):</label>
   <kiritish turi="raqam" id="miqdori" nomi="miqdori" min="1" maksimal="5">
   <input type="submit" value="yuborish">
</form>
```


Kirish cheklovlari

Quyida ba'zi umumiy kirish cheklovlari ro'yxati keltirilgan:
Atribut tavsifi
Belgilangan Sahifa yuklanganda kiritish maydoni oldindan tanlanishi kerakligini bildiradi ( type="checkbox" yoki type="radio" uchun)
disabled Kirish maydonini o'chirib qo'yish kerakligini bildiradi
max Kirish maydoni uchun maksimal qiymatni belgilaydi
maxlength Kirish maydoni uchun belgilarning maksimal sonini belgilaydi
min Kirish maydoni uchun minimal qiymatni belgilaydi
naqsh Kirish qiymatini tekshirish uchun muntazam ifodani belgilaydi
faqat o'qish Kirish maydoni faqat o'qilishini bildiradi (o'zgartirib bo'lmaydi)
zarur Kirish maydoni zarurligini bildiradi (to'ldirilishi kerak)
size Kirish maydonining kengligini (belgilarda) belgilaydi
qadam Kirish maydoni uchun qonuniy raqamlar oralig'ini belgilaydi
qiymat Kirish maydoni uchun standart qiymatni belgilaydi

Keyingi bobda kirish cheklovlari haqida ko'proq bilib olasiz.

Quyidagi misolda siz 0 dan 100 gacha qiymatni 10 bosqichda kiritishingiz mumkin bo'lgan raqamli kiritish maydonini ko'rsatadi. Standart qiymat 30:
```
<form action="/action_page.php">
   <label for="quantity">Miqdor:</label>
   <kiritish turi="raqam" id="miqdori" nomi="miqdori" min="0" max="100" qadam="10" qiymati="30">
   <input type="submit" value="yuborish">
</form>
```

* Kirish turi diapazoni
```<input type="diapazon">``` aniq qiymati muhim bo`lmagan raqamni kiritish uchun boshqaruvni belgilaydi (slayder boshqaruvi kabi). Standart diapazon 0 dan 100 gacha. Biroq min, maks va qadam atributlari bilan qanday raqamlar qabul qilinishiga cheklovlar o‘rnatishingiz mumkin:
```
<form action="/action_page.php" method="get">
   <label for="vol">Ovoz balandligi (0 dan 50 gacha):</label>
   <input type="diapazon" id="vol" name="vol" min="0" max="50">
   <input type="submit" value="yuborish">
</form>
```

* Kirish turini qidirish
```
<form action="/action_page.php">
   <label for="gsearch">Google orqali qidirish:</label>
   <input type="search" id="gsearch" name="gsearch">
   <input type="submit" value="yuborish">
</form>
```
* Kirish turini qidirish
```<input type="tel">``` telefon raqami bo`lishi kerak bo`lgan kiritish maydonlari uchun ishlatiladi.
```
<form action="/action_page.php">
   <label for="phone">Telefon raqamini kiriting:</label><br><br>
   <input type="tel" id="telefon" nomi="telefon" to'ldiruvchisi="123-45-678" naqsh="[0-9]{3}-[0-9]{2}-[0- 9]{3}" kerak <br><br>
   <small>Format: 123-45-678</small><br><br>
   <input type="submit" value="yuborish">
</form>
```

* Kirish turi vaqti

```<input type="time">``` foydalanuvchiga vaqtni tanlash imkonini beradi (vaqt zonasi yo'q).

Brauzer qo'llab-quvvatlashiga qarab, vaqt tanlagichi kiritish maydonida ko'rinishi mumkin.Agar brauzer uni qo'llab-quvvatlasa, kiritish maydoniga kirishda vaqt tanlagichi paydo bo'ladi.
```
<form action="/action_page.php">
   <label for="appt">Vaqtni tanlang:</label>
   <input type="time" id="appt" name="appt">
   <input type="submit" value="yuborish">
</form>
```

* Url kiritish turi

```<input type="url">``` URL manzili bo`lishi kerak bo`lgan kiritish maydonlari uchun ishlatiladi.

Brauzer qo'llab-quvvatlashiga qarab, url maydoni yuborilganda avtomatik ravishda tasdiqlanishi mumkin.

Ba'zi smartfonlar url turini taniydi va url kiritishiga mos kelish uchun klaviaturaga ".com" ni qo'shadi.

```
<form action="/action_page.php">
   <label for="homepage">Bosh sahifangizni qo'shing:</label>
   <input type="url" id="homepage" name="homepage">
   <input type="submit" value="yuborish">
</form>
```
* Kirish turi haftasi
```<input type="hafta">``` foydalanuvchiga hafta va yilni tanlash imkonini beradi.

Brauzer qo'llab-quvvatlashiga qarab, sanani tanlash vositasi kiritish maydonida paydo bo'lishi mumkin.Agar brauzer uni qo'llab-quvvatlasa, kiritish maydoniga kirganda sana tanlagich paydo bo'ladi.
```
<form action="/action_page.php">
   <label for="week">Haftani tanlang:</label>
   <input type="hafta" id="hafta" nomi="hafta">
   <input type="submit" value="yuborish">
</form>
```
<kbd>qaytish</kbd>[Mundarijaga qaytish](#homepage)

## HTML kiritish atributlari

HTML kiritish turi atributi
Teg tavsifi
```<input type="">``` Ko`rsatish uchun kiritish turini belgilaydi

- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
HTML kiritish atributlari: kiritish elementining atributlari

* Qiymat atributi
Import maydoni uchun boshlang'ich (standart) qiymatni belgilaydi
```
<form action="/action_page.php">
   <label for="fname">Ism:</label><br>
   <input type="text" id="fname" name="fname" value="Jon"><br>
   <label for="lname">Familiya:</label><br>
   <input type="text" id="lname" name="lname" value="Doe"><br><br>
   <input type="submit" value="yuborish">
</form>
```

* Faqat o'qish uchun atribut
Faqat o'qish uchun kiritish maydonini belgilaydi. Ushbu kiritish maydonini o'zgartirib bo'lmaydi, lekin foydalanuvchi unga kirishi, matnni ajratib ko'rsatishi va undan nusxa ko'chirishi mumkin. Qiymat shaklni yuborishda yuboriladi.
```
<form action="/action_page.php">
   <label for="fname">Ism:</label><br>
   <input type="text" id="fname" name="fname" value="Jon" faqat o'qish uchun<br>
   <label for="lname">Familiya:</label><br>
   <input type="text" id="lname" name="lname" value="Doe"><br><br>
   <input type="submit" value="yuborish">
</form>
```

* Disabled atributi
Kirish maydoni o'chirilganligi va bunday maydonni ishlatish mumkin emasligi va bosish mumkin emasligi ko'rsatilgan. Shaklni yuborishda qiymat yuborilmaydi.
```
<form action="/action_page.php">
   <label for="fname">Ism:</label><br>
   <input type="text" id="fname" name="fname" value="Jon" o'chirilgan><br>
   <label for="lname">Familiya:</label><br>
   <input type="text" id="lname" name="lname" value="Doe"><br><br>
   <input type="submit" value="yuborish">
</form>
```

* Hajmi atributi

Kirish maydonining belgilar bilan ko'rinadigan kengligini belgilaydi. Standart qiymat 20 oʻlchamdir. Bu atribut Matn, qidiruv, tel, url, elektron pochta va parol bilan ishlaydi.
```
<form action="/action_page.php">
   <label for="fname">Ism:</label><br>
   <input type="text" id="fname" name="fname" size="50"><br>
   <label for="pin">PIN:</label><br>
   <input type="text" id="pin" name="pin" size="4"><br><br>
   <input type="submit" value="yuborish">
</form>
```
* Maksimal uzunlik atributi

Kirish maydonida ruxsat etilgan belgilarning maksimal sonini belgilaydi.

Eslatma: Maksimal uzunlik o'rnatilganda, kiritish maydoni belgilangan belgilar sonidan ko'pini qabul qilmaydi. Biroq, bu atribut hech qanday fikr bildirmaydi. Shunday qilib, agar siz foydalanuvchini ogohlantirmoqchi bo'lsangiz, JavaScript kodini yozishingiz kerak.

```
<form action="/action_page.php">
   <label for="fname">Ism:</label><br>
   <input type="text" id="fname" name="fname" size="50"><br>
   <label for="pin">PIN:</label><br>
   <input type="text" id="pin" name="pin" maxlength="4" size="4"><br><br>
   <input type="submit" value="yuborish">
</form>
```

* Min va Maks atributi
Kirish maydoni uchun minimal va maksimal qiymatlarni belgilaydi. Raqam, diapazon, sana, sana-mahalliy, oy, vaqt va hafta bilan ishlaydi.

Maslahat: Bir qator qonuniy qiymatlarni yaratish uchun maksimal va min atributlaridan birgalikda foydalaning.
```
<form action="/action_page.php">
   <label for="datemax">1980-01-01 dan oldingi sanani kiriting:</label>
   <input type="date" id="datemax" name="datemax" max="1979-12-31"><br><br>

   <label for="datemin">2000-01-01 dan keyingi sanani kiriting:</label>
   <input type="date" id="datemin" name="datemin" min="2000-01-02"><br><br>
  
   <label for="quantity">Miqdor (1 va 5 orasida):</label>
   <kiritish turi="raqam" id="miqdori" nomi="miqdori" min="1" max="5"><br><br>

   <input type="submit" value="yuborish">
</form>
```

* Bir nechta atribut
Foydalanuvchiga kirish maydoniga bir nechta qiymat kiritishga ruxsat berilganligini bildiradi. bir nechta atribut elektron pochta va fayl turlari bilan yaxshi ishlaydi
```
<form action="/action_page.php">
   <label for="files">Fayllarni tanlang:</label>
   <input type="file" id="files" name="fayllar" bir nechta><br><br>
   <input type="submit" value="yuborish">
</form>
```

* Naqsh atributi

Shakl yuborilganda kirish maydonining qiymati tekshiriladigan muntazam ifodalarni belgilaydi. Pattern atributi matn, sana, qidiruv, url, tel, elektron pochta va parol bilan ishlaydi.

Maslahat: foydalanuvchiga yordam berish uchun naqshni tasvirlash uchun global sarlavha atributidan foydalaning.

Maslahat: Muntazam iboralar haqida koʻproq maʼlumotni JavaScript qoʻllanmamizda oʻrganing.

```
<form action="/action_page.php">
   <label for="country_code">Mamlakat kodi:</label>
   <input type="text" id="mamlakat_kodi" nomi="mamlakat_kodi" naqsh="[A-Za-z]{3}" title="Uch harfli mamlakat kodi"><br><br>
   <input type="submit" value="yuborish">
</form>
```

* To'ldiruvchi atributi
Input placeholder atributi kiritish maydonining kutilgan qiymatini tavsiflovchi qisqa maslahatni bildiradi (namuna qiymati yoki kutilgan formatning qisqa tavsifi).

Qisqa ko'rsatma foydalanuvchi qiymat kiritishdan oldin kirish maydonida ko'rsatiladi.

To'ldiruvchi atributi quyidagi kiritish turlari bilan ishlaydi: matn, qidiruv, url, tel, elektron pochta va parol.
```
<form action="/action_page.php">
   <label for="phone">Telefon raqamini kiriting:</label>
   <input type="tel" id="telefon" nomi="telefon" to'ldiruvchisi="123-45-678" naqsh="[0-9]{3}-[0-9]{2}-[0- 9]{3}"><br><br>
   <input type="submit" value="yuborish">
</form>
```

* Kerakli atribut

Shaklni yuborishdan oldin kiritilgan ma'lumotlar to'ldirilishi kerakligini bildiradi. U quyidagi kiritish turlari bilan ishlaydi: matn, qidiruv, url, tel, elektron pochta, parol, sana tanlash, raqam, tasdiqlash qutisi, radio va fayl.
```
<form action="/action_page.php">
   <label for="username">Foydalanuvchi nomi:</label>
   <input type="text" id="foydalanuvchi nomi" name="foydalanuvchi nomi" kerak>
   <input type="submit" value="yuborish">
</form>
```


* u qadam atributi

Kirish maydoni uchun qonuniy raqamlar oralig'ini belgilaydi (masalan, qadam="3" yuridik raqamlar -3, 0, 3, 6 va hokazo bo'lishi mumkinligini anglatadi)

Maslahat: Bu atributdan maksimal va min atributlar bilan birgalikda bir qator qonuniy qiymatlarni yaratish uchun foydalanish mumkin.

Step atributi quyidagi kiritish turlari bilan ishlaydi: raqam, diapazon, sana, sana-mahalliy, oy, vaqt va hafta.

```
<form action="/action_page.php">
   <label for="points">Bollar:</label>
   <kiritish turi="raqam" id="nuqta" nomi="nuqta" qadam="3">
   <input type="submit" value="yuborish">
</form>
```
Eslatma: Kirish cheklovlari ishonchli emas va JavaScript noqonuniy kiritishning ko'plab usullarini taqdim etadi. Kirishni xavfsiz cheklash uchun uni qabul qiluvchi (server) ham tekshirishi kerak!

* Avtofokus atributi
Kirish avtofokus atributi sahifa yuklanganda avtomatik ravishda fokus olinadigan kirish maydonini belgilaydi.
```
<form action="/action_page.php">
   <label for="fname">Ism:</label><br>
   <input type="text" id="fname" name="fname" autofocus><br>
   <label for="lname">Familiya:</label><br>
   <input type="text" id="lname" name="lname"><br><br>
   <input type="submit" value="yuborish">
</form>
```

* Balandlik va kenglik atributlari

Kirish balandligi va kengligi atributlari ```<input type="image">``` elementining balandligi va kengligini belgilaydi.

Maslahat: Har doim tasvirlar uchun balandlik va kenglik atributlarini belgilang. Agar balandlik va kenglik o'rnatilgan bo'lsa, sahifa yuklanganda rasm uchun zarur bo'sh joy ajratiladi. Ushbu atributlarsiz brauzer tasvir hajmini bilmaydi va unga tegishli joy ajrata olmaydi. Buning ta'siri shundaki, yuklash paytida sahifa tartibi o'zgaradi (tasvirlar yuklanganda).
```
<form action="/action_page.php">
   <label for="fname">Ism:</label>
   <input type="text" id="fname" name="fname"><br><br>
   <label for="lname">Familiya:</label>
   <input type="text" id="lname" name="lname"><br><br>
   <input type="image" src="img_submit.gif" alt="Yuborish" kengligi="48" balandligi="48">
</form>
```
Eslatma: ```type="image"``` kiritish rasm tugmasini faollashtirgan bosishning X va Y koordinatalarini yuboradi.


* Ro'yxat atributi
Kirish ro'yxati atributi <input> elementi uchun oldindan belgilangan variantlarni o'z ichiga olgan <datalist> elementiga ishora qiladi.

```
<form action="/action_page.php">
   <input list="brauzerlar" name="brauzer">
   <datalist id="brauzerlar">
     <option value="Internet Explorer">
     <option value="Firefox">
     <option value="Chrome">
     <option value="Opera">
     <option value="Safari">
   </datalist>
   <input type="submit" value="yuborish">
</form>
```

* Avtomatik to'ldirish atributi

Input autocomplete atributi shakl yoki kiritish maydonida avtomatik toʻldirishni yoqish yoki oʻchirish kerakligini belgilaydi.

Avtomatik to'ldirish brauzerga qiymatni taxmin qilish imkonini beradi. Agar foydalanuvchi maydonga yozishni boshlaganida, brauzer oldingi kiritilgan qiymatlar asosida maydonni to'ldirish variantlarini ko'rsatishi kerak.

Avtoto'ldirish atributi <form> va quyidagi <input> turlari bilan ishlaydi: matn, qidiruv, url, tel, elektron pochta, parol, sana tanlash, diapazon va rang.

Quyidagi holatda avtomatik to‘ldirish ariza uchun yoqilgan, lekin elektron pochta maydoni uchun o‘chirilgan. Effektni ko'rish uchun shaklni to'ldiring va qayta yuklang.
```
<form action="/action_page.php" autocomplete="on">
   <label for="fname">Ism:</label>
   <input type="text" id="fname" name="fname"><br><br>
   <label for="lname">Familiya:</label>
   <input type="text" id="lname" name="lname"><br><br>
   <label for="email">E-pochta:</label>
   <input type="email" id="email" name="email" autocomplete="off"><br><br>
   <input type="submit" value="yuborish">
</form>
```

* Belgilar soni uchun maxlengthdan foydalaning: ```maxlength="40"```
Raqamli qiymat uchun max dan foydalaning, maksimaldan foydalaning: ```max=40```

<kbd>qaytish</kbd>[Mundarijaga qaytish](#homepage)


---------



## HTML kiritish atributlari

HTML kiritish turi atributi
Teg tavsifi
```<input type="">``` Ko`rsatish uchun kiritish turini belgilaydi

- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
HTML kiritish atributlari: kiritish elementining atributlari

* Qiymat atributi
Import maydoni uchun boshlang'ich (standart) qiymatni belgilaydi
```
<form action="/action_page.php">
   <label for="fname">Ism:</label><br>
   <input type="text" id="fname" name="fname" value="Jon"><br>
   <label for="lname">Familiya:</label><br>
   <input type="text" id="lname" name="lname" value="Doe"><br><br>
   <input type="submit" value="yuborish">
</form>
```

* Faqat o'qish uchun atribut
Faqat o'qish uchun kiritish maydonini belgilaydi. Ushbu kiritish maydonini o'zgartirib bo'lmaydi, lekin foydalanuvchi unga kirishi, matnni ajratib ko'rsatishi va undan nusxa ko'chirishi mumkin. Qiymat shaklni yuborishda yuboriladi.
```
<form action="/action_page.php">
   <label for="fname">Ism:</label><br>
   <input type="text" id="fname" name="fname" value="Jon" faqat o'qish uchun<br>
   <label for="lname">Familiya:</label><br>
   <input type="text" id="lname" name="lname" value="Doe"><br><br>
   <input type="submit" value="yuborish">
</form>
```

* Disabled atributi
Kirish maydoni o'chirilganligi va bunday maydonni ishlatish mumkin emasligi va bosish mumkin emasligi ko'rsatilgan. Shaklni yuborishda qiymat yuborilmaydi.
```
<form action="/action_page.php">
   <label for="fname">Ism:</label><br>
   <input type="text" id="fname" name="fname" value="Jon" o'chirilgan><br>
   <label for="lname">Familiya:</label><br>
   <input type="text" id="lname" name="lname" value="Doe"><br><br>
   <input type="submit" value="yuborish">
</form>
```

* Hajmi atributi

Kirish maydonining belgilar bilan ko'rinadigan kengligini belgilaydi. Standart qiymat 20 oʻlchamdir. Bu atribut Matn, qidiruv, tel, url, elektron pochta va parol bilan ishlaydi.
```
<form action="/action_page.php">
   <label for="fname">Ism:</label><br>
   <input type="text" id="fname" name="fname" size="50"><br>
   <label for="pin">PIN:</label><br>
   <input type="text" id="pin" name="pin" size="4"><br><br>
   <input type="submit" value="yuborish">
</form>
```

* Maksimal uzunlik atributi

Kirish maydonida ruxsat etilgan belgilarning maksimal sonini belgilaydi.

Eslatma: Maksimal uzunlik o'rnatilganda, kiritish maydoni belgilangan belgilar sonidan ko'pini qabul qilmaydi. Biroq, bu atribut hech qanday fikr bildirmaydi. Shunday qilib, agar siz foydalanuvchini ogohlantirmoqchi bo'lsangiz, JavaScript kodini yozishingiz kerak.

```
<form action="/action_page.php">
   <label for="fname">Ism:</label><br>
   <input type="text" id="fname" name="fname" size="50"><br>
   <label for="pin">PIN:</label><br>
   <input type="text" id="pin" name="pin" maxlength="4" size="4"><br><br>
   <input type="submit" value="yuborish">
</form>
```

* Min va Maks atributi
Kirish maydoni uchun minimal va maksimal qiymatlarni belgilaydi. Raqam, diapazon, sana, sana-mahalliy, oy, vaqt va hafta bilan ishlaydi.

Maslahat: Bir qator qonuniy qiymatlarni yaratish uchun maksimal va min atributlaridan birgalikda foydalaning.
```
<form action="/action_page.php">
   <label for="datemax">1980-01-01 dan oldingi sanani kiriting:</label>
   <input type="date" id="datemax" name="datemax" max="1979-12-31"><br><br>

   <label for="datemin">2000-01-01 dan keyingi sanani kiriting:</label>
   <input type="date" id="datemin" name="datemin" min="2000-01-02"><br><br>
  
   <label for="quantity">Miqdor (1 va 5 orasida):</label>
   <kiritish turi="raqam" id="miqdori" nomi="miqdori" min="1" max="5"><br><br>

   <input type="submit" value="yuborish">
</form>
```

* Bir nechta atribut
Foydalanuvchiga kirish maydoniga bir nechta qiymat kiritishga ruxsat berilganligini bildiradi. bir nechta atribut elektron pochta va fayl turlari bilan yaxshi ishlaydi
```
<form action="/action_page.php">
   <label for="files">Fayllarni tanlang:</label>
   <input type="file" id="files" name="fayllar" bir nechta><br><br>
   <input type="submit" value="yuborish">
</form>
```

* Naqsh atributi

Shakl yuborilganda kirish maydonining qiymati tekshiriladigan muntazam ifodalarni belgilaydi. Pattern atributi matn, sana, qidiruv, url, tel, elektron pochta va parol bilan ishlaydi.

Maslahat: foydalanuvchiga yordam berish uchun naqshni tasvirlash uchun global sarlavha atributidan foydalaning.

Maslahat: Muntazam iboralar haqida koʻproq maʼlumotni JavaScript qoʻllanmamizda oʻrganing.

```
<form action="/action_page.php">
   <label for="country_code">Mamlakat kodi:</label>
   <input type="text" id="mamlakat_kodi" nomi="mamlakat_kodi" naqsh="[A-Za-z]{3}" title="Uch harfli mamlakat kodi"><br><br>
   <input type="submit" value="yuborish">
</form>
```

* To'ldiruvchi atributi
Input placeholder atributi kiritish maydonining kutilgan qiymatini tavsiflovchi qisqa maslahatni bildiradi (namuna qiymati yoki kutilgan formatning qisqa tavsifi).

Qisqa ko'rsatma foydalanuvchi qiymat kiritishdan oldin kirish maydonida ko'rsatiladi.

To'ldiruvchi atributi quyidagi kiritish turlari bilan ishlaydi: matn, qidiruv, url, tel, elektron pochta va parol.
```
<form action="/action_page.php">
   <label for="phone">Telefon raqamini kiriting:</label>
   <input type="tel" id="telefon" nomi="telefon" to'ldiruvchisi="123-45-678" naqsh="[0-9]{3}-[0-9]{2}-[0- 9]{3}"><br><br>
   <input type="submit" value="yuborish">
</form>
```

* Kerakli atribut

Shaklni yuborishdan oldin kiritilgan ma'lumotlar to'ldirilishi kerakligini bildiradi. U quyidagi kiritish turlari bilan ishlaydi: matn, qidiruv, url, tel, elektron pochta, parol, sana tanlash, raqam, tasdiqlash qutisi, radio va fayl.
```
<form action="/action_page.php">
   <label for="username">Foydalanuvchi nomi:</label>
   <input type="text" id="foydalanuvchi nomi" name="foydalanuvchi nomi" kerak>
   <input type="submit" value="yuborish">
</form>
```


* u qadam atributi

Kirish maydoni uchun qonuniy raqamlar oralig'ini belgilaydi (masalan, qadam="3" yuridik raqamlar -3, 0, 3, 6 va hokazo bo'lishi mumkinligini anglatadi)

Maslahat: Bu atributdan maksimal va min atributlar bilan birgalikda bir qator qonuniy qiymatlarni yaratish uchun foydalanish mumkin.

Step atributi quyidagi kiritish turlari bilan ishlaydi: raqam, diapazon, sana, sana-mahalliy, oy, vaqt va hafta.

```
<form action="/action_page.php">
   <label for="points">Bollar:</label>
   <kiritish turi="raqam" id="nuqta" nomi="nuqta" qadam="3">
   <input type="submit" value="yuborish">
</form>
```
Eslatma: Kirish cheklovlari ishonchli emas va JavaScript noqonuniy kiritishning ko'plab usullarini taqdim etadi. Kirishni xavfsiz cheklash uchun uni qabul qiluvchi (server) ham tekshirishi kerak!

* Avtofokus atributi
Kirish avtofokus atributi sahifa yuklanganda avtomatik ravishda fokus olinadigan kirish maydonini belgilaydi.
```
<form action="/action_page.php">
   <label for="fname">Ism:</label><br>
   <input type="text" id="fname" name="fname" autofocus><br>
   <label for="lname">Familiya:</label><br>
   <input type="text" id="lname" name="lname"><br><br>
   <input type="submit" value="yuborish">
</form>
```

* Balandlik va kenglik atributlari

Kirish balandligi va kengligi atributlari ```<input type="image">``` elementining balandligi va kengligini belgilaydi.

Maslahat: Har doim tasvirlar uchun balandlik va kenglik atributlarini belgilang. Agar balandlik va kenglik o'rnatilgan bo'lsa, sahifa yuklanganda rasm uchun zarur bo'sh joy ajratiladi. Ushbu atributlarsiz brauzer tasvir hajmini bilmaydi va unga tegishli joy ajrata olmaydi. Buning ta'siri shundaki, yuklash paytida sahifa tartibi o'zgaradi (tasvirlar yuklanganda).
```
<form action="/action_page.php">
   <label for="fname">Ism:</label>
   <input type="text" id="fname" name="fname"><br><br>
   <label for="lname">Familiya:</label>
   <input type="text" id="lname" name="lname"><br><br>
   <input type="image" src="img_submit.gif" alt="Yuborish" kengligi="48" balandligi="48">
</form>
```
Eslatma: ```type="image"``` kiritish rasm tugmasini faollashtirgan bosishning X va Y koordinatalarini yuboradi.


* Ro'yxat atributi
Kirish ro'yxati atributi <input> elementi uchun oldindan belgilangan variantlarni o'z ichiga olgan <datalist> elementiga ishora qiladi.

```
<form action="/action_page.php">
   <input list="brauzerlar" name="brauzer">
   <datalist id="brauzerlar">
     <option value="Internet Explorer">
     <option value="Firefox">
     <option value="Chrome">
     <option value="Opera">
     <option value="Safari">
   </datalist>
   <input type="submit" value="yuborish">
</form>
```

* Avtomatik to'ldirish atributi

Input autocomplete atributi shakl yoki kiritish maydonida avtomatik toʻldirishni yoqish yoki oʻchirish kerakligini belgilaydi.

Avtomatik to'ldirish brauzerga qiymatni taxmin qilish imkonini beradi. Agar foydalanuvchi maydonga yozishni boshlaganida, brauzer oldingi kiritilgan qiymatlar asosida maydonni to'ldirish variantlarini ko'rsatishi kerak.

Avtoto'ldirish atributi <form> va quyidagi <input> turlari bilan ishlaydi: matn, qidiruv, url, tel, elektron pochta, parol, sana tanlash, diapazon va rang.

Quyidagi holatda avtomatik to‘ldirish ariza uchun yoqilgan, lekin elektron pochta maydoni uchun o‘chirilgan. Effektni ko'rish uchun shaklni to'ldiring va qayta yuklang.
```
<form action="/action_page.php" autocomplete="on">
   <label for="fname">Ism:</label>
   <input type="text" id="fname" name="fname"><br><br>
   <label for="lname">Familiya:</label>
   <input type="text" id="lname" name="lname"><br><br>
   <label for="email">E-pochta:</label>
   <input type="email" id="email" name="email" autocomplete="off"><br><br>
   <input type="submit" value="yuborish">
</form>
```

* Belgilar soni uchun maxlengthdan foydalaning: ```maxlength="40"```
Raqamli qiymat uchun max dan foydalaning, maksimaldan foydalaning: ```max=40```

<kbd>qaytish</kbd>[Mundarijaga qaytish](#homepage)


----------


## HTML kiritish formasi atributlari

HTML kiritish shakli* Atributlar

Form atributi: Input form atributi Formaning <input> element elementiga tegishli ekanligini bildiradi. Uning qiymati u tegishli <form> elementining id atributiga teng bo'lishi kerak.

```
<p>Forma atributi kiritish elementi tegishli shaklni bildiradi.</p>

<form action="/action_page.php" id="form1">
   <label for="fname">Ism:</label>
   <input type="text" id="fname" name="fname"><br><br>
   <input type="submit" value="yuborish">
</form>
```
```
<p>Quyidagi "Familiya" maydoni shakl elementidan tashqarida, ammo shaklning bir qismidir.</p>

<label for="lname">Familiya:</label>
<input type="text" id="lname" name="lname" form="form1">
```

* Shakllanish atributi
Input to formation atributi forma yuborilganda kirishni qayta ishlovchi faylning URL manzilini belgilaydi.

Eslatma: Bu atribut ```<form>``` elementining harakat atributini bekor qiladi.

Shakllanish atributi quyidagi kiritish turlari bilan ishlaydi: yuborish va tasvir.

```
<form action="/action_page.php">
   <label for="fname">Ism:</label>
   <input type="text" id="fname" name="fname"><br><br>
   <label for="lname">Familiya:</label>
   <input type="text" id="lname" name="lname"><br><br>
   <input type="submit" value="yuborish">
   <input type="submit" formation="/action_page2.php" value="Administrator sifatida yuborish">
</form>
```

* Forencttype atributi
Input formenctype atributi shakl ma'lumotlari yuborilganda qanday kodlanishi kerakligini belgilaydi (faqat method="post" bilan shakllar uchun).

Eslatma: Bu atribut ```<form>``` elementining enctype atributini bekor qiladi.

Formenctype atributi quyidagi kiritish turlari bilan ishlaydi: yuborish va tasvir.
```
<form action="/action_page_binary.asp" method="post">
   <label for="fname">Ism:</label>
   <input type="text" id="fname" name="fname"><br><br>
   <input type="submit" value="yuborish">
   <input type="submit" formenctype="multipart/form-data" value="Ko'p qismli/form-ma'lumotlar sifatida yuborish">
</form>
```

* Formmethod atributi

Input formmethod atributi amal URL manziliga forma ma'lumotlarini yuborish uchun HTTP usulini belgilaydi.

Eslatma: Bu atribut ```<form>``` elementining metod atributini bekor qiladi.

Formmethod atributi quyidagi kiritish turlari bilan ishlaydi: yuborish va tasvir.

Shakl-ma'lumotlar URL o'zgaruvchilari (method="get") yoki HTTP post tranzaksiyasi (metod="post") sifatida yuborilishi mumkin.

"Get" usuli bo'yicha eslatmalar:

     Ushbu usul forma ma'lumotlarini URL manziliga nom/qiymat juftliklarida qo'shadi
     Bu usul foydalanuvchi natijani belgilamoqchi bo'lgan shakllarni yuborish uchun foydalidir
     URL manziliga qancha maʼlumot joylashtirishingiz mumkin boʻlgan chegara mavjud (brauzerlar orasida farq qiladi), shuning uchun barcha shakl maʼlumotlari toʻgʻri uzatilishiga ishonchingiz komil emas.
     Nozik ma'lumotlarni uzatish uchun hech qachon "olish" usulidan foydalanmang! (parol yoki boshqa maxfiy ma'lumotlar brauzerning manzil satrida ko'rinadi)

"Post" usuli bo'yicha eslatmalar:

     Ushbu usul forma ma'lumotlarini HTTP post tranzaksiyasi sifatida yuboradi
     “Post” usuli bilan yuborilgan arizalarni xatcho‘p qilib bo‘lmaydi
     "Post" usuli "olish" dan ko'ra mustahkamroq va xavfsizroqdir va "post" o'lchamida cheklovlarga ega emas.

```
<form action="/action_page.php" method="get" target="_blank">
   <label for="fname">Ism:</label>
   <input type="text" id="fname" name="fname"><br><br>
   <label for="lname">Familiya:</label>
   <input type="text" id="lname" name="lname"><br><br>
   <input type="submit" value="GET-dan foydalanib yuborish">
   <input type="submit" formmethod="post" value="POST yordamida yuborish">
</form>
```

* Formtarget atributi

Input formattarget atributi forma yuborilgandan so'ng olingan javobni qayerda ko'rsatishni ko'rsatadigan nom yoki kalit so'zni belgilaydi.

Eslatma: Bu atribut ```<form>``` elementining maqsad atributini bekor qiladi.

Formtarget atributi quyidagi kiritish turlari bilan ishlaydi: yuborish va tasvir.
```
<form action="/action_page.php">
   <label for="fname">Ism:</label>
   <input type="text" id="fname" name="fname"><br><br>
   <label for="lname">Familiya:</label>
   <input type="text" id="lname" name="lname"><br><br>
   <input type="submit" value="yuborish">
   <input type="submit" formtarget="_blank" value="Yangi oynaga/tabga yuborish">
</form>
```

* Formnovalidate atributi
Input formnovalidate atributi <input> elementi yuborilganda tasdiqlanmasligi kerakligini bildiradi.

Eslatma: Bu atribut ```<form>``` elementining novalidate atributini bekor qiladi.

Formnovalidate atributi quyidagi kiritish turlari bilan ishlaydi: yuborish.

```
<form action="/action_page.php">
   <label for="email">E-pochta manzilingizni kiriting:</label>
   <input type="email" id="email" name="email" kerak><br><br>
   <input type="submit" value="yuborish">
   <input type="submit" formnovalidate="formnovalidate" value="Tasdiqlanmagan holda yuborish">
</form>
```

* Novalidate atributi
Novalidate atributi <form> atributidir.

Agar mavjud bo'lsa, novalidate barcha shakl ma'lumotlari yuborilganda tasdiqlanmasligi kerakligini bildiradi.
```
<form action="/action_page.php" novalidate>
   <label for="email">E-pochta manzilingizni kiriting:</label>
   <input type="email" id="email" name="email" kerak><br><br>
   <input type="submit" value="yuborish">
</form>
```

Chapter summary
HTML Form and Input Elements
Tag 	Description
<form> 	Defines an HTML form for user input
<input> 	Defines an input control

<kbd>return</kbd>[Back to table of contents](#homepage)



----------

## CSS Forms

CSS can enhance the looks of an HTML form. 


<!DOCTYPE html>
<html>
<style>
input[type=text], select {
  width: 100%;
  padding: 12px 20px;
  margin: 8px 0;
  display: inline-block;
  border: 1px solid #ccc;
  border-radius: 4px;
  box-sizing: border-box;
}

input[type=submit] {
  width: 100%;
  background-color: #4CAF50;
  color: white;
  padding: 14px 20px;
  margin: 8px 0;
  border: none;
  border-radius: 4px;
  cursor: pointer;
}

input[type=submit]:hover {
  background-color: #45a049;
}

div {
  border-radius: 5px;
  background-color: #f2f2f2;
  padding: 20px;
}
</style>
<body>

<h3>Using CSS to style an HTML Form</h3>

<div>
  <form action="/action_page.php">
    <label for="fname">First Name</label>
    <input type="text" id="fname" name="firstname" placeholder="Your name..">

    <label for="lname">Last Name</label>
    <input type="text" id="lname" name="lastname" placeholder="Your last name..">

    <label for="country">Country</label>
    <select id="country" name="country">
      <option value="australia">Australia</option>
      <option value="canada">Canada</option>
      <option value="usa">USA</option>
    </select>
  
    <input type="submit" value="Submit">
  </form>
</div>

</body>
</html>



Styling Input Fields

Use the width property to determine the width of the input field:


<!DOCTYPE html>
<html>
<head>
<style> 
input {
  width: 100%;
}
</style>
</head>
<body>

<h2>A full-width input field</h2>

<form>
  <label for="fname">First Name</label>
  <input type="text" id="fname" name="fname">
</form>

</body>
</html>


The example above applies to all <input> elements. If you only want to style a specific input type, you can 

use attribute selectors:

    input[type=text] - will only select text fields
    input[type=password] - will only select password fields
    input[type=number] - will only select number fields
    etc..


Padded Inputs

Use the padding property to add space inside the text field.

Tip: When you have many inputs after each other, you might also want to add some margin, to add more space 

outside of them:

<!DOCTYPE html>
<html>
<head>
<style> 
input[type=text] {
  width: 100%;
  padding: 12px 20px;
  margin: 8px 0;
  box-sizing: border-box;
}
</style>
</head>
<body>

<h2>Padded input fields</h2>

<form>
  <label for="fname">First Name</label>
  <input type="text" id="fname" name="fname">
  <label for="lname">Last Name</label>
  <input type="text" id="lname" name="lname">
</form>

</body>
</html>



E'tibor bering, biz box-sizing xususiyatini border-box-ga o'rnatdik. Bu plomba va oxir-oqibat ishonch hosil qiladi

chegaralar elementlarning umumiy kengligi va balandligiga kiritilgan.


Chegaralangan kirishlar

Chegara o'lchami va rangini o'zgartirish uchun border xususiyatidan foydalaning va qo'shish uchun border-radius xususiyatidan foydalaning

yumaloq burchaklar:

<!DOCTYPE html>
<html>
<head>
<uslub>
kiritish[type=matn] {
   kengligi: 100%;
   to'ldirish: 12px 20px;
   chegara: 8px 0;
   quti o'lchami: chegara qutisi;
   chegara: 2px qattiq qizil;
   chegara radiusi: 4px;
}
</style>
</head>
<tana>

<h2>Chegarali kiritish maydonlari</h2>

<form>
   <label for="fname">Ism</label>
   <input type="text" id="fname" name="fname">
   <label for="lname">Familiya</label>
   <input type="text" id="lname" name="lname">
</form>

</body>
</html>


border-bottom xususiyatidan foydalaning, siz quyida ko'rsatilganidek, faqat pastki chegarani xohlaysiz:

<!DOCTYPE html>
<html>
<head>
<uslub>
kiritish[type=matn] {
   kengligi: 100%;
   to'ldirish: 12px 20px;
   chegara: 8px 0;
   quti o'lchami: chegara qutisi;
   chegara: yo'q;
   chegara-pastki: 2px qattiq qizil;
}
</style>
</head>
<tana>

<h2>Kirish maydonlari pastki chegarasi</h2>

<form>
   <label for="fname">Ism</label>
   <input type="text" id="fname" name="fname">
   <label for="lname">Familiya</label>
   <input type="text" id="lname" name="lname">
</form>

</body>
</html>




Rangli kirishlar

Kirish uchun fon rangini qo'shish uchun fon rangi xususiyatidan foydalaning va o'zgartirish uchun rang xususiyatidan foydalaning

matn rangi:

<!DOCTYPE html>
<html>
<head>
<uslub>
kiritish[type=matn] {
   kengligi: 100%;
   to'ldirish: 12px 20px;
   chegara: 8px 0;
   quti o'lchami: chegara qutisi;
   chegara: yo'q;
   fon rangi: #3CBC8D;
   rang: oq;
}
</style>
</head>
<tana>

<h2>Rangli kiritish maydonlari</h2>

<form>
   <label for="fname">Ism</label>
   <input type="text" id="fname" name="fname" value="Jon">
   <label for="lname">Familiya</label>
   <input type="text" id="lname" name="lname" value="Doe">
</form>

</body>
</html>




Fokuslangan kirishlar

Odatiy bo'lib, ba'zi brauzerlar diqqat markazida bo'lganda (bosilganda) kiritish atrofida ko'k kontur qo'shadi. Siz .. qila olasiz; siz ... mumkin

konturni qo'shish orqali ushbu xatti-harakatni olib tashlang: none; kirishga.

Fokus olinganda kiritish maydoni bilan biror narsa qilish uchun :focus selektoridan foydalaning:


<!DOCTYPE html>
<html>
<head>
<uslub>
kiritish[type=matn] {
   kengligi: 100%;
   to'ldirish: 12px 20px;
   chegara: 8px 0;
   quti o'lchami: chegara qutisi;
   chegara: 1px qattiq #555;
   kontur: yo'q;
}

kiritish[type=matn]:fokus {
   fon rangi: ochiq ko'k;
}
</style>
</head>
<tana>

<h2>Rangli kiritish maydonlari:fokus</h2>

<p>Bu yerda, kiritish maydoni diqqat markazida boʻlganda (bosilganda) rangga ega boʻladi:</p>

<form>
   <label for="fname">Ism</label>
   <input type="text" id="fname" name="fname" value="Jon">
   <label for="lname">Familiya</label>
   <input type="text" id="lname" name="lname" value="Doe">
</form>

</body>
</html>



Fokus paytida ochiq ko'k chiziqqa o'tish uchun:


<!DOCTYPE html>
<html>
<head>
<uslub>
kiritish[type=matn] {
   kengligi: 100%;
   to'ldirish: 12px 20px;
   chegara: 8px 0;
   quti o'lchami: chegara qutisi;
   chegara: 3px qattiq #ccc;
   -webkit-o'tish: 0,5s;
   o'tish: 0,5 s;
   kontur: yo'q;
}

kiritish[type=matn]:fokus {
   chegara: 3px qattiq #555;
}
</style>
</head>
<tana>

<h2>Qora hoshiyali kiritish maydonlari:fokus</h2>

<p>Bu yerda kiritish maydoni diqqat markazida boʻlganda (bosilganda) qora hoshiya rangiga ega boʻladi. Biz ham qo'shdik

Chegara rangini jonlantirish uchun CSS oʻtish xususiyati (fokusdagi rangni oʻzgartirish uchun 0,5 soniya ketadi):</p>

<form>
   <label for="fname">Ism</label>
   <input type="text" id="fname" name="fname" value="Jon">
   <label for="lname">Familiya</label>
   <input type="text" id="lname" name="lname" value="Doe">
</form>

</body>
</html>



Belgi/tasvir bilan kiriting

Agar siz kiritishda belgi bo'lishini istasangiz, background-image xususiyatidan foydalaning va uni bilan joylashtiring

fon-pozitsiya xususiyati. Shuningdek, belgining bo'sh joyini zaxiralash uchun katta chap to'ldirishni qo'shayotganimizga e'tibor bering:

<!DOCTYPE html>
<html>
<head>
<uslub>
kiritish[type=matn] {
   kengligi: 100%;
   quti o'lchami: chegara qutisi;
   chegara: 2px qattiq #ccc;
   chegara radiusi: 4px;
   shrift o'lchami: 16px;
   fon rangi: oq;
   fon rasmi: url('searchicon.png');
   fon holati: 10px 10px;
   fon-takrorlash: takrorlanmaslik;
   to'ldirish: 12px 20px 12px 40px;
}
</style>
</head>
<tana>

<h2>Ichkarida belgi bo'lgan kiritish maydoni</h2>

<form>
   <input type="text" name="search" placeholder="Search..">
</form>

</body>
</html>



Animatsiyalangan qidiruv kiritish

Ushbu misolda biz CSS-ga o'tish xususiyatidan foydalanib, qidiruv kiritish kengligi kelganda uni jonlantiramiz

diqqat. O'tish xususiyati haqida keyinroq, CSS Transitions bo'limida bilib olasiz.

<!DOCTYPE html>
<html>
<head>
<uslub>
kiritish[type=matn] {
   kengligi: 130px;
   quti o'lchami: chegara qutisi;
   chegara: 2px qattiq #ccc;
   chegara radiusi: 4px;
   shrift o'lchami: 16px;
   fon rangi: oq;
   fon rasmi: url('searchicon.png');
   fon holati: 10px 10px;
   fon-takrorlash: takrorlanmaslik;
   to'ldirish: 12px 20px 12px 40px;
   o'tish: kengligi 0,4 s qulaylik;
}

kiritish[type=matn]:fokus {
   kengligi: 100%;
}
</style>
</head>
<tana>

<h2>Qidiruv kiritish kengligini jonlantiring</h2>

<form>
   <input type="text" name="search" placeholder="Search..">
</form>

</body>
</html>



Styling Textreas

Maslahat: Matn maydonlarining oʻlchamini oʻzgartirishga yoʻl qoʻymaslik uchun oʻlchamini oʻzgartirish xususiyatidan foydalaning (pastki qismdagi “grabber”ni oʻchiring.

o'ng burchak):

<!DOCTYPE html>
<html>
<head>
<uslub>
matn maydoni {
   kengligi: 100%;
   balandligi: 150px;
   to'ldirish: 12px 20px;
   quti o'lchami: chegara qutisi;
   chegara: 2px qattiq #ccc;
   chegara radiusi: 4px;
   fon rangi: #f8f8f8;
   shrift o'lchami: 16px;
   o'lchamini o'zgartirish: yo'q;
}
</style>
</head>
<tana>

<h2>Matn maydonini uslublash</h2>

<p><strong>Maslahat:</strong> Matn maydonlarining oʻlchamini oʻzgartirishning oldini olish uchun oʻlchamini oʻzgartirish xususiyatidan foydalaning (oʻchiring

Pastki o'ng burchakdagi "grabber"):</p>

<form>
   <textarea>Ba'zi matn...</textarea>
</form>

</body>
</html>



Styling Menyularni tanlang

Quyidagi rasmga qarang:


<!DOCTYPE html>
<html>
<head>
<uslub>
tanlang {
   kengligi: 100%;
   to'ldirish: 16px 20px;
   chegara: yo'q;
   chegara radiusi: 4px;
   fon rangi: #f1f1f1;
}
</style>
</head>
<tana>

<h2>Tanlangan menyuni shakllantirish</h2>

<form>
   <select id="mamlakat" nomi="mamlakat">
   <option value="au">Avstraliya</option>
   <option value="ca">Kanada</option>
   <option value="usa">AQSh</option>
   </select>
</form>

</body>
</html>



Styling kiritish tugmalari

<!DOCTYPE html>
<html>
<head>
<uslub>
kiritish[turi=tugma], kiritish[turi=yuborish], kiritish[turi=qayta tiklash] {
   fon rangi: #4CAF50;
   chegara: yo'q;
   rang: oq;
   to'ldirish: 16px 32px;
   matn-bezak: yo'q;
   chegara: 4px 2px;
   kursor: ko'rsatgich;
}
</style>
</head>
<tana>

<h2>Stillash shakli tugmalari</h2>

<kiritish turi="tugma" qiymati="tugma">
<input type="reset" value="Reset">
<input type="submit" value="yuborish">

</body>
</html>


Bu yerda CSS tugmalari qoʻllanmasini koʻring: https://www.w3schools.com/css/css3_buttons.asp

Javob berish shakli

Effektni ko'rish uchun brauzer oynasining o'lchamini o'zgartiring. Ekranning kengligi 600px dan kam bo'lsa, ikkita ustun hosil qiling

bir-birining yonida emas, balki bir-birining ustiga qo'ying.

Kengaytirilgan: Quyidagi misolda javob beruvchi shakl yaratish uchun media so'rovlaridan foydalaniladi. haqida ko'proq bilib olasiz

bu keyingi bobda.



<!DOCTYPE html>
<html>
<head>
<uslub>
* {
   quti o'lchami: chegara qutisi;
}

kiritish[type=matn], tanlash, matn maydoni {
   kengligi: 100%;
   to'ldirish: 12px;
   chegara: 1px qattiq #ccc;
   chegara radiusi: 4px;
   o'lchamini o'zgartirish: vertikal;
}

teg {
   to'ldirish: 12px 12px 12px 0;
   displey: inline-block;
}

kiritish[type=submit] {
   fon rangi: #4CAF50;
   rang: oq;
   to'ldirish: 12px 20px;
   chegara: yo'q;
   chegara radiusi: 4px;
   kursor: ko'rsatgich;
   suzuvchi: o'ng;
}

kiritish[type=submit]: suring {
   fon rangi: #45a049;
}

.idish {
   chegara radiusi: 5px;
   fon rangi: #f2f2f2;
   to'ldirish: 20px;
}

.col-25 {
   float: chap;
   kengligi: 25%;
   tepadan chet: 6px;
}

.col-75 {
   float: chap;
   kengligi: 75%;
   tepadan chet: 6px;
}

/* Ustunlardan keyingi floatlarni tozalash */
.qator:keyin {
   tarkib: "";
   ko'rsatish: jadval;
   aniq: ikkalasi ham;
}

/* Javob beruvchi tartib - ekran kengligi 600px dan kam bo'lsa, ikkita ustunni har birining ustiga qo'ying.

bir-birining o'rniga boshqa */
@media ekrani va (maksimal kenglik: 600px) {
   .col-25, .col-75, input[type=submit] {
     kengligi: 100%;
     yuqori chegara: 0;
   }
}
</style>
</head>
<tana>

<h2>Javob beruvchi shakl</h2>
<p>Effektni ko'rish uchun brauzer oynasining o'lchamini o'zgartiring. Ekranning kengligi 600px dan kam bo'lsa, ikkitasini qiling

ustunlar yonma-yon emas, bir-birining ustiga joylashadi.</p>

<div class="container">
   <form action="/action_page.php">
   <div class="satr">
     <div class="col-25">
       <label for="fname">Ism</label>
     </div>
     <div class="col-75">
       <input type="text" id="fname" name="firstname" placeholder="Sizning ismingiz..">
     </div>
   </div>
   <div class="satr">
     <div class="col-25">
       <label for="lname">Familiya</label>
     </div>
     <div class="col-75">
       <input type="text" id="lname" name="familiya" placeholder="Sizning familiyangiz..">
     </div>
   </div>
   <div class="satr">
     <div class="col-25">
       <label for="country">Mamlakat</label>
     </div>
     <div class="col-75">
       <select id="mamlakat" nomi="mamlakat">
         <option value="australia">Avstraliya</option>
         <option value="canada">Kanada</option>
         <option value="usa">AQSh</option>
       </select>
     </div>
   </div>
   <div class="satr">
     <div class="col-25">
       <label for="subject">Mavzu</label>
     </div>
     <div class="col-75">
       <textarea id="subject" name="subject" placeholder="Biror narsa yozing.." style="height:200px"></textarea>
     </div>
   </div>
   <br>
   <div class="satr">
     <input type="submit" value="yuborish">
   </div>
   </form>
</div>

</body>
</html>
<kbd>qaytish</kbd>[Mundarijaga qaytish](#homepage)