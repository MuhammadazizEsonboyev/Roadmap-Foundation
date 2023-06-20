## HTML ATTRIBUTES
 **Attribute comes as name="value"
* HTML havolalari: ```<a href="https://www.w3schools.com">Visit W3Schools</a>``` 
SRC atributi: 
```
<h2>The src Attribute</h2>
<p>HTML images are defined with the img tag, and the filename of the image source is specified in the src attribute:</p>
<img src="img_girl.jpg" width="500" height="600">
```
**ichida urlni ko'rsatish ```src``` xususiyat
Mutlaq url: boshqa saytdagi rasmga havolalar: src="https://www.w3schools.com/images/img_girl.jpg"
Nisbiy url: Veb-sayt ichida joylashtirilgan rasmga havolalar. Bu yerda hech qanday domen nomi kiritilmagan.src="img_girl.jpg"
src="/images/img_girl.jpg"   **bu holda, slash sayt url-ga nisbatan
**Kenglik va balandlik atributi (piksel) bilan  ```<img>```
```
 <img src="img_girl.jpg" width="500" height="600"> 
```
**Alt atributi, agar foydalanuvchi rasmni o'qiy olmasa, rasm uchun muqobil matnni o'z ichiga oladi: <img src="img_girl.jpg" alt="Girl with a jacket"> 
**style atributi tasvirga rang, shrift, oʻlcham va boshqalar kabi uslub elementlarini qoʻshadi
```
 <p style="color:red;">This is a red paragraph.</p> 
```
**Lang atributi: har doim bir ichiga kiritilishi kerak <html> qidiruv tizimlariga sizni topishga yordam berish uchun e'lon qilingan veb-sayt tilini belgilang
```
<!DOCTYPE html>
<html lang="en">
<body>
...
</body>
</html>
```
*Siz mamlakat atributini ham kiritishingiz mumkin.
```
<!DOCTYPE html>
<html lang="en-US">
<body>
...
</body>
</html>
```
**Sarlavha atributi: element va atribut haqida qo'shimcha ma'lumot beradi
sichqoncha ko'rsatgichi ustida ishlaganda maslahatchi sifatida ko'rsatiladi.
```
 <p title="I'm a tooltip">This is a paragraph.</p> 
```
W3C qo'shtirnoq ichida atributlarga ega bo'lishni tavsiya qiladi va atributda bo'sh joy mavjud bo'lsa, sizda bo'sh joy bo'lishi kerak.
*atribut qiymati tirnoqlardan birini o'z ichiga olgan bo'lsa, boshqa tirnoqdan foydalaning
```
<p title='John "ShotGun" Nelson'>
```
Yoki aksincha:
```
<p title="John 'ShotGun' Nelson"> 
```
***Xulosa atributlari
* Barcha HTML elementlari atributlarga ega bo'lishi mumkin
* ```<a>``` ning href atributi havola boradigan sahifaning URL manzilini bildiradi.
* ```<img>``` src atributi ko`rsatiladigan rasmga yo`lni belgilaydi
* ```<img>``` kenglik va balandlik atributlari tasvirlar o`lchami haqida ma`lumot beradi
* ```<img>``` alt atributi rasm uchun muqobil matnni taqdim etadi
* Style atributi rang, shrift, oʻlcham va boshqalar kabi elementga uslublar qoʻshish uchun ishlatiladi
* ```<html>``` tegining lang atributi Web-sahifa tilini e'lon qiladi.
* Sarlavha atributi element haqida ba'zi qo'shimcha ma'lumotlarni belgilaydi
<kbd>return</kbd>[Mundarijaga qaytish](#homepage)

---------------------------------------


## References
---
* [HTML forms Guide \| MDN](https://developer.mozilla.org/en-US/docs/Learn/HTML/Forms)
* [The native form widgets](https://developer.mozilla.org/en-US/docs/Learn/HTML/Forms/The_native_form_widgets)
* [HTML5 forms introduction and new attributes](http://html5doctor.com/html5-forms-introduction-and-new-attributes/)
* [HTML Form \| W3C](https://www.w3.org/TR/html5/forms.html)
* Mobil kirishlar
  * [mobile input types](http://mobileinputtypes.com/)
  * [HTML5 for the mobile web – forms and input types](https://mobiforge.com/design-development/html5-mobile-web-forms-and-input-types)
* Elementlar: [`<form>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/form),
  [`<input>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/input),
  [`<label>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/label),
  `<button>`, `<datalist>`, `<legend>`, `<label>`, `<select>`, `<optgroup>`, `<option>`, `<textarea>`, `<keygen>`, `<fieldset>`, `<output>`, `<progress>`
* Atributlar
  * [`<form>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/form#Attributes): `action`, `method`
  * [`<input>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/input#Attributes): `type`
  * [`<label>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/label#Attributes): `for`

---------------------------------------



## HTML sarlavhalari
Sarlavhalar ```<h1> dan <h6>``` gacha bo`ladi. Qidiruv mexanizmlari ulardan veb-sahifa tuzilishini tushunish uchun foydalanadi
Asosiy sarlavhalar uchun h1 dan keyin h2 va boshqalardan foydalaning
Har bir sarlavha o'zining standart o'lchamiga ega. Buni uslub elementi ichida belgilash orqali o'zgartirishingiz mumkin.
* Uslubingizni shunday o'zgartiring:
```
<h1 style="font-size:60px;">Heading 1</h1>
```
<kbd>return</kbd>[Mundarijaga qaytish](#homepage)

---------------------------------------

## HTML SAHIFALAR
Htmlda siz har bir ekran o'lchamida html qanday ko'rsatilishiga ishonchingiz komil emas. Hujjatga qo'shimcha qatorlar yoki bo'shliqlar qo'shish sahifaga yangi qatorlarni qo'shmaydi.
Brauzer sahifa ko'rsatilgandan so'ng qo'shimcha bo'shliqlarni olib tashlaydi
```
<p>This is a paragraph</p>
```
* Gorizontal qoidalar: ```<hr>``` Tarkibni ajratish (ozgartirishni belgilash) uchun ishlatiladi va HTML sahifasida tematik tanaffusni belgilaydi. U gorizontal chiziq sifatida ko'rinadi.
```<hr>``` tegining yopish tegi yo'q, chunki u bo`sh teg.
* Satr uzilishlari: ```<br>``` elementi
Yangi paragrafni boshlamasdan, satrlar uzilishi kerak bo'lganda foydalaning.
She'r muammosi: She'rlar ```<pre>``` oldindan formatlangan matn tegiga kiritilishi kerak
```<pre>``` tegi qattiq kenglikdagi shriftda (odatda Courier) matnni ko'rsatadi va u bo'shliqlarni ham, qatorlarni ham saqlaydi.
Teglar xulosasi
```
<p>   Paragrafni belgilaydi
<hr>   Tarkibdagi tematik o'zgarishlarni belgilaydi
<br>   Bitta qatorli tanaffusni kiritadi
<pre>   Oldindan formatlangan matnni belgilaydi
```
<kbd>return</kbd>[Mundarijaga qaytish](#homepage)

---------------------------
## HTML USLUBLARI
HTML uslubi atributi sintaksisi:
```
<tagname style="property:value;">
```
* Bu erda xususiyat CSS xususiyati va qiymat CSS qiymatidir.
* Fon rangi: HTML elementi uchun fon rangini belgilaydi
```
<body style="background-color:powderblue;">
```
* Ikki xil element uchun fon rangini o'rnating:
```
<h1 style="background-color:powderblue;">This is a heading</h1>
<p style="background-color:tomato;">This is a paragraph.</p>
```
**Matn rangi
```
 <h1 style="color:blue;">This is a heading</h1>
<p style="color:red;">This is a paragraph.</p> 
```
** Shriftlar
```
 <h1 style="font-family:verdana;">This is a heading</h1>
<p style="font-family:courier;">This is a paragraph.</p> 
```
**Matn hajmi
```
 <h1 style="font-size:300%;">This is a heading</h1>
<p style="font-size:160%;">This is a paragraph.</p> 
```
**Matnni tekislash
```
 <h1 style="text-align:center;">Centered Heading</h1>
<p style="text-align:center;">Centered paragraph.</p> 
```
Uslublar haqida xulosa
* HTML elementlarini uslublash uchun uslub atributidan foydalaning
* Fon rangi uchun fon rangidan foydalaning
* Matn ranglari uchun rangdan foydalaning
* Matn shriftlari uchun shrift oilasidan foydalaning
* Matn o'lchamlari uchun shrift o'lchamidan foydalaning
* Matnni tekislash uchun matnni tekislashdan foydalaning
<kbd>qaytish</kbd>[Mundarijaga qaytish](#homepage)

