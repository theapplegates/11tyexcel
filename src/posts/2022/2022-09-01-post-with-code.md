---
title: 'Post with some code'
description: 'Syntax Highlighting is achieved by a pack of Eleventy plugins. No browser/client JavaScript, highlight transformations are all done at build-time.'
date: 2022-09-01
tags: ['sytnax highlighting', 'feature']
---
![Italy](https://applegate-paul.mo.cloudinary.net/zoom/Beautiful_Italy.jpg)

![Italy 2](https://res.cloudinary.com/paulapplegate-com/image/upload/c_limit/dpr_auto/f_auto,q_auto/w_auto:breakpoints_200_1920_30_15/Beautiful_Italy.jpg)

<img data-src="https://res.cloudinary.com/paulapplegate-com/image/upload/c_limit,w_auto/dpr_auto,f_auto,q_auto/hillshire-farm-2_fx2mno.jpg" class="cld-responsive">

<img data-src="https://res.cloudinary.com/paulapplegate-com/image/upload/c_limit,w_auto/dpr_auto,f_auto,q_auto/claudio-schwarz-b_qczKSP_X4-unsplash_hozv15.jpg" class="cld-responsive">
<img data-src="https://res.cloudinary.com/paulapplegate-com/image/upload/c_limit,w_auto/dpr_auto,f_auto,q_auto/DaPlane.jpg" class="cld-responsive">
<img data-src="https://res.cloudinary.com/paulapplegate-com/image/upload/c_limit,w_auto/dpr_auto,f_auto,q_auto/i0dohywpq5oldnhgleze.jpg" class="cld-responsive">




This theme uses 11ty's [Syntax Highlighting Plugin](https://www.11ty.dev/docs/plugins/syntaxhighlight/), a pack of Eleventy plugins for PrismJS syntax highlighting. No browser/client JavaScript, highlight transformations are all done at build-time.

```js
const cards = [...document.querySelectorAll('.card')];
cards.forEach(card => {
  card.style.cursor = 'pointer';
  let down,
    up,
    link = card.querySelector('a');
  card.onmousedown = () => (down = +new Date());
  card.onmouseup = () => {
    up = +new Date();
    if (up - down < 200) {
      link.click();
    }
  };
});

// © Heydon Pickering
```

```css
.smol-container {
  width: min(100% - 3rem, var(--container-max, 60ch));
  margin-inline: auto;
}

/* © Stephanie Eckles, https://smolcss.dev/ */
```

Edit styles in `css/blocks/code.css`
