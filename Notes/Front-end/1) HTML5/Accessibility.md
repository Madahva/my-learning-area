## Semantic

Semantic HTML is the foundation of accessibility in a web application. Using the various HTML elements to reinforce the meaning of information in our websites will often give us accessibility for free.

Semantic HTML elements are those that clearly describe their meaning in a human- and machine-readable way. 

Semantically correct HTML helps search engines, screen readers, and other user devices determine the significance and context of web content. It certainly will make your code more accessible, making it easier to read.

Elements such as `<header>`, `<nav>`, `<main>`, `<section>` and `<footer>` are all considered semantic because they accurately describe the purpose of the element and the type of content that is inside them.


## Labeling

Every HTML form control, such as `<input>` and `<textarea>`, needs to be labeled accessibly. We need to provide descriptive labels that are also exposed to screen readers.


## Focus Control

Ensure that your web application can be fully operated with the **keyboard** only.

**Keyboard focus** refers to the current element in the DOM that is selected to accept input from the keyboard.

Heading elements like a `<h2>` are not usually focusable. This isn't a problem — we can make any element programmatically focusable by adding the attribute [`tabindex="-1"`](https://developer.mozilla.org/en-US/docs/Web/HTML/Global_attributes/tabindex) to it. This means _only focusable with JavaScript_. You can't press Tab to focus on an element with a tabindex of `-1` the same way you could do with a `<button>` or `<a>` element (this can be done using `tabindex="0"`).

**Note:** The `tabindex` attribute is great for accessibility edge-cases, but you should take **great care** to not overuse it. Only apply a `tabindex` to an element when you're absolutely sure that making it focusable will benefit your user in some way. In most cases, you should be utilizing elements that can naturally take focus, such as buttons, anchors, and inputs. Irresponsible usage of `tabindex` could have a profoundly negative impact on keyboard and screen-reader users!


## Mouse and pointer events

Ensure that all functionality exposed through a mouse or pointer event can also be accessed using the keyboard alone. Depending only on the pointer device will lead to many cases where keyboard users cannot use your application.


### The keyboard

By far the easiest and also one of the most important checks is to test if your entire website can be reached and used with the keyboard alone.


## Setting the language

Indicate the human language of page texts as screen reader software uses this to select the correct voice settings.

## Color contrast

Ensure that all readable text on your website has sufficient color contrast to remain maximally readable by users with low vision.