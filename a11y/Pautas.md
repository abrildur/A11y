# The more you know... 

Ahora que sabes los beneficios que hay por tener accesibilidad web. Es momento que conozcas algunas organizaciones e instituciones que velan por el cumplimiento de leyes y normas de accesibilidad para crear un mundo más seguro.

## ¿Qué es WCAG?

En inglés son las _Web  Content Accesibility Guidelines_ o en español, las "Pautas de Accesibilidad para el contenido Web". 
-	Un rango de recomendaciones para crear contenido web mas accesible.

## Historia de WCAG
Son creados por la W3C (_World Wide Web Consortium)_, ellos son los creadores de los estándares que usamos para construir la web (HTML, CSS) y dentro de esta organización hay diferentes iniciativas para enfocarse en temas específicos como el _WAI – Web Accessibility Initiative_. Iniciativa dentro W3C cuya meta es asegurar la accesibilidad web. Es la guía que nos ayuda a implementar la accesibilidad web.

**WCAG 2.0** lo cual nos asegura que a medida nuestras tecnologías van creciendo, el estándar con la especificación tambien va creciendo con ellos. Dentro de WCAG hay 12 criterios de conformidad que debemos respetar y cada criterio se divide en tres niveles. Los tres niveles nos ayudan a escoger que tanta inversión le queremos poner a la accesibilidad web.

	- El nivel A. es el nivel mas bajo. Nos garantiza una accesibilidad básica para nuestros productos.
	- Nivel AA es el nivel intermedio
	- Nivel AAA es el nivel más alto. Este nivel lo utilizan comúnmente empresas que trabajan con gobiernos o universidades para asegurarse que su contenido que es fundamental para el publico, pueda ser accedido por cualquier persona.

Las pautas de accesibilidad de contenido web nos guían al momento de implementar la accesibilidad web. Las podemos usar durante todo el proceso de desarrollo de producto, desde que nace la idea para lo que queremos construir, durante el diseño de los estilos y las interfaces, hasta cuando escribimos código y hacemos pruebas de calidad. Nos señalan los puntos importantes para tener en cuenta con eso podemos construir páginas, productos y aplicaciones que le funcionan a todos nuestros usuarios sin importar su capacidades, dispositivos o preferencias.

Aunque las pautas (referidas también por su nombre en inglés WCAG) son muy completas y siguen creciendo a medida que nuestras tecnologías crecen, es importante conocer los 4 principios que nos guían para poder tomar decisiones puntuales a nivel de nuestros productos. Dentro de cada principio encontramos los criterios de conformidad que se pueden interpretar acorde al nivel de WCAG que le quieres o debes aplicar a tu sitio web. 

En esta lectura vamos a profundizar sobre los criterios de conformidad para tener una idea más clara de que podemos encontrar dentro de WCAG. Podemos empezar por el primer principio:

	perceptible
	operable
	comprensible
	robusto

El perceptible es que la información y los componentes de la interfaz de usuario deben ser presentados a los usuarios de modo que ellos puedan percibirlos.
Operable es que los componentes de la interfaz de usuario y la navegación deben ser operables.
Comprensible es que la información y el manejo de la interfaz de usuario deben ser comprensibles.
-	Como operar tu sitio, que es lo que hace tu sitio y que entiendan que es lo que el sitio requiere de ellos así como pueden ellos corregir algún error.
Robusto es que el contenido debe ser suficientemente robusto como para ser interpretado de forma fiable por una amplia variedad de aplicaciones de usuario, incluyendo las ayudas técnicas.

---

# Diseñando para todos
te compartiremos algunos consejos sobre como podras diseñar para todos.


"El poder de la Web està en su universalidad. El acceso detodaslaspersonas independientemente dela discapacidad es un aspecto esencial." Tim Berners-Lee, W3C Director.

Hoy en dia es obligatorio que nuestras paginas web y aplicaciones sean accesibles, la web es un deerecho para todas las personas incluidas a las personas que tienen cualquier tipo de discapacidad.

Tips básicos de accesibilidad.
- Utiliza los encabezados de manera ordenada para organizar la estructura delcontenido (HTML5 Semantico). El uso de diferentes tipos de titulos (H1, H2, H3...) nos permite generar jerarquia y esto es muy importante para la accesibilidad, ya que esto le garantiza a una persona que este navegando por el teclado que identifique que tan importante es un titulo en relacion a otro, permite agrupar por diferentes categorias, grupos de informacion, etc.
- Utiliza tamaños de fuente accesibles.
	Usar un tamaños de fuente de 10px, asi sea en un movil, no es algo practico. Tenemos que garantizar que los tamaños de fuente sean accesibles para todas las personas.
- Utiliza colores que tengan un contraste adecuado.
	hay personas que tienen diferentes formas de percibir el color. Entonces, tenemos que asegurarnos que el contraste sea lo suficientemente alto para poder diferenciar un fondo de un contenido. Muchas veces vemos como se usan fondos amarillos con textos blancos y solo pensamos en la estetica, cuando en realidad mas alla de la estetica tenemos que intentar crear productos que sean llamativos/atractivos pero que tambien le funcionen a cualquier tipo de publico.

https://platzi.com/clases/1906-diseno-programadores/28553-accesibilidad-y-diseno/

- Garantiza que el codigo de color no sea la unica forma de relacionar el contenido.
	Al implementar las agrupaciones de contenido por colores es necesario ofrecer una alternativa ya sea con un borde, icono o un titulo de categoria para que de esta manera se pueda garantizar que cualquier persona pueda acceder a dicho contenido.

- Diseña teniendo en cuenta los estados "focus" y "active" de los componentes.
	 cuando programamos vemos por defecto los formularios, los botones, u otros elementos de HTML quedan con un borde despues de hacerle click o con un subrayado, esto es importante no quitarlo porque esta es una guia visual para muchas personas o para personas que estan navegando por el teclado.

- Añade etiquetas y textos descriptivos a los campos de formulario.
	Esto es muy importante para las personas que navegan con el __tab_ no van a tener acceso a todos los titulos, entonces es importante añadirle una etiqueta descriptiva como son las Aria-Labels. 
	Es importante tambien garantizar a los usuarios que cuando aparezca algun error en el formulario ademas de que cambie de color el boton/borde a rojo o a verde tambien aparezca un mensaje que pueda ser escuchado por un lector de pantalla.
	
- Escribe contenido descriptivo que pueda reemplazar videos e imágenes.
	A veces subimos informacion muy importante en imagenes o videos lo cual no permitiria a una persona que utiliza lectores de pantalla obtener dicha informacion, asi que es mejor manera.
	Es mejor mantener el texto fuera de los videos e imagenes y de esta manera los usuarios que estan navegando por medio de un lector de pantalla van a poder escuchar la interpretacion de estos elementos.
	Ahora quieres incluir una imagen de por ejemplo un perrito que es importante para tu sitio web, añade una etiqueta alt para que las personas que estan utilizando lectores de pantalla puedan saber que hay en dicha seccion. 


- Garantiza que las animaciones no bloqueen el acceso al contenido.
	Esto va de la mano con el diseño responsivo. Cuando tenemos una pagina, en donde tenemos que haccer click para ejecutar una animacion y esto nos va a mostrar el texto, esto quiere decir queeste teexto basico esta bloqueado por una animacion. Esto tampoco es una buena practica y tampoco es buena practica que los usuarios vean muchos flashes cuando van a acceder a una pagina. 

