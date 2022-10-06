# HTML Links, JS Functions, and Intro to CSS Layout

## Learn HTML

1. to create a basic link we wrap text or other content inside an **<a>** element and using the **href** attribute.
2. The *href* element contains the web address.
3. Some ways we can ensure links on our pages are accessible to all readers is:
    - Don't repeat the URL as part of the link text — URLs look ugly, and sound even uglier when a screen reader reads them out letter by letter.
    - Don't say "link" or "links to" in the link text — it's just noise. Screen readers tell people there's a link. Visual users will also know there's a link, because links are generally styled in a different color and underlined (this convention generally shouldn't be broken, as users are used to it).
    - Keep your link text as short as possible — this is helpful because screen readers need to interpret the entire link text.
    - Minimize instances where multiple copies of the same text are linked to different places. This can cause problems for screen reader users, if there's a list of links out of context that are labeled "click here", "click here", "click here".

## CSS Layout

1. **Normal flow** means the way that webpage elements lay themselves out if you haven't changed their layout.
2. The difference between **block-level** and **inline** elements are: a block line element fills available inline space of the parent element containing it and grows along the block dimension to accommodate its content. A inline element is just the size of their content and you cannot  set width or height on inline elements.
3. **Static** positioning is the default for every html element.
4. A few advantages to using **absolute positioning** on an element is: you can create isolated UI features that doesn't interfere with the layout of other elements on the page. Also positioning is relative to the containing element not the position it was in the control flow originally.
5. The key difference between *fixed* and *absolute* positioning is absolute positioning fixes an element in place relative to its nearest positioned ancestor (the initial containing block if there isn't one), fixed positioning usually fixes an element in place relative to the visible portion of the viewport.

## Learn JS

1. The difference between a **function declaration** and a **function invocation** is a declaration is just declaring the name and it's existence. Invocation is using the declaration on code.
2. The difference between a parameter and an argument is function parameters are the names listed in the function's definition. Function arguments are the real values passed to the function.

## Pair Programming

Some benefits of pair programming are:

- Two people can work though a problem better than one.
- Multiple eyes looking at the same code can help to spot errors quicker.
- Builds emotional intelligence.
- It can help teach each other new skills that one might know but not the other.
- Help prepare for working in the field on group projects.

### Sources

- <https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Normal_Flow>
- <https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Positioning>
- <https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Creating_hyperlinks>
- <https://www.codefellows.org/blog/6-reasons-for-pair-programming/>

[Back To Home](../README.md)
