# Struktura sadrzaja pomocu HTML5 semantickih tagova

* HTML5 tagovi omogucavaju struktuiranje dokumenta u zavisnosti od znacenja sadrzaja na stranici.
* `<div>`, `<table>` tagovi omogucavaju da kreiramo strukturu stranice, layout ali nemaju semanticko znacenje.
  
## Zasto su uvedeni?

Semantički element jasno opisuje značenje taga kako browseru tako i programeru.
* Nesemantički tagovi `<div>` , `<span>` ... - Ne govore nam ništa o sadržaju elementa.
* Semanticki elementi `<form>` , `<article>` ...  - Jasno definišu sadržaj elementa

### Potrebna nam je struktura

* HTML5 semantički elementi čine stranice čitljivijim za mašine
* Pretraživači koji indeksiraju web stranice smatraju sadržaj naslova važnim ključnim rečima za uticaj na rangiranje stranice u pretrazi. Bez naslova, vaša stranica će imati loš učinak u smislu SEO (optimizacija za pretraživače)
* Omogućavaju screen readerima da čitaju sadržaj. Osobe sa oštećenim vidom često ne čitaju veb stranice; umesto toga slušaju njih.

### Migracija HTML4 -> HTML5

| HTML4                   	| HTML5       	|
|-------------------------	|-------------	|
| `<div id="header">`     	| `<header>`  	|
| `<div id="navigation">` 	| `<nav>`     	|
| `<div class="article">` 	| `<article>` 	|
| `<div id="footer"> `    	| `<footer>`  	|
 

## Neki od semantickih elemenata

| Tag         	| Use                                     	|
|-------------	|-----------------------------------------	|
| `<main>`    	| Glavni sadrzaj stranice                 	|
| `<header>`  	| Zaglavlje dokumenta ili sekcije         	|
| `<nav>`     	| Primarna navigacija                     	|
| `<section>` 	| Definise sekciju na stranici            	|
| `<article>` 	| Definise artikal                        	|
| `<aside>`   	| Desinise sadrzaj sa strane na dokumentu 	|
| `<footer>`  	| Definise footer stranice ili sekcije    	|
  
  
  
## Header

* Može biti header dokumenta ili sekcije
* Na stranici se može pojaviti više puta


Header se koristi za uvodni sadržaj, koji bliže opisuje šta korisnik može da očekuje kada poseti naš web sajt. Najčešće je to deo u kom ćemo smestiti navigaciju i logo. A možemo uključiti i sledeće:
* Naslove (h1 - h6)
* Paragraf (p)
* Profilna slika
* Logo
* Pretraga - search
* Primarna nabvigacija
* Ime autora
* Datum 
* Social Media Links

``` html
<header>
 <p>Welcome to...</p>
 <h1>PROJECT CLASSROOM</h1>
</header>
```


``` html
<!-- Header and primary navigation -->
<body>
 <header>
  <h1>PROJECT CLASSROOM</h1>
  <nav>
   <ul>
    <li><a href="/home">Home</a>
    <li><a href="/about">About</a>
    <li><a href="/contact">Contact</a>
   </ul>
  </nav>
 </header>
</body>

```
## Main

* Glavni sadržaj dokumenta ili aplikacije
* Samo jedan po dokumentu

```html
  <header>
  </header>
  <main>
  </main>
  <footer>
  </footer>
```


## Footer

* Može biti footer dokumenta ili sekcije.
* Ne moraju biti na kraju sekcije, ali uglavnom se tamo nalaze.

Footer primarno služi za meta podatke. U njega možemo uključiti sledeće elemente:
* Copyrights informations
* Napomene
* Navigaciju sajta (razlikuje se od primarne navigacije, tj. ima niži prioritet)
* Ime autora
* social media links


```html
  <footer>Made with ❤️ by <a href=https://example.com/>Example 👻</a>.</footer>
```

## Article

* Grupise blok koji ima povezan sadrzaj
* Sadrzaj unutar <article> taga je nezavisan od ostalog sadrzaja na stanici
* Primer: blog post

## Section 

* Veoma sličan `<article>` tagu
* grupiše delove stranice
* Uglavnom se unutar section taga nalazi heading tag
* Uključivanje heading taga je dobro i za SEO
* Može da se uključi unutar article taga

