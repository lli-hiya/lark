# Main Features
 - Earley parser, capable of parsing any context-free grammar
   - Implements SPPF, for efficient parsing and storing of ambiguous grammars.
 - LALR(1) parser, limited in power of expression, but very efficient in space and performance (O(n)).
   - Implements a parse-aware lexer that provides a better power of expression than traditional LALR implementations (such as ply).
 - EBNF-inspired grammar, with extra features (See: [Grammar Reference](grammar.md))
 - Builds a parse-tree (AST) automagically based on the grammar
 - Stand-alone parser generator - create a small independent parser to embed in your project.
 - Automatic line & column tracking
 - Automatic terminal collision resolution
 - Standard library of terminals (strings, numbers, names, etc.)
 - Unicode fully supported
 - Extensive test suite
 - Python 2 & Python 3 compatible
 - Pure-Python implementation

[Read more about the parsers](parsers.md)

# Extra features

  - Import rules and tokens from other Lark grammars, for code reuse and modularity.
  - Import grammars from Nearley.js
  - CYK parser

### Experimental features
  - Automatic reconstruction of input from parse-tree (see examples)

### Planned features (not implemented yet)
 - Generate code in other languages than Python
 - Grammar composition
 - LALR(k) parser
 - Full regexp-collision support using NFAs
