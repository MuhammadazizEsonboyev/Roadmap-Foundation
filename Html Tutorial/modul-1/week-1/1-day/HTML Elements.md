# HTML elementlari

- HTML elementi boshlang'ich tegdan yakuniy teggacha bo'lgan hamma narsadir:

``` html 
<tagname > Kontent shu yerda... </tagname>
```

- Ba'zi HTML elementlariga misollar:

```html 
<h1> Mening birinchi sarlavham </h1>
<p> Mening birinchi xatboshim. </p>
```

```html 
Start tag	Element content	End tag

<h1>My First Heading</h1>
<p>	My first paragraph.</p>
<br>none
```

# Ichki HTML elementlari

```html 

- HTML elementlari ichki joylashtirilishi mumkin (bu elementlar boshqa elementlarni o'z ichiga olishi mumkinligini anglatadi).

- Barcha HTML hujjatlari ichki o'rnatilgan HTML elementlaridan iborat.

- Quyidagi misolda to'rtta HTML elementi ( <html>, <body>, <h1> va <p>) mavjud:

```

```html
<!DOCTYPE html>
<html>
<body>

<h1>My First Heading</h1>
<p>My first paragraph.</p>

</body>
</html>
```

[O'zingizni sinab ko'ring👆](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_elements)


# Misol tushuntirildi


- Element <html>ildiz elementidir va u butun HTML hujjatini belgilaydi.

- Uning boshlang'ich tegi <html>va tugash tegi bor </html>.

- Keyin <html>element ichida element mavjud <body> :

```html

<body>

<h1>My First Heading</h1>
<p>My first paragraph.</p>

</body>

```


```html
Element <body>hujjatning tanasini belgilaydi.

Uning boshlang'ich tegi <body>va tugash tegi bor </body>.

Keyin <body>element ichida yana ikkita element mavjud: <h1>va <p>:
```

```html 
<h1>My First Heading</h1>
<p>My first paragraph.</p>
```

```html
Element <h1>sarlavhani belgilaydi.

Uning boshlang'ich yorlig'i <h1>va tugatish tegi mavjud </h1>:
```


```html
<h1>My First Heading</h1>
```


```html
- Element <p>paragrafni belgilaydi.

- Uning boshlang'ich yorlig'i <p>va tugatish tegi mavjud </p>
```

```html
<p>My first paragraph.</p>
```

# Hech qachon yakuniy tegni o'tkazib yubormang

- Ba'zi HTML elementlari, hatto oxirgi tegni unutgan bo'lsangiz ham, to'g'ri ko'rsatiladi:

```html 
<html>
<body>

<p>This is a paragraph
<p>This is a paragraph

</body>
</html>
```

[O'zingizni sinab ko'ring 👆](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_no_endtag)

# Bo'sh HTML elementlari


```md
Tarkibsiz HTML elementlari bo'sh elementlar deb ataladi.

Teg <br>satr uzilishini belgilaydi va yopish tegi bo'lmagan bo'sh elementdir:
```

```html
<p>This is a <br> paragraph with a line break.</p>
```

[O'zingizni sinab ko'ring 👆](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_elements_br)


# HTML katta harflarga sezgir emas

```md
HTML teglari katta-kichik harflarga sezgir emas: <p>bilan bir xil degan ma'noni anglatadi <p>.

HTML standarti kichik harf teglarini talab qilmaydi, lekin W3C HTMLda kichik harflarni tavsiya qiladi va XHTML kabi qattiqroq hujjat turlari uchun kichik harflarni talab qiladi .
```


