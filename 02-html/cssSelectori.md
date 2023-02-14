# CSS

* CSS je markup jezik (jezik za označavanje) koj koristimo za stilizovanje HTML dokumenta
* CSS-om opisujemo kako želimo da se HTML element prikazuje (gde da bude pozicioniran, koje boje, veličine itd)

## CSS Selektori

CSS selektori nam pružaju različite mogućnost da stilizujemo HTML elemete. 

## Osnovni selektori 

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

Da bismo selektovali odredjeni element koji sadrzi odredjenu vrednost atributa klase navodimo tacku (.) zatim sledi naziv klase.


```css
.text-green {
  color: green;
}
```

```html
<p class="text-green">Ja sam text zelene boje</p>
<h2 class="text-green">I ja sam text zelene boje</h2>
```

Napomena: 
* Naziv klase ne sme poceti brojem.


### 4. Univerzalni selektor 

Univerzalni selektor omogucava da selektujemo sve elemente na stranici.

```css
* {
  text-align: center;
}
```

Svi elementi na stranici ce biti centrirani.

## Grupisanje selektora


Kada više elemenata na stranci imaju istu css definiciju možemo da ih grupisemo.

Umesto ovog:
```css
h1 {
  margin: 0;
  padding: 0;
}

h2 {
  margin: 0;
  padding: 0;
}

p {
  margin: 0;
  padding: 0;
}
```

```css
h1, h2, p {
  margin: 0;
  padding: 0;
}

```







