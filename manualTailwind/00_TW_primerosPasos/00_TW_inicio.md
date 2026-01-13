https://tailwindcss.com/
https://tailwindcss.com/docs/installation/using-vite
https://tailwindcss.com/docs/responsive-design
https://play.tailwindcss.com/ (generated css -all/utilities-)

w/h- full :es el campo no mas
w/h -screen :es toda la pagina

archivo.css:
-afecta a todo la pagina y a los elementos nombrados
- generatedCSS - base
````
@layer base{

	h1{@apply text-5xl text-blue-500}
}
````

button : px-2 py-2 rounded rounded-4xl(padding horinzontal, vertical y borde redondeado)
div: flex justify-center items-center (elementos centro)
button: hover:bg-violet-700 (cuando estamos encima del botton)


#agrupar css

css:
para afectar a componente
````
@layer components{

     .btn-primary{
		@apply rounded bg-violet-500 px-4 py-2 text-white hover:bg-red-700
	 }
	
}

````

html: button -- btn-primary

# FLEXBOX ROW(flex === flex-row)

div: flex h-screen  w-screen justify-envently items-center 
flex: aliniacion horizontal

## aliniacion en FLEX respecto al padre a nivel global

justify-xxx: disposicion/espacio entre los elementos horizontalmente
items-xxx: aliniacion vertical de los elementos

## aliniacion individual elemento verticalmente dentro del FLEX

elemento: self-xxxx


# FLEXBOX COLUMN

div: flex flex-col (flex-col-reverse : aliniacion al reves)


## aliniacion individual elemento horizontal dentro del FLEX

elemento: self-xxxx

-pasar la pantalla de vertical a horinzonal cuando no sea movil:
 flex flex-col md:flex-row
 ( tamaño pantalla: sm,md,lg,xl,2xl)(md:hover:...)
 
 #GRID
 
div: grid grid-cols-2 gap-4 px-2
div: grid sm:grid-cols-3 (pant. pequeña 1 col, pant med. 2 col)
- grid: ponerlas en tabla
- grid-cols-n : numero celdas horizontal
- gap-n: separacion entre celdas
- px-n: padding horitonal entre elementos



