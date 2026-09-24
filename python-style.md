# My very opinionated Python style rules

This is a work in progress.

* Indentation: 4 spaces
* Quote style: double
* Line length:
  * Code: 119
  * Comments: 79
* Breaking long lines:
  * Opening parenthesis on 1st line
  * One item per line, _even if they would all fit on one line_ (does not seem to be enforceable through Ruff, so has to be done manually)
  * Trailing comma on last line
  * Closing parenthesis on its own line
* Ordering of members (except when their order is functionally relevant):
  * 1st order module members, from top to bottom:
    1. Uppercased constants, alphabetically sorted
    2. Snake-cased variables, alphabetically sorted
    3. Classes, alphabetically sorted
    4. Functions, alphabetically sorted
  * Class members, from top to bottom:
    1. Attributes, alphabetically sorted
    2. Properties, alphabetically sorted
    3. Nested classes, alphabetically sorted
    4. `__init__` and `__new__`
    5. Other special dunder methods (`__eq__`, `__lt__`, etc), alphabetically sorted
    6. Abstract methods, alphabetically sorted
    7. Class methods, alphabetically sorted
    8. Regular methods, alphabetically sorted
  * Sequence members, dict keys, imports, function kwargs and other similar listings should always be alphabetically sorted
* Blank lines:
  * Below imports: 2
  * Between classes and top level functions: 2
  * Between methods and properties: 1
  * Between variable/attribute definitions: 0-1 (readability governs)
* Import grouping (1 blank line between each): future, standard library, third party, first party, local folder
