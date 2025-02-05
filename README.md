# Logseq Presentation Mode Fixer

A batch of CSS files developed to fix [Logseq](https://github.com/logseq/logseq/)'s presentation mode.
The default theme is transparent and inherits the look of your favorite Logseq themes!

## Goals

- Make the Presentation Mode of Logseq behave more like vanilla [reveal.js](https://github.com/hakimel/reveal.js/) while preserving Logseq's unique features.
- Avoid using `!important` to prevent complications with the user's `custom.css` file and themes.
  
## See it in Action

[Online demo hosted on GitHub Pages](https://peter-yanase.github.io/Logseq-Presentation-Mode-Fixer/)

## How to Use?

1. Unzip the release version inside your graph's `assets` folder.
2. Add the following line __the very top__ of your `custom.css` file:
  `@import "../assets/pmfixer/pmfixer.css";`

By default, the code blocks have transparent backgrounds.
I highly advise using a [highlight.js](https://github.com/highlightjs/highlight.js) theme together with the pmfixer to improve readability.
The Monokai theme is bundled in the release for testing purposes.

Add the following __after__ the above code in your `custom.css` to overlay the Monokai theme _for your code blocks_:
`@import "../assets/pmfixer/monokai.css";`

You can replace Monokai with any of the styles available at [https://github.com/highlightjs/highlight.js/tree/main/src/styles](https://github.com/highlightjs/highlight.js/tree/main/src/styles).

## Upcoming

- reveal.js default themes
- Reveal.js docs samples redone in Logseq.

## TODO

- Fix edge cases.
