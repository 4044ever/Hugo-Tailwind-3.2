# Hugo & Tailwind 3.1 (now 3.1.6!)

## A barebone Hugo & Tailwind CSS 3.1 starter kit

**Install to VS Code with:**  
`git clone https://github.com/4044ever/Hugo-Tailwind-3.0 optinal-foldername`  
`npm install`

**To start developing:**  
`npm run start`

**To generate the site HTML:**  
`npm run build`

**npm run start** will run two commands parallel:  
`npx tailwindcss -i ./assets/css/main.css -o ./assets/css/style.css --watch`

and
`hugo server`

Note: You do not have to install Hugo with `Hugo new site hugofolder` ! But you need to have the Hugo environment running!

Note: When you start first time **npm run start** a style.css must exist - or you get an error! Just do a **Ctrl+c** and run **npm run start** - even though you got an error but a style was written anyway and 2nd time round it should start fine.

To get out of developing mode you need to do **Ctrl+c** twice.

> **Disclaimer:** This is my first try with Hugo and Tailwind 3.0. To me it looks like all functions work, classes get updated, a correct `/public/` folder with purged, minified style*.css gets created. Seems production ready, you can build a theme around it. Leave a comment if you see errors or improvements. 

> **Update Notes:** If you have an older version and new Tailwind classes don't update, change in `tailwind.config.js` to `content: ['./layouts/**/*.html', './content/**/*.md']`. Allowing `HTML` in `*.md` files may help too, allow them in `config.toml`

> **Hugo Note:** Tested up to/with [Hugo 0.101.0 extended](https://github.com/gohugoio/hugo/releases/tag/v0.101.0). So far all new Hugo version worked for me.

