# Python Coding Standards

## Basics

### Identifiers
  - Local variables
    - snake casing
  - Global variables
    - all upper case, snake casing
  - Method names
    - snake casing
    - module/class specific methods prefixed with underscore
  - Class names
    - camel casing
  - Script file names
    - snake casing
  - Data files
    - hyphenated, lower case
  - Ignoring values
    - double underscore (e.g. `a, __ = (1, 2)`)

### Formatting
  - Indentation
    - 4 spaces
  - Element spacing
    - 1 blank line before the next method declaration
      - except for top level methods (script level) which uses 2 blank lines in between
    - 2 lines from the bottom of import block
      - all imports declared at the beginning of script
  - Favour parentheses/brackets over multi-line escape symbol (`\`)
    - Examples:
      ```
      multiline = (
        "this is"
        " a "
        " multiline "
        " string "
      )
      ```
  - Spaces around operators like `=`, `>`, `<`, etc.
  - Line width
    - PEP 8 specifies that the maximum line limit is up to 79 characters
    - This can be extended from anywhere between 80 to 100 characters

## Guidelines

### Comments
  - Basically, if it does not add important information that can't be expressed in interpreted code, remove it.
  - When beginning to explain what a code block does, *refactor*!
  - Minimise comments to the following categories
    - TODOs and FIXMEs
      - TODO - something that could/must be done in the future
      - FIXME - important things to resolve
    - The why's and **not** the how's
    - Python docstrings

### Tools
  - All agreed upon coding standards should as much as possible be expressed as IDE configuration and shared among team members
