---
title: Demostración
author: autor
marp: true
theme: srd-theme
backgroundImage: url(figures/fondo.png)
footer: 'Algo'
paginate: true
---

<!-- 
_class: invert 
_header: ''
_footer: ''
-->

![bg Title slide bakcground](figures/tower_bg_swap.jpeg)
![height:2cm](figures/UGR-logo-negativo.svg) 

# Demo Slideshow
`Demo` <i class="bi bi-arrow-right"></i> **A Fancy Title**


<br><br>
> Author [<i class="bi bi-envelope-fill"></i>](mailto:john@doe.es) [<i class="bi bi-house"></i>](https://www.google.es) [<i class="bi bi-github"></i>](https://github.com)
> *Affiliation*

---

# Index slide
1) [Slide 1: Overview](#3)
2) [Slide 2: How to use the theme](#4)
3) [Slide 3: Columns](#5)
4) [Slide 4: Figures](#6)
5) [Slide 5: Hiding content](#7)
6) [Slide 6: Custom alert boxes](#8)
7) [Slide 7: Vertical spacing](#9)

---

# Slide 1: Overview
The `SRD-theme` is based on the [Marp](https://marp.app/) default theme, but adds certain CSS extensions and font customization, which makes it fit for the Marpit extension for VSCode. 

## This is a subtitle
### This is a subsubtitle
- List item 1
- List item 2 with a [link](https://www.google.es)

1. **Numbered** list item 1
2. *Numbered* list item 2 with italics
3. <u>Numbered</u> list item 3 with underline

> <i class="bi bi-info-circle-fill"></i> A blockquote with an info icon 

---

# Slide 2: How to use the theme
> Instructions to use a custom theme from [Marp discussion](https://github.com/orgs/marp-team/discussions/115):

1) In VsCode, hit F1 and run "Preferences: Open Workspace Settings".

2) Search "Themes" and find out Markdown > Marp: Themes.

3) Add a path `theme.css`. Now ready to use "srd-theme". 

4) Open `demo.md`, and confirm the root of current workspace is the working folder you've made.

5) Open Markdown preview. 

```yaml
---
marp: true
theme: your-theme
---
```

---

<!-- _class: twocolumn -->
<div>

# Slide 3: Add-ons. Text columns
We have added the possibility to embed columns in the slide, using the scoped `twocolumn` class: 
`<!-- _class: twocolumn -->` and defining two different `<div>` elements, one per column. 

Suscipit nisl nostra ligula quis tellus fringilla libero. Efficitur parturient lobortis placerat class laoreet lectus pharetra turpis pulvinar. Bibendum lectus lobortis vivamus platea semper.
</div>

<div>
Additionally, it includes the usage of bootstrap icons <i class="bi bi-bootstrap"></i>, that can be added with the code 

```html
<i class="bi bi-icon-name"></i>
```

<span class="warning">

> **Important**
> This is a requirement for the usage of the [Custom alert boxes](#8).

</span>

Fringilla curae ut viverra duis augue sollicitudin netus. Mi parturient montes vitae rutrum condimentum primis eu scelerisque. Varius luctus purus ornare cubilia fames lobortis fames nostra sit. Libero aenean arcu molestie scelerisque adipiscing montes curabitur. 
</div>

---

# Slide 4: Add-ons. Figures
Apart from the regular [image syntax](https://marpit.marp.app/image-syntax), we have added a new class `center` to allow for images to be centered in the slide, with the code:  
```markdown
![center](figures/image.png)    
```
![center](figures/image.png)    

---

# Slide 5: Add-ons. Hiding content
The `hide` span class can be used to hide content from the slide, and display it only when hovering over the slide. To do so, use `<span class='hide'>`. 

- Let's hide a math formula <span class='hide'>$R = \frac{\rho l}{A}=\frac{\rho l}{\pi r^2}$</span>

And hide an image: 
<span class='hide'>![center](figures/image.png)</span>

<span class='tip'>

> **Tip**
> Mouse over the blank space to see the hidden content. 
</span>

--- 

# Slide 6: Add-ons. Custom alert boxes
We have also added several classes for qustom blockquotes (inspired by [<i class="bi bi-github"></i> GitHub](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#alerts)): 

<span class='note'>

> **Note**
> Add it with class `note`. 
</span>

<span class='tip'>

> **Tip**
> Add it with class `tip`. 
</span>

<span class='important'>

> **Important**
> Add it with class `important`. 
> You can also embed icons and links:  <i class="bi bi-people-fill"></i> [<i class="bi bi-box-arrow-up-right"></i>](https://www.online-stopwatch.com/rocket-timer/full-screen/)
</span>

<span class='warning'>

> **Warning**
> Add it with class `warning`. 
> - Add lists
> - and other items. 
</span>

<span class='error'>

> **Error** 
> Add it with class `error`. You can also add error text and 
> span multiple lines. 
</span>

---
# Slide 7: Add-ons. Vertical spacing
We have added a vertical spacing to fit full height, using a `<div>`: 
```markdown
<div class="row content"></div>
```
<div class="row content"></div>

> Now a blockquote / footnote. 

