## Read-05

**CSS**- CSS is a language for specifying how documents are presented to users — how they are styled, laid out, etc.

-A document is usually a text file structured using a markup language — HTML is the most common markup language, but you may also come across other markup languages such as SVG or XML.

-Presenting a document to a user means converting it into a form usable by your audience. Browsers, like Firefox, Chrome, or Edge , are designed to present documents visually, for example, on a computer screen, projector or printer.

-CSS can be used for very basic document text styling — for example changing the color and size of headings and links. It can be used to create layout — for example turning a single column of text into a layout with a main content area and a sidebar for related information. It can even be used for effects such as animation

-CSS is a rule-based language — you define rules specifying groups of styles that should be applied to particular elements or groups of elements on your web page.

**Adding CSS**

**With an EXTERNAL style sheet, you can change the look of an entire website by changing just one file!**

Each HTML page must include a reference to the external style sheet file inside the <link> element, inside the head section.

An *INTERNAL* style sheet may be used if one single HTML page has a unique style.

The internal style is defined inside the <style> element, inside the head section.

An *INLINE* style may be used to apply a unique style for a single element.

To use inline styles, add the style attribute to the relevant element. The style attribute can contain any CSS property.

Cascading Order
1. Inline style (inside an HTML element)
2. External and internal style sheets (in the head section)
Browser default

CSS Color-The color property specifies the color of text.
Example- body {color: rgb(201, 76, 76);}
