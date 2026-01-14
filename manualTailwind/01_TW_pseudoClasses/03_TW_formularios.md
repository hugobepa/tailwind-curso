# FORMULARIOS

inputs type="text" text desabilitados: disabled disabled:cursor-not-allowed disabled:transparent disabled:text-gray-500 disabled:bg-gray-300/10
input type="email" invalid: text-pink-500 invalid:boder-pink-500 placeholder:text-sm placeholder:italic focus:border-sky-500 focus:invalid:border-pink-500 disabled:text-gray-500 disabled:bg-gray-300/10 disabled

afecta a todos los elementos donde se pongan "/src/styless.css":

```
@layer components {
  .form-control {
    @apply rounded-md border border-gray-600 bg-transparent px-4 py-3 text-white transition-colors outline-none placeholder:text-sm placeholder:italic invalid:border-pink-500 invalid:text-pink-500 focus:border-sky-500 focus:invalid:border-pink-500 disabled:bg-gray-300/10 disabled:text-gray-500;
  }}
```

  <input type="text" id="username" value="JuanCarlos" disabled class="form-control" />

## etiquetas errores de los campos

- "peer" en el campo de refencia del texto de aviso:

  <input type="password" id="password" minlength="8" maxlength="16" placeholder="Mínimo 8 caracteres"class="form-control peer" />
  - "peer-invalid:visible" gestionar el aviso del campo de refencia:
  - "invisible/visible2 para que se vea o no sea vea
  - "hidden/block" pero modificar el tamño dem campo NO RECOMENDABLE
    <span class="invisible text-sm text-pink-500 peer-invalid:visible">Ingresa una contraseña válida de entre 8 y 16 caracteres</span>

## botton

- mejorar botton cuando estemos (en el (chrome)): "focus:ring-sky-500 focus:ring-offset-2 focus:ring-offset-slate-900 "
- rectificar error safari: focus:outline-none

class="rounded-md bg-sky-500 px-6 py-3 font-semibold text-white transition-colors hover:bg-sky-600 focus:ring-2 focus:ring-sky-500 focus:ring-offset-2 focus:ring-offset-slate-900 focus:outline-none"

afectacion global "src/styles.css":

```
@layer base {

  button {
    @apply cursor-pointer;
  }
}
```
