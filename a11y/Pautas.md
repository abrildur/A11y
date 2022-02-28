## The more you know... 

Having now learned about the advantages of web accessibility. It is time for you to learn about some institutions and organizations that ensure compliance with accessibility laws and standards.

# What is WCAG?

 **Web  Content Accesibility Guidelines** or also known as "WCAG" are a set of recommendations for creating more accessible web content.

## WCAG History

They are created by the **W3C _(World Wide Web Consortium)_**, who are the ones who created the standards we use to build the web (HTML, CSS), and within this organization there are different initiatives that address specific issues, such as the **WAI (Web Accessibility Initiative)**.

WAI is a W3C initiative **whose goal is to ensure web accessibility**, it provides guidelines for implementing accessibility.

It is important to know that the current **WCAG** level is **2.0**, which means that as our technologies continue to grow, the standard will also grow with them.

According to WCAG, we must comply with 12 conformance criteria that are divided into three levels. The three levels enable us to decide how much investment we will make in web accessibility.

- **Level A** is the lowest level. 
	- It guarantees a basic accessibility for our products.
- **Level AA** is the intermediate level.
- **Level AAA** is the highest level. 
	- The level is often used by companies that work with governments or universities to guarantee that their content, which is critical to the public, can be accessed by anyone.

Web Content Accessibility Guidelines guide us in implementing web accessibility. They can be used throughout the entire product development process, from the conception of the idea for what we are trying to build, through the design of styles and interfaces, until we write code and perform quality testing. We should keep these points in mind when building pages, products, and applications that work for all users regardless of their capabilities, devices, or preferences.

## Explanation of the 12 compliance criteria
In spite of the fact that the guidelines (WCAG) are very comprehensive and continue to grow as our technologies progress, **is important to know the four principles** that guide us to make specific decisions at the product level. Each principle contains conformity criteria that can be interpreted based on the level of WCAG that should be applied to your website. 

As we move through this reading, we will take a closer look at the conformance criteria in order to better understand what we can find inside WCAG. 

Let's start with the first principle:
1. **Perceivable**
	- Information and user interface components must be presentable to users in ways they can perceive.
		- This means that users must be able to perceive the information being presented (it can't be invisible to all of their senses)
<br>

	We want to: <br>
	
	1.1 Ensure that we are providing textual alternatives for all non-textual content.

	1.2 Offer alternatives to the media (like subtitles or scripts for videos or audios).
	
	1.3 Provide content that can be presented in a variety of ways without losing its structure or information.
	
	1.4 Make it easier for users to see and hear content, such as separation between foreground and background.

2. **Operable**
-  User interface components and navigation must be operable.
	- _When we talk about Operable, we want our site to be easy to use and navigate, that it can be navigated using different methods and with a mouse and/or keyboard._
	<br>
	<br>

	2.1 Provide keypad access to all functionality
	
	2.2 Provide enough time for users to read and use the content (when making time-outs, communicate them clearly and provide the option of asking for more time if necessary).
	
	2.3 Do not use elements that glow or move too quickly as they may cause seizures, spasms, or convulsions.
	
	2.4 Enable users to navigate, find content, and determine where they are on our sites.

3. **Understandable**
- Information and the operation of user interface must be understandable.
	- This means that users must be able to understand the information as well as the operation of the user interface (the content or operation cannot be beyond their understanding)
	<br>
	<br>

	3.1 Make text readable and understandable by considering text sizes and color contrast.
	
	3.2 Ensure that web pages are predictable in appearance and operations.
	
	3.3 Provide instructions to avoid errors and opportunities for correction when they do occur.

4. **Robust**
- Content must be robust enough that it can be interpreted reliably by a wide variety of user agents, including assistive technologies.
	- This means that users must be able to access the content as technologies advance (as technologies and user agents evolve, the content should remain accessible)
	<br>
	<br>
4.1 Ensure compatibility with current and future applications, including assistive technologies

These are the conformance criteria for WCAG version 2.0. You can read more about the requirements at each level by visiting the [documentation](https://www.w3.org/TR/WCAG20/). What surprises you the most?

![Salem the cat reading](https://media.giphy.com/media/iqRgU7mFDGeUU/giphy.gif)

# Designing for everyone
> _"The power of the Web is in its universality. Access by everyone regardless of disability is an essential aspect,"_ said Tim Berners-Lee, W3C Director and inventor of the World Wide Web.

We'll share some tips on how you can design for everyone.

- **Ensure the colors you use have adequate contrast.**
	- Some people have different ways of perceiving color or may be color blind. 
		- We need to ensure that the contrast is high enough to distinguish a background from a content. Sometimes when we see yellow backgrounds used with white text, we only think about aesthetics, but we need to try to create products that are not only eye-catching/attractive, but also suitable for any type of audience.
<br>

- **Ensure that color coding is not the only way to relate content.**
	- To ensure that all users can access the content when grouping content by color, you should provide an alternative such as a border, icon, or category title.
<br>

- **Design taking into account the "focus" and "active" states of the components**.
	- By default, when we program forms, buttons, or other HTML elements, the border or underline is left, this is important not to remove because this is a visual guide for many people or for people who are browsing the keyboard.
<br>

- **Adds labels and descriptive text to form fields**.
	- Adding a descriptive label such as Aria-Labels is crucial since users of the _tab_ will not be able to view all titles. 
	- A screen reader should also be able to hear a message on the form when an error occurs, in addition to the button/border changing color.
<br>

- **Write descriptive content that can replace videos and images**.
	- We upload images or videos that contain very important information that may not be accessible to a person using screen readers, so by keeping the text out of the videos and images, screen readers will be able to hear the interpretation of these elements.
		- Suppose you want to include an image of a puppy that is important for your website, add an alt tag so that screen reader users can know what is in that section. 
<br>

- **Ensure that animations do not block access to web page content**.
	- This is closely related to responsive design.
		- A page where we must click to execute an animation and this will show us the text means that the basic text has been blocked by the animation. 
			- This is also not a good practice, and it is not a good practice that users are bombarded with flashes when accessing a page. 


## Interesting Articles
More information about UX Design can be accessed here so you can create more content and products that are accessible to all.
- [NielsenNorman Group - 10 Usability Heuristics for User Interface Design](https://www.nngroup.com/articles/ten-usability-heuristics/)

- [Interaction Design Foundation - User Interface Design Guidelines: 10 Rules of Thumb](https://www.interaction-design.org/literature/article/user-interface-design-guidelines-10-rules-of-thumb)

- [Laws of UX](https://lawsofux.com/)
<br>

# Go to the next lesson: [Assistive Technology](./AssistiveTech.md)


![Patricio's Gif - I'm rooting for you](https://media.giphy.com/media/12XDYvMJNcmLgQ/giphy.gif)
---

# Bibliographic References
- [W3C - Introduction to Understanding WCAG 2.0](https://www.w3.org/TR/UNDERSTANDING-WCAG20/intro.html) 
- [W3C - Module 4: Principles, Standards, and Checks](https://www.w3.org/WAI/curricula/foundation-modules/principles-standards-and-checks/)