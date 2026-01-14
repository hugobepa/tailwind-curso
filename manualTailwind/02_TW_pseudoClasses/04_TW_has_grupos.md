# HAS

afectacion cambio a elemento de dentro:

- ponemos el color en el campo principal: `<label class="bg-indigo-500/50"> `
- campo afectado tambien: `<svg fill="currentColor" ...></svg>`

afetar si esta chequeado, input dentro del label:

- etiqueta padre: `has-checked`
- campo chequeado: ` <input checked type="radio"`

```
<label
        class="has-checked:bg-indigo-500/30 has-checked:text-indigo-400"
      >
       ....
        <input checked type="radio" name="payment" value="google-pay" />
      </label>
```

si dentro de un elemento con `flex` ponemos a otro de detro de este `flex-1 ` se estira

# GRUPOS

## afectacion padres (div) e hijos (elementos internos)

### group-has-

Afectar un cambio a avarios elementos a la vez:
ejemplo aparecer span si hay un ancortar en el grupo "a":

- poner "group" dentro de la div: `class="group ..."`

- span: `<span class="hidden group-has-[a]:block">Ir al enlace</span>`

- afectacion al mismo elemento: <a href="#"class="group-has-[a]:text-sky-400">Visita este enlace</a>

### group-hover

Si el padre tiene un hover: `<div class="group ... hover:bg-sky-400">`

campo afectado: `<a href="#" class="group-hover:text-sky-800"> `

ejemplo de ambos svg: `<svg class="group-hover:text-violet-700 group-has-[a]:text-sky-400">`

## ejemplo hermonos (peer) check

checkList selecionar texto. Entonces que se tache y aparezca texto :

- elemento check que aparece o desaparece : `  <svg ... class="hidden h-5 w-5 text-gray-500 peer-has-checked:block">  ` `
  (peer-has-[checked])
- para activar el "peer-has-checked": ` <label for="task-1" class="peer " >`

tallar texto:

campo de referencia: ` <input type="checkbox" checked class="peer"/>` y ` <label class="peer ">`
campo afectado: ` <span class=" peer-checked:line-through" >`

# CHECKED

marcar un chekced:

```

<input
              type="checkbox"
              id="task-1"
              checked
              class="checked:after:absolute checked:after:top-1/2 checked:after:left-1/2 checked:after:-translate-x-1/2 checked:after:-translate-y-1/2 checked:after:text-sm checked:after:text-white checked:after:content-['✓']"
 />

```

```

```
