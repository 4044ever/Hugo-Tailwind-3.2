# Hugo & Tailwind-3.0


A barebone Hugo & Tailwind CSS 3.0 starter kit

Download and install in VS Code

To start developing:
npm run start

To generate the site HTML:
npm run build

npm run start will run two command parallel:
npx tailwindcss -i ./assets/css/main.css -o ./assets/css/style.css --watch

and
hugo server

Note: When you start npm run start a style.css must exist - or you get an error! Just do a Ctrl+C and run npm run start - even though you got an error but a style was written anyway and 2nd time round it should start fine.

To get out of developing mode you need to do Ctrl+C twice.
