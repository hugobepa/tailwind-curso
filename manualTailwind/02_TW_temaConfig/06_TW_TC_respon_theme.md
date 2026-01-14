# DISEÑO RESPONSIVE

https://tailwindcss.com/docs/responsive-design

| size |    minimum     |
| :--- | :------------: |
| sm   | 40rem (640px)  |
| md   | 48rem (768px)  |
| lg   | 64rem (1024px) |
| xl   | 80rem (1280px) |
| 2xl  | 96rem (1536px) |

0. al div (main) despues del body : `<div class=" sm:grid-cols-2 md:grid-cols-3 lg:grid-cols-4"`

# TEMA lIGHT-DARK

(tailwind-theme)[https://tailwindcss.com/docs/dark-mode#toggling-dark-mode-manually]

0. add al div principal o despues de body: ` <divclass=" dark:border-slate-700 dark:bg-slate-800"`
1. add dark a los elementos necesarios: ` <h2 class=" dark:text-slate-900">`

# CAMBIAR TEMA MANUALMENTE

0. texto cambiar segun tema:

```
  <h1 class="my-5 text-xl font-bold">
      Actualmente:
      <span class="block dark:hidden">Tema Light</span>
      <span class="hidden dark:block">Tema Dark</span>
    </h1>
```

1. add `@custom-variant dark (&:where(.dark, .dark \*));` en "/src/styles.css"

2. archivo js :

```
<script>
      // Todo: Agregar botón para cambiar tema aquí:
      // Docs: https://tailwindcss.com/docs/dark-mode#toggling-dark-mode-manually

      document.documentElement.classList.toggle(
        "dark",
        localStorage.theme === "dark" ||
          (!("theme" in localStorage) &&
            window.matchMedia("(prefers-color-scheme: dark)").matches),
      );

      document.querySelector("#theme-toggle").addEventListener("click", () => {
        // console.log("Click en toggle");
        document.documentElement.classList.toggle("dark");

        localStorage.theme = document.documentElement.classList.contains("dark")
          ? "dark"
          : "light";
      });
    </script>

```

3. cambiar el modo gracias `theme-toggle` en el botton: `<button id="theme-toggle"`
