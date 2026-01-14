https://tailwindcss.com/docs/installation/using-vite
https://tailwindcss.com/docs/installation/framework-guides
https://tailwindcss.com/docs/installation/framework-guides/nextjs
https://tailwindcss.com/docs/installation/framework-guides/astro

[solo este curso]: #

[tailwind-cli](https://tailwindcss.com/docs/installation/tailwind-cli)

0. crear archivo (index.html) rellenar-lo con ! + tab
1. reiniciar node, T: npm init -y
2. instalar tailwind, T: npm install tailwindcss @tailwindcss/cli
   3 crear archivo "src/styles.css" i rellenar con: @import "tailwindcss";
3. package.json:
   add: "tailwindcss -i ./src/styles.css -o ./dist/output.css --watch"

```
"scripts": {
    "test": "echo \"Error: no test specified\" && exit 1",
    "dev": "tailwindcss -i ./src/styles.css -o ./dist/output.css --watch"
  },
```

5. crear carpeta y doc de salida,t: npm run dev
6. hacerlouput minimizado:
   - package.json:
     add: "build": "tailwindcss -i ./src/styles.css -o ./dist/output.css --minify"

   ```
    "scripts": {
    "test": "echo \"Error: no test specified\" && exit 1",
    "dev": "tailwindcss -i ./src/styles.css -o ./dist/output.css --watch",
    "build": "tailwindcss -i ./src/styles.css -o ./dist/output.css --minify"
   ```

   - T:npm run build

7. modificar en "/src/index.html":
   add: <link href="../dist/output.css" rel="stylesheet" />

`````
 <link href="../dist/output.css" rel="stylesheet" />
  </head>
  <body>
    <h1 class="text-3xl font-bold underline">Hello, World!</h1>
	````

8. arranque, T: npm run dev

//https://github.com/tailwindlabs/prettier-plugin-tailwindcss
9. instalar plugin tailwind prettier:npm install -D prettier prettier-plugin-tailwindcss
10. crearen raiz y modificar ".prettierrc":
`````

{
"plugins": ["prettier-plugin-tailwindcss"]
}

```

11. VS/settings/B: format on save
check
format on save mode: file

12. ".gitignore":
```

dist/
node_modules/
.env

```
13. inicializar git, T: git init

14. palete comand: Live server: open with live server

15. add "src/styles.css":

```

@layer base {
body {
@apply bg-slate-800 px-4 py-2 text-white;
}
}

@layer components {
.card {
@apply bg-slate-700 p-4 rounded-lg shadow-lg;
}
}

card class="card"

```





```
