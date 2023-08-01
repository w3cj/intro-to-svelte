#### To view this as a slide deck:

`npm install`

`npm start`

---

<!-- .slide: data-background-video="https://cdn.flixel.com/flixel/ogd95qysaotxsgbycmxq.hd.mp4" data-background-video-loop="loop" data-background-video-muted -->

# Intro to

<img src="./svelte-logo.png" style="height:200px;" class="slide-img"/>

<center>
  <div style="background:rgba(0,0,0,0.8);width:400px;padding:20px;font-size:0.8em !important;">
    <code>cj@null.computer</code>
    <br />
    git.io/w3cj
    <br />
    <br />
    https://coding.garden
  </div>
</center>

---

<!-- .slide: data-background-video="https://cdn.flixel.com/flixel/ts1p4x68ezcwbofpgaw2.hd.mp4" data-background-video-loop="loop" data-background-video-muted -->

## Agenda

* whoami
* Who are you?
* What is Svelte?
* A Brief History of Svelte
* Intro to Svelte
* Svelte Community and Beyond

---

<!-- .slide: data-background-video="https://cdn.flixel.com/flixel/52vy4yxt8yw76d2u8dsm.tablet.mp4" data-background-video-loop="loop" data-background-video-muted -->

<div class="dark-bg">
  Hello friends! <span class="emoji">👋</span>
</div>

<div class="dark-bg fragment">
  I am a <strong>Full Stack Developer <span class="emoji">🥞</span></strong>,
  <strong>Educator <span class="emoji">🏫</span></strong>, and
  <strong>Maker <span class="emoji">🛠</span>
  </strong> based in the <strong>Denver <span class="emoji">🏔</span></strong> area.
</div>

----

### Coding Garden

<a href="https://YouTube.com/@CodingGarden">YouTube.com/@CodingGarden</a>

More info at https://coding.garden

<img src="https://i.ytimg.com/vi/_4M46HRHoIw/maxresdefault.jpg" style="max-width:35%">
<img src="https://i.ytimg.com/vi/B-T69_VP2Ls/maxresdefault.jpg" style="max-width:35%">
<img src="https://i.ytimg.com/vi/gcNI4rUNqQE/maxresdefault.jpg" style="max-width:35%">
<img src="https://i.ytimg.com/vi/GZM2u6QtIV8/maxresdefault.jpg" style="max-width:35%">

----

## Background

* 3+ years building with Angular 1.x
* Building with React since 2016
* Building with Vue.js since 2017
* Building with Svelte since 2019

---

<!-- .slide: data-background-video="https://cdn.flixel.com/flixel/14hemjzawc4tl7heatqw.hd.mp4" data-background-video-loop="loop" data-background-video-muted -->

<div style="background: rgba(0, 0, 0, 0.4);">
  <h1>Who are you?</h1>
</div>

----

## Show of hands:
# Who writes JavaScript daily?

----

## Show of hands:
# Who has used a front-end JS framework?

----

## Show of hands:
# Who uses React daily?

----

## Show of hands:
# Who uses Vue daily?

----

## Show of hands:
# Who uses Angular daily?

----

## Show of hands:
# Who has heard of Svelte before this talk?

----

## Show of hands:
# Who has never used Svelte?

----

## Show of hands:
# Who has used Svelte in a project?

----

## Show of hands:
# Who uses Svelte daily?

---

<!-- .slide: data-background-video="https://cdn.flixel.com/flixel/sjytbnalz6tpbgl9jqzn.hd.mp4" data-background-video-loop="loop" data-background-video-muted -->

<div class="dark-bg">
  <h1>What is Svelte?</h1>
</div>

----

# Cybernetically enhanced web apps

----

<img src="https://i.imgur.com/kIqu3A8.png" class="slide-img" />

----

# Compiled

Svelte shifts as much work as possible out of the browser and into your build step. No more manual optimisations - just faster, more efficient apps.

----

# Compact

Write breathtakingly concise components using languages you already know - HTML, CSS and JavaScript.

----

# Complete

Built-in scoped styling, state management, motion primitives, form bindings and more.

---

<!-- .slide: data-background-video="https://cdn.flixel.com/flixel/h1pnkz1q4exz9wy0d70a.hd.mp4" data-background-video-loop="loop" data-background-video-muted -->

# A Brief History of Svelte

----

* Created by Rich Harris in late 2016.
  * November 2016 - [Svelte v1](https://svelte.dev/blog/frameworks-without-the-framework)
* April 2018 - [Svelte v2](https://svelte.dev/blog/version-2)
  * Dropped mustache template syntax in favor of single brackets
* April 2019 - [Svelte v3](https://svelte.dev/blog/svelte-3-rethinking-reactivity)
  * Major re-write, many breaking changes
  * You probably started hearing about Svelte around this time
* July 2020 - [TypeScript support added](https://svelte.dev/blog/svelte-and-typescript)
* November 2020 - Svelte Summit
  * SvelteKit initial demo / announcement
* December 2022 - [SvelteKit Reaches v1.0](https://svelte.dev/blog/announcing-sveltekit-1.0)
* June 2023 - [Svelte v4](https://svelte.dev/blog/svelte-4)
  * No major breaking changes.
  * Improved performance, developer experience, documentation and tutorials

----

# Svelte Today

* [Github](https://github.com/sveltejs/svelte)
* [Github Star history](https://star-history.com/#sveltejs/svelte&Date)
* [npm](https://www.npmjs.com/package/svelte)

---

<!-- .slide: data-background-video="https://cdn.flixel.com/flixel/jjihphnwquisxx0xyxtg.phone.mp4" data-background-video-loop="loop" data-background-video-muted -->

# Intro to Svelte

* Getting Started
* Components
* Reactivity
* Logic
* Bindings
* Transitions
* Beyond Svelte
* Community

---

<!-- .slide: data-background-video="https://cdn.flixel.com/flixel/1732iv96pd4mp6zx6xwa.hd.mp4" data-background-video-loop="loop" data-background-video-muted -->

## Getting Started

----

```svelte
<script>
	let name = 'world';
</script>

<h1>Hello {name}!</h1>
```

----

# To the [Docs](https://svelte.dev)!

----

The create-svelte package uses sveltekit... more on that later.

We'll use vite to create an app:

```sh
npm create vite@latest my-vite-app -- --template svelte
```

```sh
npm create vite@latest my-vite-app -- --template svelte-ts
```

----

Setup prettier:

```sh
npm i --save-dev prettier-plugin-svelte prettier
```

```json
{
  "plugins": ["prettier-plugin-svelte"],
  "trailingComma": "es5",
  "tabWidth": 2,
  "semi": true,
  "singleQuote": true
}
```

---

<!-- .slide: data-background-video="https://cdn.flixel.com/flixel/u08ojgwwslba0ghx53on.hd.mp4" data-background-video-loop="loop" data-background-video-muted -->

<div class="dark-bg">
  <h1>Components</h1>
</div>

----

* Single File Components (SFC)
* Attributes
* Scoped Styles
* Nesting
* Props
* DOM Events

---

<!-- .slide: data-background-video="https://cdn.flixel.com/flixel/bane1smc4639qj931ujq.hd.mp4" data-background-video-loop="loop" data-background-video-muted -->

# Reactivity

----

* Assignments / Declarations
* Statements
* Updating Arrays and Objects

---

<!-- .slide: data-background-video="https://cdn.flixel.com/flixel/rebln7j1jqwq3c8d0fw3.tablet.mp4" data-background-video-loop="loop" data-background-video-muted -->

# Logic

----

* General Syntax
* Conditionals
* Iteration
* Await / Async

---

<!-- .slide: data-background-video="https://cdn.flixel.com/flixel/yqaf3nj6lrakowekph7r.tablet.mp4" data-background-video-loop="loop" data-background-video-muted -->

<div class="dark-bg">
  <h1>Bindings</h1>
</div>

----

* Text Inputs
* DOM Elements

---

<!-- .slide: data-background-video="https://cdn.flixel.com/flixel/crmoqzfoajbuq0uwubiz.tablet.mp4" data-background-video-loop="loop" data-background-video-muted -->

<div class="dark-bg">
  <h1>Transitions</h1>
</div>

---

<!-- .slide: data-background-video="https://cdn.flixel.com/flixel/602x1s1bl1k5j6yks6ea.hd.mp4" data-background-video-loop="loop" data-background-video-muted -->

<div class="dark-bg">
  <h1>Beyond Svelte</h1>
</div>

---

<!-- .slide: data-background-video="https://cdn.flixel.com/flixel/ez3tqe8xzerp9tark1m1.tablet.mp4" data-background-video-loop="loop" data-background-video-muted -->

<div class="dark-bg">
  <h1>Community</h1>
</div>

----

* https://sveltesociety.dev/
* Awesome Svelte
  * https://github.com/TheComputerM/awesome-svelte
  * https://github.com/rocketlaunchr/awesome-svelte

---

# ?

---


<!-- .slide: data-background-video="https://cdn.flixel.com/flixel/ogd95qysaotxsgbycmxq.hd.mp4" data-background-video-loop="loop" data-background-video-muted -->

# Thank you!

<center>
  <div style="background:rgba(0,0,0,0.8);width:400px;padding:20px;font-size:0.8em !important;">
    <code>cj@null.computer</code>
    <br />
    git.io/w3cj
    <br />
    <br />
    https://coding.garden
  </div>
</center>