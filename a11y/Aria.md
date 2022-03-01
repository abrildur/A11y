# ARIA: Accessible Rich Internet Applications
> *The most important thing about accessibility is that we are giving an equal or more equal experience as we can to people who are using assistive technologies.*

Accessible Rich Internet Applications (ARIA) is a set of attributes that define ways to make web content and web applications (especially those developed with JavaScript) more accessible to people with disabilities.

It was created by the WAI (Web Accessibility Initiative), they are in charge of the ARIA specification and they created it so that we can communicate special changes in our applications.

---

## ARIA Attributes
ARIA has **three special attributes** that we can add to HTML: **_roles, properties, and states_**. Next, we will describe each of the attributes.

**Roles**
- These attributes tell the browser what interaction is expected and how the object will be used on our page or in our application.
        - Defines the general type of the object (such as an article, an alert or a slider).
    - **It is better to rely on semantic HTML** to communicate the roles rather than assigning roles to each of the elements, since **it is a difficult specification to use and you need to know when is appropriate**.
    - In general, **they should be used only on special occasions**, and semantic HTML should be used instead of adding roles to each element.
    - Browsers and screen readers are given different interactions based on the role they play in that section. 
    - The screen reader will not expect much interaction from the user when reading an article as opposed to a form which has different methods to deal with interaction when it occurs.


 > We will not use roles in your portfolio; however, if you're interested in knowing more about the types of roles that can be specified in Aria, [click here](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles).

**Properties**
- We use this ARIA attribute more frequently.
    - They communicate different properties to the browser.
    - In general, they communicate attributes that are essential to the behavior or meaning of an element, but are typically communicated visually.
        - ARIA properties describe various elements and their functions, such as icons, forms, and slideshows.    
        - The forms may be common to someone who has full physical capabilities, but for someone with disabilities, they are not so intuitive, since they rely on reading readers.

```HTML
    <!--Example -->
        <form class ="form-container">
            Name <input type="text" aria-label="Name"/><br/>
            E-mail <input type="text" aria-label="E-mail"/>
        </form>
```


- **States**
    - The elements they communicate provide information about states and state changes that are usually communicated visually.
       - Suppose we have a checkbox:
            - It has a visual indication that it has been selected
            - People with vision disabilities may not be able to see those visual marks

    - Screen readers are able to read every element in our HTML, even those that are hidden.
        - Therefore, aria-hidden should be used so that the screen reader has the same experience as other people have.

  ```HTML
            <li aria-hidden="true"> <!-- The use of aria-hidden will hide everything that is inside of this -->
                 <button>
                    <img src="images/project5.png" class="Project Project 5" alt="My fifth project"/>
                </button>
            </li>
    ```

## Summary 
An **ARIA role** prepares the browser or screen reader to understand which interactions to expect. They are used only on rare occasions, and in most cases semantic HTML is recommended.

We can provide a similar experience to users with disabilities as well as users who have all the physical benefits, using statuses which will communicate what things will be displayed on the screen.

---
## ARIA attribute types

States and properties in the ARIA are divided into four categories, and we will explain some attributes of each category that you might use in your portfolio:

1 -  **Widget attributes**

    - aria-autocomplete
        - The aria-autocomplete attribute indicates whether inputting text could trigger display of one or more predictions of the user's intended value for a combobox, searchbox, or textbox and specifies how predictions will be presented if they are made.

    - aria-checked
        - The aria-checked attribute indicates the current "checked" state of checkboxes, radio buttons, and other widgets.

    - aria-disabled
        -The aria-disabled state indicates that the element is perceivable but disabled, so it is not editable or otherwise operable.

    - aria-errormessage
        - The aria-errormessage attribute on an object identifies the element that provides an error message for that object.

    - aria-expanded
        - The aria-expanded attribute is set on an element to indicate if a control is expanded or collapsed, and whether or not its child elements are displayed or hidden.

    - aria-hidden
        - attribute can be used to hide non-interactive content from the accessibility API.

    - aria-invalid
        - state indicates the entered value does not conform to the format expected by the application.

    - aria-label
        - attribute defines a string value that labels an interactive element.

    - aria-placeholder
        - attribute defines a short hint (a word or short phrase) intended to help the user with data entry when a form control has no value.
        - The hint can be a sample value or a brief description of the expected format.

    - aria-pressed
        -  attribute indicates the current "pressed" state of a toggle button.

    - aria-readonly
        - attribute indicates that the element is not editable, but is otherwise operable.

    - aria-required
        - attribute indicates that user input is required on the element before a form may be submitted.

    - aria-selected
        - attribute indicates the current "selected" state of various widgets.

    - aria-sort
        - attribute indicates if items in a table or grid are sorted in ascending or descending order.
    - etc...

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
    - etc ...

### If you would like to learn more about each properties and states, [please click here](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Attributes#aria_attribute_types).



## Interesting resources
- [Videos of screen readers using ARIA](https://zomigi.com/blog/videos-of-screen-readers-using-aria-updated/)
- [Using ARIA - A practical guide for developers:  It suggests what ARIA attributes to use on HTML elements. Suggestions are based on implementation realities.](https://w3c.github.io/using-aria/)
- [Improving form accessibility](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/forms)
- [Etiquetas y relaciones de ARIA](https://developers.google.com/web/fundamentals/accessibility/semantics-aria/aria-labels-and-relationships)
- [HTML 'label' for Attribute](https://www.w3schools.com/tags/att_label_for.asp)

---

# You're done! it's time to [create your portfolio!](./HandsOn.md)

![Aladdin's movie gif - Showtime ](https://media.giphy.com/media/cIh8DK7Or9BpI926WJ/giphy.gif)

## Bibliographic references
- [MDN Web Docs - ARIA](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA)
- [MDN Web Docs - ARIA states and properties](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Attributes)
- [MDN Web Docs - WAI-ARIA Roles](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles)