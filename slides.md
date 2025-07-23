---
# You can also start simply with 'default'
theme: default
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
background: /assets/intro.jpg
# some information about your slides (markdown enabled)
title: Software Development | Foundations
info: |
  ## Software Development | Foundations
# apply unocss classes to the current slide
class: text-left
drawings:
  persist: false
transition: slide-left
mdc: true
---

# React: CSS Styling and Component Frameworks 
Frontend Development: Unit 06 - Lesson 04

- [ ] Various ways of styling with CSS
- [ ] Styling with CSS Modules
- [ ] MaterialUI + PrimeReact 

<div class="abs-br m-6 text-xl">
  <a href="https://github.com/slidevjs/slidev" target="_blank" class="slidev-icon-btn">
    <carbon:logo-github />
  </a>
</div>

<!--
-->


---
transition: slide-left
---

# Recap

- repo of where we left off: https://github.com/avcoder/test-react

---
layout: image-right
transition: slide-left
image: /assets/cory.png
backgroundSize: 420px 500px
class: text-left
---

# 10 minute break

🍦 Cool Tips, Trends and Resources:

- 🥊 [Function Component React vs Class Component React](https://www.freecodecamp.org/news/function-component-vs-class-component-in-react/)
- 📊 [State of Devs 2025](https://2025.stateofdevs.com/en-US)
- 🦮 [useState guide](https://blog.logrocket.com/guide-usestate-react/)



<br>
<hr>
<br>

- 🧪 [Enter anonymous lab questions](https://docs.google.com/forms/d/e/1FAIpQLSevvGARdHQikso-uLqFCO481MABKE5HofuSrlzEPMNQ2ZLykw/viewform?usp=dialog)
- ℹ️ [Course feedback survey](https://circuitstream.typeform.com/to/ZoyYk7px#course_id=SoftwareAN&instructor=9514)


---
transition: slide-left
---

# Common Gotchas
Try the following common errors to see what errors look like in React.  Find solutions for each.

- Forgetting to `return` JSX
- Confusing camelCase for HTML attributes `onclick vs onClick`
- Using `class` instead of `className`
- if using inline styles, using hyphenated names instead of camelCase 
  - ex: `background-color vs backgroundColor`
- Multiple top-level elements without a wrapper/fragment
- DON'T use if statements directly inside JSX like `return ( if (isLoggedIn) { <p>Welcome</p> });`
- Not using `key` in lists
- JSX requires properly closed tags, even for void elements. ex: `<input /> <br />`
- what happens if props are undefined? ex: `return (<div className={someUndefinedClass}>Hi</div>)`
- if `numOfItems` is 0, this will render 0 `{numOfItems && <ShoppingList items={shoppingList} />}`
- examine if there are any more red squiggly lines in VSCode? 



---
transition: slide-left
---

# Exercise: Lifting State Up
Parent-Child communication means having a parent component manage the state, and pass down state setters as props

- see https://unit06-lesson02.netlify.app/4
- Identify where state needs to located, and where state needs to be lifted up

---
transition: slide-left
---

# Optional: Configure imports to use absolute path

- Use ChatGPT to help you configure your tsconfig.json, tsconfig.app.json, vite.config.ts
- ❌ BEFORE: Using relative paths can be a pain point, especially when refactoring locations of files/folders
- ✅ AFTER: should now be able to use `import Component from '@/components/whatever' 




---
transition: slide-left
---

# Homework

- Finish converting to JSX [Email template layout](https://pure-css.github.io/layouts/email/) to JSX; [Github code here](https://github.com/pure-css/pure/tree/main/site/static/layouts/email)
- Begin thinking about your "Weather Forecasting App" assignment due Aug 17 midnight EST
