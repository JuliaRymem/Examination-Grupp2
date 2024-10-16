
![News flash](https://i.pinimg.com/originals/8b/e0/e0/8be0e0113eabf70ce1c42efdef2298d4.png)

# News flash :newspaper:
I den här övningen används HTML-element tillsammans med Tailwind och Sass för att bygga upp en nyhetssida!

### Steg 1. Gör en plan! 
Läs igenom instruktionerna och skapa en gemensam förståelse för uppgiften (skapa gärna ett design-dokument för att rita upp layouten i t ex Figma). Skapa sedan ett repo i GitHub som alla i gruppen har tillgång till. 

### Steg 2. Uppmärkning av enskilda element
Börja med att skapa content till 2 stycken artiklar. 

Använd följande element:

* ```<h1>```
* ```<p>```
* ```<img>```


Använd texten nedan eller skapa en egen "Lorem Ipsum": 
 
 ```
Lorem ipsum dolor sit amet, consectetur adipisicing elit. 
Et recusandae eius aut minus amet fuga exercitationem delectus sint eos aliquid.

Lorem ipsum dolor sit amet consectetur adipisicing elit. 
Nobis consectetur corrupti est voluptatem dolore id laudantium debitis magni 
necessitatibus ad enim exercitationem nihil provident velit similique, 
architecto placeat illum consequuntur? Aliquam voluptatem quod expedita 
minima ipsa assumenda necessitatibus delectus asperiores!

Skriven av Yngve Magnusdottir
```

### Steg 3. Uppdelning av innehåll med nesting
Efter att uppmärkningen av de enskilda elementen är färdig är det dags att fokusera på uppdelningen av innehållet (layouten). 

Använd följande element:

* ```<header>```, brukar innehålla saker som navigationslänkar och logotyp 
* ```<section>```, representerar en samling av liknande innehåll
* ```<article>```, ett innehållselement som är återanvändbart - tänk en nyhetsartikel, produkt, ett blogginlägg etc.
* ```<footer>```, brukar innehålla saker som kontaktuppgifter och dylikt

Sidans ```<header>``` ska innehålla ```The Garlic News``` som en rubrik
och sidans ```<footer>``` ska innehålla:
```
info@garlicnews.com
+850 555-1337
```

### Steg 4. Sass - preprocessor
Använd Sass för att bygga upp struktur och logik till er CSS. 
* Börja med att skapa en fil som ska innehålla den huvudsakliga stylingen, döp den till ```main.scss```

* Skapa sedan en fil som döps till ```_variables.scss```
I filen skapar ni variabler för primary color, secondary color och fonter. Importera och använd dessa i ```main.scss```

```
@import 'variables';

body {
  font-family: $font-stack;
  background-color: $secondary-color;
}
```

* Skapa ytterligare en fil som döps till ```_mixins.scss```
Använd Mixins för att skapa återanvändbar styling som:

```
@mixin flex-center {
  display: flex;
  justify-content: center;
  align-items: center;
}
```

Importera era mixins och använd i ```main.scss```

```
@import 'variables';
@import 'mixins';

article {
  font-family: $font-stack;
  background-color: $secondary-color;
  @include flex-center;
}
```

### Skriv kommandot nedan i terminalen för att kompilera er Sass till CSS:

```
sass main.scss style.css
```

### Steg 5. Tailwind - ramverk
Använd Tailwind för att styla enskilda element (testa exempelvis att lägga en bild som bakgrund i en av "boxarna"). 

Lycka till! :)
