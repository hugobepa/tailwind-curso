//https://tailwindcss.com/docs/hover-focus-and-other-states
https://tailwindcss.com/docs/hover-focus-and-other-states#first-last-odd-and-even

# GENERAL

0. "src/styles.css":

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

# LISTAS

tipo de lista: <ul class="list-inside list-xxxx">
solamente el primero: <li class="first:mt-4">Item 1</li>
solamente el ultimo: <li class="last:mb-4">Item 4</li>
efecto link: class="text-blue-500 hover:underline cursor-pointer">

# TABLAS

- odd : par
- even: impar

```
<thead class="bg-gray-900/35">
<thead class="bg-gray-900 opacity-40">
   <tbody>
        <!--  -->
        <tr
          class="odd:bg-white even:bg-gray-50 dark:odd:bg-gray-900/50 dark:even:bg-gray-950"
        >

         <th class="p-3 text-right">Email</th>
```

# TABLA RESPONSIVE

- convierte tabla resposive= "overflow-x-xxxx
- respeta tamaño contenido: min-w-max

```
<div class="overflow-x-auto">
 <thead class="hidden bg-gray-900/35 md:table-header-group">
     <img class="h-12 w-12 rounded-full"
      <table class="w-full min-w-max">
      class="mb-5 p-2 flex flex-col items-center justify-center md:table-row
       <td class="capitalize">Juan Pérez</td>
            <td>28</td>
            <td class="lowercase">juan.perez@email.com</td>
```
