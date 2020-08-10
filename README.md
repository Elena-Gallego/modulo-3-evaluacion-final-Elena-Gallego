## Buscador de personajes de la serie Rick & Morty

El ejercicio consiste en desarrollar una página web con un listado de personajes de Rick and Morty, que podemos filtrar por el nombre del personaje. Vamos a usar React para realizarlo.
Definimos las siguientes partes del ejercicio:

1. Listado de personajes

Vamos a realizar una web con el listado de personajes de Rick and Morty. Para eso, vamos a utilizar el servicio de https://raw.githubusercontent.com/Adalab/rick-y-morty/master/data/rick-y-morty.json. que nos devuelve información sobre los primeros 20 personajes de la serie. De cada uno pintaremos al menos las siguientes propiedades:

- Foto.
- Nombre.
- Especie.

Para esta primera parte del ejercicio no es necesario maquetar el resultado pintado.

2. Filtrado de personajes

Ahora que ya tenemos el listado de personajes en pantalla, la segunda parte consiste en realiar búsquedas por nombre. Para ello añadiremos un input a la interfaz de forma que al ir escribiendo un nombre queden en la interfaz solo los personajes cuyo nombre contiene las letras escritas en el input.

- NOTA: en principio no es necesario tener en cuenta si las letras están en mayúscula / minúscula para la búsqueda, pero si queréis añadir esta mejora podéis hacerlo.

3. Componentes del listado de personajes

El listado debe tener los siguientes componentes como mínimo:

    - Componente para los filtros.
    - Componente para el listado.
    - Componente para la tarjeta de cada personaje del listado.
    - Componente para el detalle de cada personaje.

4. Detalle de personajes

   - Vamos a implementar una nueva funcionalidad: al hacer clic sobre la tarjeta de un personaje, su información aparecerá a pantalla completa. Para hacer esto usaremos rutas y React Router. En la pantalla de detalle aparecerá además de la foto, nombre y la especie, el planeta de origen, el número de episodios en los que aparece y si el personaje está vivo o muerto.

5. Detallitos de calidad

   - Como nos gusta cuidar la semántica, el campo de texto debe estar recubierto por una etiqueta <form>.
   - Si estando en el campo de filtrado pulsamos intro debéis impedir que el navegador cambie la ruta sin querer.
   - Si se busca por un texto por ejemplo "XXX" y no hay ningún personaje que coincida con dicho texto se mostrará un mensaje del tipo "No hay ningún personaje que coincida con la palabra XXX".
   - El filtro debe filtrar independientemente de que la usuaria introduzca el texto en mayúsuclas o minúsculas.
   - Al entrar en el detalle de un personaje y a continuación pulsar atrás, el campo de texto debe mostrar el texto que tenía anteriormente.

6. BONUS: Mejoras visuales

Para terminar, podéis realizar algunas mejoras visuales del ejercicio. Por ejemplo:

    - Mostrar la especie y si un personajes está muerto con un icono.
    - Usar un sistema de grid para pintar el listado de personajes.
    - Que funcione bien el responsive para dispositivos pequeños.

7. BONUS: URL compartible

   - Como ejercicio extra os proponemos que la URL del detalle de personaje sea compartible, es decir, que si visitamos esa URL directamente en el navegador se vea el detalle del personaje.
   - En el caso de que el usuario navegue a una URL inexistente como por ejemplo
     http://localhost:3000/#/detail/12345 (el id 12345 no existe) debemos mostrar un mensaje del tipo "El personaje que buscas no existe".

8. BONUS: Ordenación

   Un extra interesante sería que ordenáseis el listado de personajes alfabéticamente por nombre.
