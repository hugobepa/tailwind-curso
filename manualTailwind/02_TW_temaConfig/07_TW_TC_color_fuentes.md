# CUSTOM COLOR

0. añadir colores al "/src/styles.css":

```

@theme {
  --color-gold-50: oklch(98.5% 0.02 100);
  --color-gold-100: oklch(96.7% 0.035 100);
  --color-gold-200: oklch(92.5% 0.07 100);
  --color-gold-300: oklch(87.1% 0.107 100);
  --color-gold-400: oklch(80.5% 0.14 100);
  --color-gold-500: oklch(73.2% 0.175 100);
  --color-gold-600: oklch(65.5% 0.18 100);
  --color-gold-700: oklch(54.1% 0.17 100);
  --color-gold-800: oklch(42.5% 0.13 100);
  --color-gold-900: oklch(27.2% 0.09 100);
  --color-gold-950: oklch(16% 0.06 100);
  --color-gold-950: oklch(0.01 0.005 123.39);

}
```

1. llamar "/src/styles.css" en web: ` head <link rel="stylesheet" href="../../dist/output.css" />`

2. usar colores cutomizados: ` <button class="rounded-md bg-gold-50  text-gold-500">`

# FUENTES

(google fuentes)[https://fonts.google.com/]
(monserrat font)[https://fonts.google.com/specimen/Montserrat+Alternates]
(font family tailwind)[https://tailwindcss.com/docs/font-family]

0. escoger funente google [https://fonts.google.com/]:

```
- gent font
- get embed code
- web --- import:
      - change styles: escoger(thin100, light300,regular400,bold700))

-url  de web import canvia con las escogidas
```

1. añadir fuentes al "/src/styles.css":

- la primera fuente es la principal, las posteriores si falla la primera

```
@import url("https://fonts.googleapis.com/css2?family=Montserrat+Alternates:wght@100;300;400;700&display=swap");
@import "tailwindcss";
...
@theme {
  ...
  //obligatorio --font , lo demas puede ser inventado: "nombre igual de la fuente copiada"
  --font-montserrat-alternatives: "Montserrat Alternates", sans-serif;
}
```

2. utilizar fuentes en la web : `<p class="font-montserrat-alternatives font-thin">`
   - font-thin,font-light,font-normal,font-bold
