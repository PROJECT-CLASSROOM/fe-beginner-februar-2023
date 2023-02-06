*   📖: dokumentacija ili članak
*   🛠: online alati / alati za testiranje
*   📹: slika ili video sadrzaj

## Osnovne Frontend Tehnologije

1.  [HTML](#html---hyper-text-markup-language)
    1.  [HTML](#html)
    2.  [HEAD](#head)
    3.  [BODY](#body)
2.  [CSS](#css)
3.  [JAVASCRIPT](#javascript)

## HTML - Hyper Text Markup Language

**HTML** nam omogućava da definišemo strukturu i sadržaj web stranice.

### Minimalna struktura stranice

Svaki HTML dokument ima sledecu strukturu:

```html
<!DOCTYPE html>
<html>
    <head>
        <meta charset="UTF-8">
        <title>Title</title>
    </head>
    <body>
        <!-- content here -->
    </body>
</html>
```

**Doctype:** Deklaracija koju navodimo na početku svakog HTML dokumenta. Govori pretraživaču kog je tipa dokument kojeg čita, na taj način pretraživač zna kako da interpretira sadržaj. Deklaracija nije HTML tag i nije _case sensitive_.

```html
<!DOCTYPE html> <!-- Označava da je u pitanju HTML5 -->
```
#### **HTML Validator**

Kada smo napisali HTML stranicu, neophodno je da i validiramo koristeći neki od servisa za validaciju. Često će nam pretraživač oprostiti greške koje napravimo, i činiće nam se kao da je sa našom stranicom sve naizgled onako kako treba biti. Validacija nam može pomoći da proverimo  da li smo napravili dobru strukturu stranice, ili smo možda zaboravili da ubacimo neke atribute koji su obavezni. Preporuka je da se svaki HTML dokument na kom radimo validira, jer se i samo pretraživači menjaju, i možda u budućnosti nam neće toliko praštati greške koje nam se slučajno potkradu.

> *   🛠:   [**W3C Validator**](https://dev.to/maggiecodes_/why-is-lt-meta-charset-utf-8-gt-important-59hl)
> *   📖:  [**Blog- Greške u HTML dokumentu**](https://www.classroom.rs/greske-u-html-dokumentu/)


[**⬆ back to top**](#)

#### **HTML**

---

Ceo dokument se nalazi unutar \<html> taga. Ovaj tag se navodi odmah nakon _doctype_ deklaracije. Unutar **html** taga nalaze se **head** i **body** tag. 

_Note: Uvek uključi **lang** atribut unutar \<html> taga. Ovo treba da pomogne pretraživačima._

_›_ **Language atribut:** Definiše jezik na kom je napisan sadržaj dokumenta.

```html
<html lang="en">
```

#### **HEAD**

---

Neki od elemenata koji se mogu naci unutar `<head>` taga su: `meta`, `title`, `link,` `style`, `script`.

<table><tbody><tr><td><strong>tag</strong></td><td><strong>element</strong></td></tr><tr><td>title</td><td>page title</td></tr><tr><td>meta</td><td>metadata</td></tr><tr><td>link</td><td>link to external source</td></tr><tr><td>script</td><td>Jacascript code</td></tr></tbody></table>

### Preporučeni minimum tagova koje treba uključiti

Ispod su osnovni elementi za bilo koji web dokument:

```html
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<!--
  Ova 2 meta taga koja su navedena iznad,
  treba da dodju prvi unutar <head> taga
  kako bi obezbedili pravilno renderovanje dokumenta.
  Svi ostali elementi dolaze posle ovih tagova.
 -->
<title>Page Title</title>
```

`meta charset` - defines the encoding of the website, `utf-8` je standard. (Omogućava prikazivanje nestandardih simbola - emoji, slova sa kvačicama)

`meta name="viewport"` - viewport settings utiče na responsivnost mobilnih uređaja

`width=device-width` - koristi fizičku širinu uređaja (odlično za mobilne uređaje!)

`initial-scale=1` - inicijalni zoom, 1 znači nema inicijalnog zumiranja

_Note: Moguće je upotpunosti isključiti mogućnost korisniku da uvećava stranicu, međutim to nije preporučljivo. Mnogi ljudi koriste opciju zumiranja prilikom korišćenja web sajta ili aplikacije. Isključivanje je ponekad zaista neophodno za određene vrste igrica i aplikacija._

> *   📖:  [**Meta charset**](https://dev.to/maggiecodes_/why-is-lt-meta-charset-utf-8-gt-important-59hl)

### meta

---

**› description:** kratak opis dokumenta (do 150 karaktera). Može da se koristi kao za optimizaciju search engine rezultata. 

```html
<meta name="description" content="A description of the page">
```

> *   📖 [**Meta Description**](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/The_head_metadata_in_HTML#adding_an_author_and_description)

› **keywords:** ključne reči za search engine, ključne reči se razdvajaju zarezom.

```html
  <meta name="keywords" content="HTML, CSS, JavaScript">
```

> _Many search engines do not consider such keywords, because this feature has historically been used unreliably and even misleadingly as a way to spam search engine results in a way that is not helpful for users._

› **author:** omogućava da se navede autor web stranice.

```html
<meta name="author" content="John Doe">
```

### title

---

Title tag se koristi na svim stranicama (dužina title-a je bitna i utiče na SEO: Google računa širinu pixela karaktera koji se koristi u title-u. Prosečan broj za limit broja karaktera koji se koriste u title tagu je oko 55.)

```html
<!-- Nalov dokumenta -->
<title>My First Page</title>
```

> *   📖:  [**The Document Title element**](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/title)


### link

Link tag sastoji se od sledećih atributa:

```html
<link rel="" type="" sizes="" href="">
```

**rel -** koristi se za definisanje veze između html dokumenta i povezanog resursa. 

**type** - tip povezanog resursa

**sizes** - za definisanje velicine ikonice

**href** - putanja do resursa

##### Primer - favicon

favicon je mala ikonica koja se prikazuje na početku tab-a pored naslova dokumenta.

```html
 <link rel="icon" type="image/x-icon" href="/images/favicon.ico">
```

#### **BODY**

Unutar \<body> taga korisnimo tagove kako bismo kreirali sadržaj dokumenta. Možemo reći i da predstavlja konterjner za sve elemente koji su vidljivi na stranici kao sto su naslovi, paragrafi, slike, hiperveze, tabele, liste itd.

> *  📖: [**W3School**](https://www.w3schools.com/html/)

---

#### **Komentari u HTML**

---

Komentar je moguće posstaviti na bilo kom mestu unutar HTML dokumenta. 

Uloga komentara je da bliže objasne HTML tekst. Takođe ukoliko želimo da sakrijemo deo stranice koji ne želimo da se više prikazuje za koji još uvek nismo spremni da obrišemo.

```html
<!-- Ovo je komentar i on se ne vidi  -->
<div class="card">
    <h2>Title</h2>
    <img src="" alt ="" >
</div>
```

## CSS

**CSS** - Cassading Style Sheet

### Tri načina kako uključiti css u HTML dokument

1.  Inline style
2.  Unutar style taga
3.  External fajl

#### Inline style

Inline stilizacija direktno utiču na tag, bez korišćenja selektora.

```html
<p style="color:red;">This is a paragraph.</p>
```

#### Style tag

```html
<!-- Used for adding in-document CSS -->
<style>
  /* ... */
</style>
```

#### External fajl

```html

<!-- Link to an external CSS file -->
<link rel="stylesheet" href="styles.css">
```

#### [**⬆ back to top**](#)

#### **Komentari u CSS**

---

Komentari nemaju uticaja na layout HTML dokumenta. Služe da bliže objasne kod ili da spreče pretraživač da interpretira određena pravila koja su deo css-a.

```css
/* Jednolinijski komentar */

/*
Komentar može da
se piše i u
više linija
*/

/* Komentar ispod služi da onemogući definisanu stilizaciju */

/*
.card {
    padding: 1rem; 
}
*/
```

## Javascript

---

Programski jezik - izvršava se u onom trenutku kada web čitač naiđe na njega.

Skripte možemo pisati unuta**r \<head>** i **\<body>** taga.

Umetanje scripte na kraj \<body> taga omogućava brže loadovanje html stranice. 

Pisanje skripte u eksternom fajlu je praktično jer isti kod možemo kosistiti na različitim web stranicama.

Eksterne skripte ne sadrže \<script> tag.

```html
<script src="script.js"></script>
<script>
 // function(s) go here
</script>
```

**Komentari u JavaScriptu**

---

Komentari se koriste da objasne JavaScript kod, kako bi bio čitljiviji programerima. Takođe se koriste da spreče izvršavanje koda.

```html
//Ovo je jednoliniski komentar

/* 
Ovo je
višelinijsi komentar
*/
```

**[⬆ back to top](#)**
