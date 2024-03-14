# Calculadora
Calculadora basica con HTML CSS y JAVASCRIPT
# Lora Jalomo Daniel Alejo Marzo 2024

Introducción

En este proyecto creamos una calculadora mediante las tecnologías HTML, CSS y JavaScript, nosotros por si solos hubiésemos podido crear la calculadora simplemente con el diseño, con HTML y CSS pero el código que nos proporciono fue el de JavaScript que básicamente realiza mediante funciones todas las operaciones de la calculadora, esto nos sirve de aprendizaje para ver en retrospectiva la correcta utilización de JavaScript, como lo podemos aplicar a nuestros programas y su importancia dentro del desarrollo Web, puesto que va de la mano con HTML y CSS. Para lograr esta calculadora requerimos de varias propiedades básicas tal como lo es el DOM.

El modelo de objeto de documento (DOM) es una interfaz de programación para los documentos HTML y XML. Facilita una representación estructurada del documento y define de qué manera los programas pueden acceder, al fin de modificar, tanto su estructura, estilo y contenido. El DOM da una representación del documento como un grupo de nodos y objetos estructurados que tienen propiedades y métodos. Esencialmente, conecta las páginas web a scripts o lenguajes de programación.


Desarrollo
Por supuesto, profundizaré en cada una de estas líneas para ofrecerte una comprensión más detallada sobre cómo trabajan estas instrucciones de JavaScript para interactuar con el Document Object Model (DOM) de una página web, que es esencialmente la estructura de objetos que el navegador utiliza para representar el documento HTML.

1. document.querySelector(".display");

Esta instrucción es una llamada al método `querySelector` del objeto `document`. Lo que hace es buscar en todo el documento HTML el primer elemento que coincida con el criterio de búsqueda especificado, en este caso, cualquier elemento que tenga asignada la clase CSS `display`. Es una herramienta poderosa para seleccionar elementos de forma precisa utilizando selectores CSS. Si el documento contiene múltiples elementos con la clase `.display`, solo se devolverá el primero de ellos. Si no se encuentra ningún elemento que coincida, el método retorna `null`. Esta funcionalidad es particularmente útil para manipular o extraer información de un elemento específico dentro de la estructura HTML de una página.

2. const buttons = document.querySelectorAll("button");

  Aquí se utiliza el método `querySelectorAll` para seleccionar todos los elementos en el documento que se ajusten al selector proporcionado, que en este caso es `"button"`. A diferencia de `querySelector`, que solo devuelve el primer elemento coincidente, `querySelectorAll` devuelve todos los elementos que coinciden con el selector como una NodeList. Aunque similar a un array en que puedes acceder a elementos por su índice y recorrerlo con métodos como `forEach`, una NodeList tiene algunas diferencias en cuanto a los métodos que soporta directamente. Esta operación es crucial cuando necesitas trabajar con múltiples elementos del mismo tipo, como botones en una interfaz de usuario, permitiendo aplicar operaciones o eventos a cada uno de ellos de manera eficiente.

3. buttonText = button.textContent;

   En este fragmento, se accede a la propiedad `textContent` de un objeto `button`. Esta propiedad obtiene o establece el contenido de texto de un nodo y sus descendientes. Aquí, `textContent` se usa para extraer el texto contenido dentro de un elemento de botón específico, asignando este valor a la variable `buttonText`. Esta operación es comúnmente utilizada para leer o modificar el texto de elementos en la página, lo cual es útil en diversas situaciones, como actualizar dinámicamente el texto mostrado en la página o realizar acciones basadas en el contenido de texto de elementos específicos.






4. buttons.forEach((button) => { ... }

   Este código demuestra el uso del método `forEach` para iterar sobre cada elemento de la NodeList `buttons` obtenida con `querySelectorAll`. `forEach` es un método que permite ejecutar una función sobre cada elemento de una lista. La sintaxis `(button) => { ... }` define una función flecha que se ejecuta para cada elemento `button` en la lista. Dentro de las llaves `{ ... }`, puedes incluir cualquier lógica o operaciones que desees realizar con cada botón individualmente. Esto es especialmente útil para asignar manejadores de eventos a múltiples elementos o aplicar cambios de estilo o contenido de manera masiva.

5. button.addEventListener("click", () => { } )

  Finalmente, esta línea ilustra cómo agregar un escuchador de eventos a un elemento `button` usando el método `addEventListener`. El primer parámetro especifica el tipo de evento a escuchar, en este caso, un evento de `"click"`. El segundo parámetro es una función que se ejecutará cada vez que el evento ocurra, aquí representado por una función flecha vacía `() => { }`, dentro de la cual puedes colocar el código que desees ejecutar cuando el usuario haga clic en el botón. Este patrón es fundamental para la interactividad en aplicaciones web, permitiendo a los desarrolladores vincular comportamientos específicos a acciones del usuario, como clics, entradas de teclado, movimientos del mouse, entre otros.



Conclusión
Los aprendizajes obtenidos en esta practica fueron bastantes, pudimos controlar y entender el DOM, que básicamente podemos acceder a los atributos y etiquetas de HTML y modificarlos, así como crear las funciones requeridas para llevar a cabo la funcionalidad de una calculadora, sabemos que JavaScript es un lenguaje de programación en donde tenemos lo mismo, que son estructuras de control, variables, sentencias, etc. Entonces aquí hacemos uso de los conocimientos adquiridos en los primeros semestres en programación, simplemente utilizando la misma lógica pero con distinta sintaxis.
