# ARIA: Accessible Rich Internet Applications

> Lo mas importante de la accesibilidad es que les estamos dando una experiencia igual o más igual que podamos a personas que esten usando tecnologias asistivas. No es justo ofrecerles otra experiencia completa simplemente porque no tienen la necesidad de usar las maquinas como nosotros lo usamos.

Accessible Rich Internet Applications (ARIA) is a set of attributes that define ways to make web content and web applications (especially those developed with JavaScript) more accessible to people with disabilities.

Fue creado por la WAI (Web Accessibility Initiative), ellos son los encargados de la especificacion de ARIA y la crearon para que podamos comunicar cambios especiales en nuestras aplicaciones.

---

## Atributos de ARIA
ARIA tiene tres atributos especiales que a podemos agregar a HTML.

- Roles
    - Define el tipo general del objeto (como un articulo, una alerta o un deslizador)
    - Le comunican al navegador cuales son las interacciones que deberian esperar y como se va usar ese objeto dentro de nuestra pagina o dentro de nuestra aplicacion.
    - **Los roles SOLO se usan en situaciones muy especificas**, es mejor que dependas del HTML semantico para comunicar los roles y no meterte a asignarle roles a cada uno de los elementos, ya que es una especificacion muy dificil de usar y hay que saber cuando son los momentos apropiados.
    - Los roles comunican diferentes interacciones a navegadores y lectores de pantalla de como se navega en esa sección. Los navegadores y especialmente los lectores de pantalla, navegan diferentes roles en diferentes estilos.
    - Un articulo, un lector de pantalla no esperara mucha interaccion del usuario a comparacion de un formulario en el cual tiene diferentes metodos para esperar esa interaccion y para manejarla cuando pasa.

- Propiedades
    - **Estos atributos de ARIA, sí los vamos a usar mas seguido**
    - Estas le comunican al navegador diferentes propiedades.
    - Comunican atributos que son escenciales para el comportamiento o significado de un elemento pero que se suelen comunicar visualmente.
        - Los iconos, formularios, slideshows, entre otros, necesitan las propiedades ARIA que describan dichos elementos y sus funcionamientos.
    
    ```HTML
        <form class ="form-container">
            Name <input type="text" aria-label="Name"/><br />
            E-mail <input type="text" aria-label="E-mail"/>
        </form>
    ```
- **Estados**
    - Comunican estados y cambios de estados en elementos que se suelen comunicar visualmente.
        - Digamos que tenemos un checkbox, si el checkbox esta tick esa opcion esta seleccionada pero una persona que utiliza el lector de pantalla no podra ver esa opcion de checkbox. Por eso, tenemos que comunicar los diferentes estados que tengamos en nuestras aplicaciones para poder ofrecer una experiencia igual o parecida a una persona usando el lector de pantalla.
    - Los lectores de pantalla leen todos los elementos que tenemos en nuestro HTML incluyendo los que tenemos escondidos, por lo cual hay que usar aria-hidden para que de esta manera el lector de pantalla tenga la misma experiencia que tiene las demas personas.

  ```HTML
        <ul class ="project-container">
            <li>
                <button>
                    <img src="images/project1.png" class="Project Project 1" alt="My first project"/>
                </button>
            </li>
            <li>
                 <button>
                    <img src="images/project2.png" class="Project Project 1" alt="My second project"/>
                </button>
            </li>
            <li>
                 <button>
                    <img src="images/project3.png" class="Project Project 3" alt="My third project">
                </button>
            </li>
            <li  aria-hidden="true">
                 <button>
                    <img src="images/project4.png" class="Project Project 4" alt="My fourth project"/>
                </button>
            </li>
            <li aria-hidden="true">
                 <button>
                    <img src="images/project5.png" class="Project Project 5" alt="My fifth project"/>
                </button>
            </li>
        </ul>
    ```
---

## Bibliographic references
- [Microsoft](www.microsoft.com)
- [MDN Web Docs - ARIA](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA)
- [ARIA states and properties](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Attributes)
- [Videos of screen readers using ARIA](https://zomigi.com/blog/videos-of-screen-readers-using-aria-updated/)
- [Using ARIA - A practical guide for developers:  It suggests what ARIA attributes to use on HTML elements. Suggestions are based on implementation realities.](https://w3c.github.io/using-aria/)
- [Improving form accessibility](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/forms)
- [WAI-ARIA Roles](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles)
