English Version (GitHub Project Description)
Regex Semantic Fault Detection

Regular expressions are widely used in modern software systems, but they often contain semantic faults—patterns that are syntactically valid yet behave differently from the developer’s intended specification. Such issues can lead to incorrect data processing, security vulnerabilities, and unexpected program behavior.

This project provides an automata-based testing framework for detecting semantic bugs in regular expressions. The approach converts a regular expression into its minimal deterministic finite automaton (DFA) and systematically generates test cases guided by Prime Path Coverage (PPC), a strong structural coverage criterion in software testing.

To address the common problem of excessively large test suites, the framework incorporates a multi-stage reduction strategy that combines minimum-flow-based path selection, structural path clustering, and pairwise-based test string generation. This design enables effective detection of semantic faults while maintaining a compact and practical test suite.

Key Features

Automata-Based Analysis
Transforms regular expressions into minimized DFAs to enable structural testing.

Prime Path Coverage Testing
Generates test paths guided by the Prime Path Coverage criterion to improve fault detection capability.

Multi-Stage Test Suite Reduction
Reduces redundant tests through minimum-flow path optimization, similarity-based clustering, and pairwise string generation.

Efficient Test Generation
Produces compact test suites while preserving strong coverage of the automaton structure.

Supported Regular Expression Features

The framework supports standard regular expression operators, including:

Concatenation

Union (|)

Kleene star (*)

One-or-more (+)

Optional (?)

Bounded repetition ({m,n})

Character classes ([a-z], [0-9])

Predefined character classes (\d)

Note:
Non-regular features such as backreferences and lookaround assertions are not supported.
