# Tools: Text Editor

This is a simple text editor in a web browser; part of the ongoing Creative Coding series of experiments.
The main aim is to study all the simple interactions that we take for granted with modern editors and IDE and see how to implement these features.
One of my motivation is to explore alternative to Codepen for my teaching session at Alba this coming February and build a tool for me to share live code examples with the students. The development of such a tool lies at the cross roads of different projects involving realtime video mix on a canvas, reactive and genrative svg editor and various image generators.

Things to ponder: how things work in general
- when the cursor moves,
- when a key is pressed like '"<([{ and it auto-closes the symbol
- when html, js, css, svg (etc) tags are auto-completed
- when usign syntax highlighting
- to have multiple selection are copied and/or pasted
- when decoupling selection and cursor position (like in a unix terminal)

Things to work on next
- [ ] make it possible to write the code of this text editor within itself, asap
  - [X] multi-lines text paste
  - [ ] multi-lines text copy
    - issue might be similar to difficult selection issue on Notion.so 
  - [ ] multi-lines file import
  - [ ] multi files opened; tabs?
  - [ ] save and open files
  - [ ] keep the file when the page is reloaded; webstorage api
  - [ ] use an automated workflow; webpack/grunt/gulp to watch the files; use browsersync
- [ ] Document 
  - the use of Valet
  - the use of the console; plan/think the real need for an internal console
- [ ] Editor
  - [ ] Delete a line
  - [ ] Select across multiple lines
    - [ ] shortcuts, point-and-click
    - [ ] examples: Nano/Vim, Notion.so, Sublime Text, Acme (Plan9), Ed, Sam (text-command-language vs mouse-command-language)
- [ ] real time preview
  - how to assemble the content of the <li> into a single text and interpret it
      - js: can use eval()
      - how to design the ability to change the language: svg, css, html, js etc.
- [ ] text selection, shortcuts and meta actions (
  - move this line up, 
  - convert upper/lowercase, 
  - prettify JSON, 
  - fold/unfold section, 
  - indentation
  - multiple panes(i3)/tabs/files 
  - Languages
    - Markdown
    - SVG
    - Javascript
    - Three.js
  - continue: establishing a list

Some features to be considered:
- preview of the code; similar to Codepen
  — how to interpret the text cut inide multiple elements.
  - how to implement/link with git in mind
- preview could have specific feature for SVG, like  with point and click to select code element, coordinates of points, etc
- open/save file; with the Filesystem API; export content
- previous experiments. and tools 
  - SVG Generate tool used a Nodejs backend to manipulate the files freely
  - SVG Generate tools https://github.com/jrgd/svg-generate
  - Notes app
  - Creative Codepending workshop — assignments not published yet
- Filesystem API https://developer.mozilla.org/en-US/docs/Web/API/FileSystem#Browser_compatibility
- Syntax Highlighter https://github.com/victorqribeiro/syntax
- HTML5 contentEditable https://developer.mozilla.org/en-US/docs/Web/HTML/Global_attributes/contenteditable
- Notion.so

Some background thoughts
- https://tom.preston-werner.com/2010/08/23/readme-driven-development.html
- https://www.simonewebdesign.it/how-to-make-browser-editor-with-html5-contenteditable/
- https://web.eecs.utk.edu/~azh/blog/challengingprojects.html

Notes
- Shortcurts with combo keys:
  The event object has a metaKey property that can be tested along the keycode liek so:
  ```case event.which = 86 && event.metaKey == true:``


----
"Build your own tools.", Daniel Nordh.