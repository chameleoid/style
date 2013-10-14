Chameleoid Styleguide
=====================
To help ensure a unified style across Chameleoid projects, we've prepared the
following styleguide.

### Overview
A similar style should be preserved across most languages, here's a general
overview of what we use:

- [Smart tabs][] - unless where otherwise noted
  * 8-wide tabs recommended, but not required
  * In languages that do not allow tabs, we'll generally use 8-space indentation
- Curly braces should not be on their own line in function definition
- Most projects will be using [Grunt][] for linting and testing

[Smart tabs]: http://vim.wikia.com/wiki/Indent_with_tabs,_align_with_spaces#Smart_tabs
[Grunt]: http://gruntjs.com/

### Local .vimrc
For Vim users, we've prepared a `.vimrc_local.vim` which we recommend [taking a
look at](.vimrc_local.vim)

### Contact
When in doubt, try to keep the same style as the surrounding code, or contact
@rummik on Freenode in #chameleoid.

### Index
1. CSS
  1. LESS
  2. Stylus
2. HTML
  1. Swig
  2. Twig
3. [Javascript](#javascript)
  1. [JSON](#json)
4. [Markdown](#markdown)
5. PHP
6. [YAML](#yaml)


## Javascript
We're using @felixge's [Node.js Style Guide](http://nodeguide.com/style.html),
but with a few changes:

- We aren't enforcing a maximum line width, but it's generally a good idea to
  keep it less than 100 lines
- [Smart tabs][] - as explained in [the overview](#overview)
- Multi-line arrays should have a comma on the final item
  - Right:
    ```js
    var array = [
        'foo',
        'bar',
    ];
    ```

  - Wrong:
    ```js
    var array = [
        'foo',
        'bar'
    ];
    ```

### JSON
JSON should follow the [Javascript styleguide](#javascript) as applicable


## Markdown
- Indentation
  - Use 2-space indentation for nested lists
  - Use 4-space indentation inside code blocks
- Lines should word-wrap at 80 columns
- Try to use reference links where possible, as this makes reading easier
  * When using reference links, try to keep them as near to the end of their
    respective section as possible without making them difficult to see. Think
    of reference links as being in footnotes
  * When in doubt, see this file for reference, or [contact someone](#contact)
    for help
- Unordered lists should mainly use `-`, though `*` may be used for marking
  notes within lists


## YAML
- Use 8-space indentation ([see overview](#overview)), as YAML does not allow
  tabs by spec
