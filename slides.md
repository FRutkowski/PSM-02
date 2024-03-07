---
theme: default
background: https://images.unsplash.com/photo-1507838153414-b4b713384a76?q=80&w=2070&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D
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

# Aplikacja do komponowania muzyki za pomocą interfejsu z nutami
  <div>
    Dyplomant: Filip Rutkowski
  </div>
  <div>
    Promotor: dr. inż Łukasz Gadomer
  </div>
  <!-- <div class="pt-12">
    <span @click="$slidev.nav.next" class="px-2 py-1 rounded cursor-pointer" hover="bg-white bg-opacity-10">
      Press Space for next page <carbon:arrow-right class="inline"/>
    </span>
  </div> -->

  <!-- <div class="abs-br m-6 flex gap-2">
    <button @click="$slidev.nav.openInEditor()" title="Open in Editor" class="text-xl slidev-icon-btn opacity-50 !border-none !hover:text-white">
      <carbon:edit />
    </button>
    <a href="https://github.com/slidevjs/slidev" target="_blank" alt="GitHub" title="Open in GitHub"
      class="text-xl slidev-icon-btn opacity-50 !border-none !hover:text-white">
      <carbon-logo-github />
    </a>
  </div> -->

<!--
The last comment block of each slide will be treated as slide notes. It will be visible and editable in Presenter Mode along with the slide. [Read more in the docs](https://sli.dev/guide/syntax.html#notes)
-->

---
transition: fade-out
---
<h1 class="text-teal">Cel pracy</h1>
Celem pracy było stworzenie aplikacji do komponowania utworów muzycznych
za pomocą interfejsu z nutami. Ponadto obejmował on określenie
wymagań, jakie dokładnie powinno spełniać tworzone oprogramowanie,
analizę rynku, a także zaprojektowanie aplikacji.
MusicForm to aplikacja umożliwiająca tworzenie kompozycji muzycznych za
pomocą nut. Udostępnia 6 instrumentów, dzięki którym można odsłuchać
tworzony utwór. Ponadto program umożliwia dodawanie nut za pomocą
myszy, tworzenie melodi oraz dodawanie akordów. Wspiera różną ilość
tonacji, jak i znaki chromatyczne. Dzięki zapisowi do pliku użytkownik posiada
możliwość pracy nad jednym utworem nawet przez wiele miesięcy.
Nie posiada tak ogromnomnej liczby funkcjonalności, jak inne
popularne aplikacje na rynku (Flat, NoteFlight oraz MuseScore), ale cechuje się
prostotą oraz zapewnia odpowiednie narzędzia do tworzenia prostych
kompozycji, a także świetnie nadaje się do nauki komponowania muzyki.

<!-- JavaScript jest językiem kompilowanym, który czasami jest mylony z językiem interpretowanym, gdyż kompiluje się za każdym razem, gdy jest wykonywany. 

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
 -->

---
layout: image-right
image: https://vuejsnation.com/images/workshop-vue.png
---

<h1 class="text-teal">Wykorzystane Technologie</h1> 

Program został zbudowany przy użyciu frameworka Vue.js oraz narzędzia Vite, które umożliwiają szybkie i efektywne rozwijanie aplikacji internetowych. Vue.js zapewnia elastyczność i wydajność w tworzeniu interaktywnych interfejsów użytkownika, natomiast Vite dostarcza narzędzi do szybkiego budowania projektu.
Do stylizacji interfejsu graficznego zastosowano UnoCSS, który pozwala na szybkie tworzenie estetycznych i responsywnych komponentów bez konieczności pisania własnych arkuszy stylów CSS.
---
layout: default
---

<h1 class="text-teal">Tone.js</h1> 

Tone.js to biblioteka JavaScript, która umożliwia interaktywną manipulację dźwiękiem w przeglądarkach internetowych. Dzięki niej programiści mogą generować dźwięki, tworzyć skomplikowane sekwencje dźwiękowe, stosować różnorodne efekty dźwiękowe oraz obsługiwać standard MIDI. Ta wszechstronna biblioteka jest niezastąpiona w projektach, gdzie dźwięk odgrywa kluczową rolę, takich jak aplikacje muzyczne, gry czy interaktywne strony internetowe. Tone.js oferuje także precyzyjne narzędzia do synchronizacji dźwięku w czasie, co pozwala na tworzenie zaawansowanych i dynamicznych doświadczeń dźwiękowych. Dzięki jego elastyczności i bogatej funkcjonalności, Tone.js stał się popularnym wyborem wśród deweloperów, którzy chcą wnieść do swoich projektów element dźwiękowy o wysokiej jakości i interaktywności.

---
layout: image-right
image: https://images.unsplash.com/photo-1694675274861-c4ceb495305c?q=80&w=1935&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D
---
<h1 class="text-teal">VexFlow</h1> 

VexFlow to biblioteka JavaScript, która umożliwia renderowanie notacji muzycznej w przeglądarkach internetowych. Jest to narzędzie stworzone specjalnie dla twórców aplikacji muzycznych i stron internetowych związanych z notacją muzyczną. Dzięki VexFlow programiści mogą generować interaktywne, wysokiej jakości wydruki nutowe, tabulatury oraz inne elementy związane z muzyką, które mogą być wyświetlane bezpośrednio w przeglądarce.
---
layout: end
transition: slide-up
background: white
---

# Dziękuję za uwagę

Filip Rutkowski
---
