# Tools: Text Editor

This is a simple text editor in a web browser; part of the ongoing Creative Coding series of experiments.
The main aim is to study all the simple interactions that we take for granted with modern editors and IDE and see how to implement these features.

Think about how things work:
- when the cursor moves,
- when a key is pressed like '"<([{ and it auto-closes the symbol
- when html, js, css, svg (etc) tags are auto-completed
- when usign syntax highlighting
- to have multiple selection are copied and/or pasted
- when decoupling selection and cursor position (like in the terminal)

Some features to be considered:
- preview of the code; similar to Codepen
  — how to interpret the text cut inide multiple elements.
- preview could have specific feature for SVG,like  with point and click to select code element, coordinates of points, etc
- open/save file; with the Filesystem API; export content

----
"Build your own tools.", Daniel Nordh.