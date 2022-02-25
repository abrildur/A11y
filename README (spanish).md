# Accessibility Allies: ¡Crea tu portafolio + subelo a la nube!
> Haz el mundo más accesible al crear contenido para todos y todas.

¡Hola, viajero galactico! 🌍 Te damos la bienvenida a esta nueva aventura que estas a punto de comenzar, el objetivo de este taller es que crees tu portafolio y lo subas a la nube de Azure, teniendo en cuenta principios de accesibilidad.

> Tiempo estimado total de lectura: 30 minutos. 
> Tiempo estimado para realizar las actividades: 1 hora.

Asi que, te estaras preguntando:  

¿Qué es lo que voy a necesitar para continuar mi viaje? Muy simple mi estimadx Padawan, necesitaras lo siguiente:
- Conocimientos básicos de programación (HTML, CSS)
- Visual Studio Code.
- Una cuenta de Azure.
    - Si aun no tienes tu cuenta de Azure y eres estudiante, ve a la siguiente [liga](https://azure.microsoft.com/es-mx/free/students/) para que obtengas tus creditos y cuenta gratuita como estudiante en Azure. 
- Una cuenta en GitHub

¿Estas listo para nuestro viaje a un mundo mas accesible? ¡Comenzemos!

!["Bug's Bunny listo para iniciar - Gif"](https://media.giphy.com/media/QJvwBSGaoc4eI/giphy.gif)

---
## Antes de empezar
**¿Qué es la Accesibilidad Web?** Es la práctica continua de asegurarnos que todo lo que creamos para la web se puede usar, interpretar y operar por una variedad de personas en una variedad de situaciones.

**¿Por que es importante la accesibilidad?**


**¿Cuales son los beneficios de tomar en cuenta la accesibilidad en mi pagina web o en mi portafolio?**
- Al utilizar HTML Semantico, esto mejora el SEO de dicha pagina web: lo cual significa, que apareceras en mayores resultados.
-	Para incluir a personas en situaciones de discapacidad.
-	Para mejorar la usabilidad de nuestros proyectos.
-	Porque en algunos lugares es la ley.
    - En Estados Unidos hay una ley que se llama: _“American’s with Disabilities Act (ADA)”_ en la cual, no importa si tu creaste el producto fuera de Estados Unidos, pero si los consumidores de tu producto están en EE.UU, ELLOS TIENEN el derecho a que todos los productos, servicios que utilicen sean accesibles.  
        -	Caso de Domino's Pizza que fue multado por su sitio web inaccesible [Lee un poco más sobre el caso aquí (INGLES)](https://www.cnbc.com/2019/10/07/dominos-supreme-court.html) 
    - En LATAM el 55% de países tiene una ley, norma una guía que es específicamente para la accesibilidad web.
    - El resto de leyes no tienen normas especificas para la web, pero si tienen normas y leyes para personas en situaciones de discapacidad. 
- Es importante que sepas cuales leyes son las que te aplican a ti, a tus productos para protegerte y para proteger tus empresas. 

**¿Por que es importante la accesibilidad?**


---
## The more you know... 
Ahora que sabes los beneficios que hay por tener accesibilidad web. Es momento que conozcas algunas organizaciones e instituciones que velan por el cumplimiento de leyes y normas de accesibilidad para crear un mundo más seguro.

¿Qué es WCAG?
En ingles son las Web  Content Accesibility Guidelines o en español las pautas de accesibilidad para el contenido web. 
-	Un rango de recomendaciones para crear contenido web mas accesible.
Historia de WCAG
Son creados por la W3C (World Wide Web Consortium), ellos son los creadores de los estándares que usamos para construir la web (HTML, CSS) y dentro de esta organización hay diferentes iniciativas para enfocarse en temas específicos como el WAI – Web Accessibility Initiative. Iniciativa dentro W3C cuya meta es asegurar la accesibilidad web. Es la guía que nos ayuda a implementar la accesibilidad web.
WCAG 2.0 lo cual nos asegura que a medida nuestras tecnologías van creciendo, el estándar con la especificación tambien va creciendo con ellos. Dentro de WCAG hay 12 criterios de conformidad que debemos respetar y cada criterio se divide en tres niveles. Los tres niveles nos ayudan a escoger que tanta inversión le queremos poner a la accesibilidad web.
El nivel A. es el nivel mas bajo. Nos garantiza una accesibilidad básica para nuestros productos.
Nivel AA intermedio y Nivel AAA mas alto, este lo usa comúnmente empresas que trabajan con gobiernos o universidades para asegurarse que su contenido que es fundamental para el publico, pueda ser accedido por cualquier persona.

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
Las tecnologías asistivas, ayudan a las personas que no tienen sus capacidades visuales o motoras perfectamente bien, como las tienen muchas personas. Las tecnologías asistivas nos dan alternativas a las existentes para mejorar nuestras habilidades de consumir el mundo alrededor de nosotros.
Las tecnologías asistidas para la web se pueden dividir en dos campos: las que son para las habilidades visuales y las que son para las habilidades motoras. 
- visuales: No todo el mundo puede usar una pantalla como lo utilizan las personas usualmente.
-	lectores de pantalla: son software que instalas, que nos ayudan a interpretar los sitios y leerlo a voz alta para personas que no pueden leer ese sitio. 
-	extensiones que manipulan el CSS. Estas extensiones pueden manipular el CSS de sitios para ser que el foco sea mas grande, un color especifico, que el texto del sitio web sea mas grande, cambia los estilos del sitio para ayudar a una persona decidir que les ayuda mejor a interpretar ese sitio.

### Motoras:
-	varilla bucal. Una persona que no tiene puede usar sus manos, puede usar esto al introducirlo en su boca y manejar ya sea un teclado u otra tecnología asistida que ellos hayan configurado para señalar con esa varilla bucal.
-	switch. Se vuelve todo un mundo de tecnologías asistidas porque simplemente darle una persona la opción de manejar un interruptor que prenda o apague, puede ser un botón, dos botones, botones grandes o chiquitos. Puede ser un sensor que detecte que si la cara se mueve y que la misma persona configura. ¿Cómo funcionan las tecnologías asistivas cuando son para habilidades motoras? Escuchan el teclado y esto es muy importante: El teclado es el puente que va a conectar nuestro sitio web con un mundo de tecnologías asistidas, entonces, tenemos que tener en cuenta que no estemos usando de la mejor manera.


---

Con amor desde México  ♥️

![Gato con sombrero mexicano - gif](https://media.giphy.com/media/TN0kjxBsz3iXm/giphy.gif)

---
## Referencias Bibliograficas y articulos de interes
- [Microsoft Learn - Accessibility fundamentals (INGLES)](https://docs.microsoft.com/en-us/learn/paths/accessibility-fundamentals/)
- [Microsoft Learn - Introduction to disability and accessibility (INGLES)](https://docs.microsoft.com/en-us/learn/modules/intro-accessibility-disability/00-what-is-accessibility)
- [Microsoft - AI for Accessibility Projects (INGLES)](https://www.microsoft.com/en-us/ai/ai-for-accessibility-projects)
- [Microsoft - Text to Speech](https://azure.microsoft.com/es-mx/services/cognitive-services/text-to-speech/#overview)
- [Microsoft - Funciones de accesibilidad de Microsoft](https://www.microsoft.com/es-mx/accessibility/features?rtc=1&activetab=pivot_1:primaryr2)
- [Microsoft - Accessibility (INGLES)](https://www.microsoft.com/en-us/accessibility)