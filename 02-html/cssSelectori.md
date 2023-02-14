# CSS

* CSS je markup jezik (jezik za označavanje) koj koristimo za stilizovanje HTML dokumenta
* CSS-om opisujemo kako želimo da se HTML element prikazuje (gde da bude pozicioniran, koje boje, veličine itd)

## CSS Selektori

CSS selektori nam pružaju različite mogućnost da stilizujemo HTML elemete. 

## Jednostavni selektori - 3 vrste

### 1. CSS element selector

Omogućava da selektujemo HTML element na osnovu njegovog imena.


Primer: 

```css
p {
  color: red;
}

```

```html
<p>Text crvene boje</p>
 ```


### 2. ID selector

Id je HTML atribut koji jedinstveno identifikuje HTML element.
Nije dozvoljeno da na stranici imamo vise id atributa sa istom vrednoscu!

> 📖 [https://www.w3schools.com/html/html_id](https://www.w3schools.com/html/html_id.asp)

id selektor omogucava nam da selektujemo HTML element na osnovu vrednosti id atributa.

Primer: 

```css
#naslov {
  color: blue;
}

```

```html
<h1 id="naslov">Naslov plave sam boje</h1>
 ```

Napomena: 
* Naziv id je case-sensitive (razlikuje mala i velika slova)
* Naziv ne sme sadzati razmake, tabove itd.
* Naziv mora imati barem jedan karakter.
* Naziv ne sme poceti brojem.


### 3. CLASS selector

Slektor klase omogucava da selektujemo HTML element sa odredjenim atributom klase.

Class selektor pocinje sa tackom (.) zatim sledi naziv klase.

```css
.text-green {
  color: green;
}
```

```html
<p class="text-green">Ja sam text zelene boje</p>
<h2 class="text-green">I ja sam text zelene boje</h2>
```
