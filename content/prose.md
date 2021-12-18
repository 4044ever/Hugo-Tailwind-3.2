---
title: "Prose"
date: 2021-12-18T11:10:36+08:00
draft: false
language: en
description: A test with @tailwindcss/typography & Prose
---

## A Test with Tailwind Prose Classes   

With the new [@tailwindcss/typography](https://tailwindcss.com/docs/typography-plugin) module I can add prose modifiers that will render to the output HTML. This allows you to style HTML tags individually with i.e. `prose-h*:text-color-*00`

# this is a H1 header 
## this is a H2 header
### this is a H3 header
#### this is a H4 header   

You can change link colors too and define hover with `prose prose-a:text-pink-700 hover:prose-a:text-cyan-700` - example: 
[gohugo.io](https://gohugo.io) 

##### Note that in standard prose code snippets show the ` for some reason. So in standard prose you get:

&#96;`<code>Something</code>`&#96;

But I want want:

`<code>Something</code>`

So I modified the `tailwind.config.js` to:

    module.exports = {
    content: ['./layouts/**/*.html'],
    theme: {
        extend: {
            typography: {
                DEFAULT: {
                    css: {
                        "code::before": {content: ''},
                        "code::after": {content: ''}
                    }
                }
            }
        }
    },
    plugins: [
        require('@tailwindcss/typography'),
    ],
    }

Remove those extra lines you want the &#96;`ticks`&#96;. Tailwind uses them on their website.

Click for more about: [@tailwindcss/typography](https://tailwindcss.com/docs/typography-plugin)  

### ~~ The End ~~
