# ARIA: Accessible Rich Internet Applications

> *Lo mas importante de la accesibilidad es que les estamos dando una experiencia igual o más igual que podamos a personas que esten usando tecnologias asistivas.*

!!!!! idea para el canva Los roles le comunican al navegadores cuales son las interacciones que debería esperar y cómo se va a usar este objeto en nuestro proyecto. Se usan en situaciones muy especificas, es mejor depender del HTML semántico para comunicar los roles.

> *The most important thing about accessibility is that we are giving an equal or more equal experience as we can to people who are using assistive technologies.*


Accessible Rich Internet Applications (ARIA) is a set of attributes that define ways to make web content and web applications (especially those developed with JavaScript) more accessible to people with disabilities.

Fue creado por la WAI (Web Accessibility Initiative), ellos son los encargados de la especificacion de ARIA y la crearon para que podamos comunicar cambios especiales en nuestras aplicaciones.

It was created by the WAI (Web Accessibility Initiative), they are in charge of the ARIA specification and they created it so that we can communicate special changes in our applications.

---

## Atributos de ARIA
ARIA has **three special attributes** that we can add to HTML: **_roles, properties, and states_**. Next, we will describe each of the attributes.

- **Roles**
    - Define el tipo general del objeto (como un articulo, una alerta o un deslizador)
    - Le comunican al navegador cuales son las interacciones que deberian esperar y como se va usar ese objeto dentro de nuestra pagina o dentro de nuestra aplicacion.
    - **Los roles SOLO se usan en situaciones muy especificas**, es mejor que dependas del HTML semantico para comunicar los roles y no meterte a asignarle roles a cada uno de los elementos, ya que es una especificacion muy dificil de usar y hay que saber cuando son los momentos apropiados.
    ** Se usan en ocasiones especiales es mejor usar HTML semántico para no meterse en agregar roles a todos los elementos

    - Los roles comunican diferentes interacciones a navegadores y lectores de pantalla de como se navega en esa sección. 
        - Los navegadores y especialmente los lectores de pantalla, navegan diferentes roles en diferentes estilos.
    - Un articulo, un lector de pantalla no esperara mucha interaccion del usuario a comparacion de un formulario en el cual tiene diferentes metodos para esperar esa interaccion y para manejarla cuando pasa.


 > En tu portafolio no utilizaremos roles, sin embargo, si quieres saber mas sobre los tipos de roles que se pueden especificar en Aria, [haz click aquí](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles).

Resumen: the ARIA roles preparan al navegador o lectores de pantalla a indicar cuales son las interacciones que debería esperar, se usan en ocasiones especiales, en la mayoría de los casos se recomienda usar HTML semántico,

---

- **Propiedades**
    - Utilizamos con más frecuencia este atributo de ARIA.
    - Le comunican al navegador diferentes propiedades.
    - Comunican atributos que son escenciales para el comportamiento o significado de un elemento pero que se suelen comunicar visualmente.
        - Los iconos, formularios, slideshows, entre otros, necesitan las propiedades ARIA que describan dichos elementos y sus funcionamientos.    
        - Esto puede ser común (formularios) para una persona que cuenta con todas sus capacidades físicos, pero para una persona con discapacidades no es tan intuitivo, ya que ellos dependen de los lectores de lectura.

```HTML
    <!--Example -->
        <form class ="form-container">
            Name <input type="text" aria-label="Name"/><br/>
            E-mail <input type="text" aria-label="E-mail"/>
        </form>
```

- **Estados**
    - Comunican estados y cambios de estados en elementos que se suelen comunicar visualmente.
       - Si tenemos un checkbox
            - Sabemos que esta seleccionado por que está marcado
            - Alguien con discapacidad quizás no pueda ver eso

    - Los lectores de pantalla leen todos los elementos que tenemos en nuestro HTML incluyendo los que tenemos escondidos a simple vista.
        - Por lo cual hay que usar aria-hidden para que de esta manera el lector de pantalla tenga la misma experiencia que tiene las demas personas.
        - Therefore, aria-hidden should be used so that the screen reader has the same experience as other people have.

  ```HTML
            <li aria-hidden="true"> <!-- The use of aria-hidden will hide everything that is inside of this -->
                 <button>
                    <img src="images/project5.png" class="Project Project 5" alt="My fifth project"/>
                </button>
            </li>
    ```

## Summary 

We can provide a similar experience to users with disabilities as well as users who have all the physical benefits, using statuses which will communicate what things will be displayed on the screen.

Podemos brindar una experiencia similar a usuarios con discapacidades al igual que usuarios que tienen todos los beneficios físicos, usando estados los cuales comunicarán que cosas se estarán mostrando en pantalla

---
## ARIA attribute types

There are 4 categories of ARIA states and properties:

1 -  **Widget attributes**

    - aria-autocomplete
    - aria-checked
    - aria-disabled
    - aria-errormessage
    - aria-expanded
    - aria-haspopup
    - aria-hidden
    - aria-invalid
    - aria-label
    - aria-level
    - aria-modal
    - aria-multiline
    - aria-multiselectable
    - aria-orientation
    - aria-placeholder
    - aria-pressed
    - aria-readonly
    - aria-required
    - aria-selected 
    - aria-sort
    - aria-valuemax
    - aria-valuemin
    - aria-valuenow
    - aria-valuetext

2 - **Live region attributes**

    - aria-busy
    - aria-live
    - aria-relevant
    - aria-atomic

3 - **Drag-and-Drop attributes**

    - aria-dropeffect
    - aria-grabbed

4 - **Relationship attributes**

    - aria-activedescendant
    - aria-colcount
    - aria-colindex
    - aria-colspan
    - aria-controls
    - aria-describedby
    - aria-description
    - aria-details
    - aria-errormessage
    - aria-flowto
    - aria-labelledby
    - aria-owns
    - aria-posinset
    - aria-rowcount
    - aria-rowindex
    - aria-rowspan
    - aria-setsize

If you would like to learn more about each properties and states, [please click here](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Attributes#aria_attribute_types).

---

## Interesting resources
- [Videos of screen readers using ARIA](https://zomigi.com/blog/videos-of-screen-readers-using-aria-updated/)
- [Using ARIA - A practical guide for developers:  It suggests what ARIA attributes to use on HTML elements. Suggestions are based on implementation realities.](https://w3c.github.io/using-aria/)
- [Improving form accessibility](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/forms)
- [Etiquetas y relaciones de ARIA](https://developers.google.com/web/fundamentals/accessibility/semantics-aria/aria-labels-and-relationships)
- [HTML 'label' for Attribute](https://www.w3schools.com/tags/att_label_for.asp)
## Bibliographic references
- [MDN Web Docs - ARIA](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA)
- [MDN Web Docs - ARIA states and properties](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Attributes)
- [MDN Web Docs - WAI-ARIA Roles](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles)