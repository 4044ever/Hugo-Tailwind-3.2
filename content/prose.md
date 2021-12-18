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

##### Code snippets show the ` for some reason: 

`<tca focal="17" model="poly3" vb="1.0000" vr="1.00073"/>`

The above code wraps in &lt;code&gt; tags.

The code sample below wraps in &lt;pre&gt;&lt;code&gt;:  

    "scripts": {
    "dev": "concurrently npm:watch:*",
    "watch:tw": "tailwindcss -i ./assets/css/main.css -o ./assets/css/output.css --watch",
    "watch:hugo": "hugo server",

Click for more about: [@tailwindcss/typography](https://tailwindcss.com/docs/typography-plugin)  

### ~~ The End ~~