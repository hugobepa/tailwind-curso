# GRUPOS ANIDADOS

## grupo anomino

0. declarar grupo en padre: `<li class="group hover:bg-slate-500/30"`
1. anchora aparezca: `<a class="invisible  group-hover:visible"`
2. flechita se mueve a la derecha: `<svg  class="transition-transform group-hover:translate-x-0.5" ` y
   ` <span class="transition-colors group-hover:text-gray-200"`

## grupo declarado

0. declarar grupo en padre: `<li class="group/item hover:bg-slate-500/30"`
1. anchora aparezca: `<a class="invisible  group-hover/item:visible"`

2. declarar grupo: `<a class="group/edit invisible  group-hover/item:visible"`
3. flechita se mueve a la derecha: `<svg  class="transition-transform group-hover/edit:translate-x-0.5" ` y
   ` <span class="transition-colors group-hover/edit:text-gray-200"`

# GRUPO IMPLICITOS

## group-focus-within

0. declarar el group: `<div class="group ring-pink-500 focus:ring-2"`
1. llammar al grupo:` <div class="group-focus:opacity-100 group-hover:bg-sky-500"`

## in-focus

0. declarar grupo: `<div tabindex="0" class="focus:ring-2"`
1. hacer la llamada sin declarar group previa.: `<div class="in-focus:opacity-100 in-hover:bg-sky-500" `

(difeerenciadoPeers)[https://tailwindcss.com/docs/hover-focus-and-other-states#styling-based-on-sibling-state]

# DIFERENCIADO PEERS

## declarion anonima

0. declarar class en el hermano : `<input class="peer" `
1. afectar la visilidad del div: `<div class="hidden peer-checked:block"  `

## declaracion propia

0. declarar class en el hermano con nombre: `<input class="peer/draf" `
1. afectar la visilidad del div especifico: `<div class="hidden peer-checked/draft:block"  `
