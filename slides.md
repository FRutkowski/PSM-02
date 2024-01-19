---
theme: default
background: https://images.unsplash.com/photo-1550063873-ab792950096b?q=80&w=2070&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D
class: text-center
highlighter: shikiji
lineNumbers: false
author: Filip Rutkowski
colorSchema: light
info: |
  ## Slidev Starter Template
  Presentation slides for developers.

  Learn more at [Sli.dev](https://sli.dev)
drawings:
  persist: false
transition: slide-left
title: Prezentacja JavaScript
mdc: true
config:
  styles: |
    :root {
      --slide-background: #2c3e50; /* Ustaw kolor tła prezentacji */
      --slide-text: #ecf0f1; /* Ustaw kolor tekstu na slajdach */
    }
---

# Porównanie wydajności silników JavaScript
  <div>
    Dyplomant: inż. Filip Rutkowski
  </div>
  <div>
    Promotor: dr. inż Tomasz Grześ
  </div>
  <div class="pt-12">
    <span @click="$slidev.nav.next" class="px-2 py-1 rounded cursor-pointer" hover="bg-white bg-opacity-10">
      Press Space for next page <carbon:arrow-right class="inline"/>
    </span>
  </div>

  <div class="abs-br m-6 flex gap-2">
    <button @click="$slidev.nav.openInEditor()" title="Open in Editor" class="text-xl slidev-icon-btn opacity-50 !border-none !hover:text-white">
      <carbon:edit />
    </button>
    <a href="https://github.com/slidevjs/slidev" target="_blank" alt="GitHub" title="Open in GitHub"
      class="text-xl slidev-icon-btn opacity-50 !border-none !hover:text-white">
      <carbon-logo-github />
    </a>
  </div>

<!--
The last comment block of each slide will be treated as slide notes. It will be visible and editable in Presenter Mode along with the slide. [Read more in the docs](https://sli.dev/guide/syntax.html#notes)
-->

---
transition: fade-out
---
<h1 class="text-purple">Co to jest JavaScript</h1>
<!-- # Co to jest JavaScript? -->

JavaScript jest językiem kompilowanym, który czasami jest mylony z językiem interpretowanym, gdyż kompiluje się za każdym razem, gdy jest wykonywany. 

Podstawowymi zaletami JS są jego:
<v-clicks>

- 🎨 **Wszechstronność** - Może być on używany zarówno po stronie klienta(w przeglądarkach internetowych) jak i po stronie serwera(Node.js)
- ⏳ **Asynchroniczność** - obsługa asynchroniczności za pomocą callbaków i obietnic(Promise) oraz async/await
- 🔀 **Dynamiczne typowanie danych** - jedna zmienna w przeciągu swojego życia może posiadać wartości różnych typów
- 🤹‍♂️ **Interakcja z DOM** - JavaScript umożliwia interakcję z modelem obiektowym dokumentu (DOM), co pozwala na dynamiczną modyfikację treści i struktury stron internetowych.
- 🧑‍💻 **Wsparcie dla programowania obiektowego** - JavaScript jest językiem programowania obiektowego, co umożliwia tworzenie bardziej zorganizowanego i modularnego kodu.

</v-clicks>


<br>
<br>


---
layout: default
---

<h1 class="text-purple">Przykładowy kod w JavaScript</h1> 

```js {all|1|1|1|2-3|2-3|2-3|5-9|6|1-12|14-15|17-21}
function generateRandomPassword(length) {
  const charset = "abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789";
  let password = "";

  for (let i = 0; i < length; i++) {
    var hello = 20
    const randomIndex = Math.floor(Math.random() * charset.length);
    password += charset[randomIndex];
  }

  return password;
}

const passwordLength = 12;
const randomPassword = generateRandomPassword(passwordLength);

console.log('2' === 2) // False
console.log('2' == 2) // True
console.log('' == false) // True
console.log('NoEmpty' == false) // False

```

<arrow v-click="[1, 2]" x1="280" y1="220" x2="110" y2="130" color="#564" width="3" arrowSize="1" />
<arrow v-click="[2, 3]" x1="400" y1="220" x2="230" y2="130" color="#564" width="3" arrowSize="1" />
<arrow v-click="[3, 4]" x1="500" y1="220" x2="330" y2="130" color="#564" width="3" arrowSize="1" />
<arrow v-click="[5, 6]" x1="280" y1="230" x2="110" y2="140" color="#564" width="3" arrowSize="1" />
<arrow v-click="[6, 7]" x1="265" y1="250" x2="95" y2="160" color="#564" width="3" arrowSize="1" />
<arrow v-click="[8, 9]" x1="280" y1="304" x2="110" y2="214" color="#564" width="3" arrowSize="1" />

<style>
.footnotes-sep {
  @apply mt-20 opacity-10;
}
.footnotes {
  @apply text-sm opacity-75;
}
.footnote-backref {
  display: none;
}
</style>

---
layout: image-right
image: https://images.unsplash.com/photo-1482745637430-91c0bbcea3e1?q=80&w=2070&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D
---

# Frameworki

JavaScript posiada także frameworki, które ułatwiają pisanie kodu w nim.

Najbardziej popularnymi są frameworki frontendowe Angular, Vue i React.

<img src="https://relevant.software/wp-content/uploads/2018/04/0_9N9J9YiGJrISLIBP.png">

---
layout: image-right
image: https://plus.unsplash.com/premium_photo-1671439543718-9e4d009827e8?q=80&w=2113&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D
---

# Silniki
Silniki JavaScriptowe to programy komputerowe, które interpretują i wykonują kod napisany w języku JavaScript. Silniki JavaScriptowe są niezbędne do przetwarzania i wykonania tego kodu w środowisku przeglądarki internetowej.

---
layout: default
---
# Przykładowe silniki


Silniki jakie można wyróżnić to:
<v-clicks> 

<div>
<div class="flex pt-10">
 <div class="text-xs pt-1 pr-1">◼</div>
	
   <div class="">
     <img class="w-6 h-6" :src="'./components/V8-logo.png'"/> 
   </div>  
   <div class="font-bold pr-2">
     V8
   </div>
   <div> - V8 to silnik JavaScript stworzony przez Google. Jest on używany w przeglądarkach internetowych  </div>
 </div> 

<div> opartych na Chromium, takich jak Google Chrome i Opera. V8 jest znany ze swojej szybkości wykonania kodu JavaScript dzięki technologiom takim jak kompilacja do natywnego kodu maszynowego.  </div>
</div>

<div>
<div class="flex pt-10">
 <div class="text-xs pt-1 pr-1">◼</div>
	
   <div class="">
     <img class="w-6 h-6" :src="'./components/spidermonkey-logo.png'"/> 
   </div>  
   <div class="font-bold pr-2">
     SpiderMonkey  
   </div>
   <div> - Jest to silnik JavaScript używany w przeglądarkach Mozilla Firefox. SpiderMonkey jest   </div>
 </div> 

<div> jednym z najstarszych silników JavaScript i rozwijany jest przez Mozilla Foundation. Został on napisany w językach C++, Rust i JavaScript. </div>
</div>

<div>
<div class="flex pt-10">
 <div class="text-xs pt-1 pr-1">◼</div>
	
   <div class="">
     <img class="w-6 h-6" :src="'./components/apple-logo.png'"/> 
   </div>  
   <div class="font-bold pr-2">
     JavaScriptCore  
   </div>
   <div> - Silnik ten jest używany w przeglądarkach Safari firmy Apple. Jest również znany jako </div>
 </div> 

<div> Nitro. JavaScriptCore jest częścią projektu WebKit, który obejmuje również renderowanie stron internetowych. </div>
</div>

</v-clicks>

<!-- <div grid="~ cols-2 gap-4">
<div>

You can use Vue components directly inside your slides.

We have provided a few built-in components like `<Tweet/>` and `<Youtube/>` that you can use directly. And adding your custom components is also super easy.

```html
<Counter :count="10" />
``` -->

<!-- ./components/Counter.vue -->
<!-- <Counter :count="10" m="t-4" />

Check out [the guides](https://sli.dev/builtin/components.html) for more.

</div>
<div>

```html
<Tweet id="1390115482657726468" />
```

<Tweet id="1390115482657726468" scale="0.65" />

</div>
</div> -->

<!--
Presenter note with **bold**, *italic*, and ~~striked~~ text.

Also, HTML elements are valid:
<div class="flex w-full">
  <span style="flex-grow: 1;">Left content</span>
  <span>Right content</span>
</div>
-->

---
layout: iframe-right
url: https://hermesengine.dev/
preload: false
transition: slide-up
---

# HermesEngine

Hermes to silnik JavaScript typu open source zoptymalizowany pod kątem React Native. W przypadku wielu aplikacji korzystanie z Hermes spowoduje skrócenie czasu uruchamiania, zmniejszenie zużycia pamięci i mniejszy rozmiar aplikacji w porównaniu z JavaScriptCore. Hermes jest domyślnie używany przez React Native i nie jest wymagana żadna dodatkowa konfiguracja, aby go włączyć.

---
layout: image
image: ./components/image-grayscale.png
---
<h1 class="text-white">Cel pracy</h1>
Temat pracy koncentruje się na analizie porównawczej wydajności czterech silników JavaScriptowych: SpiderMonkey, V8, JavaScriptCore oraz HermesEngine. Badanie ma na celu ocenę wydajności nowego silnika, tj. HermesEngine, względem starszych rozwiązań. Analiza uwzględnia różne parametry wydajności, takie jak szybkość wykonywania operacji, optymalizacja zarządzania pamięcią oraz zgodność ze standardami. Pozwoli to na określenie, który silnik jest najlepszy w zależności od tych parametrów, co skutkuje tym, że programista będzie miał świadomość, na co powinien zwracać uwagę, gdy tworzy oprogramowanie dla różnych przeglądarek internetowych. Poza tym badanie uświadomi, jak wielkie możliwości ma nowy silnik, gdyż aktualnie nie jest on jeszcze popularnym rozwiązaniem.
---
transition: fade-out
---

# Benchmark.js

Benchmark.js to biblioteka JavaScript stworzona do pomiaru wydajności różnych fragmentów kodu w środowisku przeglądarki internetowej lub w środowisku Node.js. Pozwala na przeprowadzanie testów wydajnościowych, porównywanie czasów wykonania operacji oraz identyfikowanie potencjalnych obszarów optymalizacji. Biblioteka ta jest przydatna dla programistów, którzy chcą zoptymalizować swoje aplikacje lub porównać wydajność różnych rozwiązań.

<div>Posiada:</div>

<v-clicks>

- 🛠️ **Łatwość użycia** - Benchmark.js oferuje prostą i zwięzłą składnię do definiowania testów wydajnościowych.
- 📊 **Porównywanie testów** - Pozwala na definiowanie wielu testów i porównywanie ich wyników, co umożliwia identyfikację różnic w wydajności między różnymi fragmentami kodu.
- 📏 **Dokładne pomiary czasu** - Benchmark.js dba o dokładność pomiarów czasu wykonania, co pozwala na uzyskanie precyzyjnych wyników testów.
- 🐬 **Wsparcie dla różnych środowisk** - Może być używane zarówno w przeglądarkach internetowych (np. w narzędziach deweloperskich) jak i w środowisku Node.js, co ułatwia testowanie wydajności w różnych kontekstach.

</v-clicks>

---
transition: fade-out
layout: image-right
image: https://images.unsplash.com/photo-1519389950473-47ba0277781c?q=80&w=2070&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D
---

# Wbudowane devtools

Można pomyśleć, że sprawdzenia wydajności optymalizacji zarządzania pamięcią można wykorzystać narzędzia deweloperskie, które są wbudowane w daną przeglądarkę. Dla przeglądarkach opartych na Chromium(silnik V8) będzie to Chrome DevTools, dla Firefox(Spider Monkey) będzie to Firefox DevTools i dla Safari(JavaScriptCore) - Safari Developer Tools. Natomiast Hermes jest ściśle połączony z React Native i aby go uruchomić, należy stworzyć odpowiednią konfigurację. Jednak, gdy aplikacja pracuje na HermesEngine, możliwość debugowania go, jest dostępna w Google Chrome.
---
transition: fade-out
layout: image-right
image: https://images.unsplash.com/photo-1460925895917-afdab827c52f?q=80&w=2015&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D
---

# Overhead

Sposób wydaje się na pierwszy rzut oka mający sens, jednak problemem jest to, że każda przeglądarka sama w sobie zużywa zasoby, co sprawia, że wyniki nie byłyby wiarygodne. Z tego powodu należy szukać innych sposobów na przetestowanie tych silników.

---

# Ręczna kompilacja silników

Aby warunki do testowania były dobre, należy ręcznie skompilować te silniki, na jednej maszynie, po czym przeprowadzić odpowiednie testy. 

<v-clicks> 

<div>
<div class="flex pt-10">
 <div class="text-xs pt-1 pr-1">◼</div>
	
   <div class="">
     <img class="w-6 h-6" :src="'./components/V8-logo.png'"/> 
   </div>  
   <div class="font-bold pr-2">
     V8
   </div>
   <div> - Jest napisany w C++ oraz posiada repozytorium otwartoźródlowe repozytorium na Githubie, które </div>
 </div> 

<div> można skolonować i ręcznie skompilować. </div>
</div>

<div>
<div class="flex pt-10">
 <div class="text-xs pt-1 pr-1">◼</div>
	
   <div class="">
     <img class="w-6 h-6" :src="'./components/spidermonkey-logo.png'"/> 
   </div>  
   <div class="font-bold pr-2">
     SpiderMonkey  
   </div>
   <div> - Na oficjalnej stronie SpiderMonkey jest dostęp do oficjalnego kodu, który można   </div>
 </div> 

<div> skompilować. Na stronie mozilli w dokumentacji jest cała instrukcja, jak krok po kroku to zrobić.  </div>
</div>

<div>
<div class="flex pt-10">
 <div class="text-xs pt-1 pr-1">◼</div>
	
   <div class="">
     <img class="w-6 h-6" :src="'./components/apple-logo.png'"/> 
   </div>  
   <div class="font-bold pr-2">
     JavaScriptCore  
   </div>
   <div> - Bazuje on na wieloplatformowym silniku webowym WebKit. Można go skompilować    </div>
 </div> 

<div> korzystając z GTK Port - zgodnie z instrukcją zawartą w README.md na stronie repozytorium. </div>
</div>

<div>
<div class="flex pt-10">
 <div class="text-xs pt-1 pr-1">◼</div>
	
   <div class="">
     <img class="w-6 h-6" :src="'./components/hermes.png'"/> 
   </div>  
   <div class="font-bold pr-2">
     Hermes  
   </div>
   <div> - Można go znaleźć pod linkiem https://github.com/facebook/hermes,   </div>
 </div> 

<div> Tutaj także instrukcja jest jasno opisana, wszystkie kroki opisane zostały w README.md </div>
</div>

</v-clicks>

---
layout: default
transition: slide-up
---

# Plan na realizację pracy

- **Kompilacja silników**
- **Przygotowanie testów**
- **Wybór technologii do testowania** 
- **Przeprowadzenie testów**
- **Dokumentacja**
---
layout: end
transition: slide-up
background: https://images.unsplash.com/photo-1655196601100-8bfb26cf99e9?q=80&w=1931&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D
---

# Dziękuję za uwagę

Filip Rutkowski
---
