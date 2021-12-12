# Hugo & Tailwind 3.0

## A barebone Hugo & Tailwind CSS 3.0 starter kit

**Install to VS Code with:**  
`git clone https://github.com/4044ever/Hugo-Tailwind-3.0`
`npm install`

**To start developing:**  
`npm run start`

**To generate the site HTML:**  
`npm run build`

**npm run start** will run two commands parallel:  
`npx tailwindcss -i ./assets/css/main.css -o ./assets/css/style.css --watch`

and
`hugo server`

Note: When you start first time **npm run start** a style.css must exist - or you get an error! Just do a **Ctrl+c** and run **npm run start** - even though you got an error but a style was written anyway and 2nd time round it should start fine.

To get out of developing mode you need to do **Ctrl+c** twice.
