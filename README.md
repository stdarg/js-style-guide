JavaScipt style Guide
=====================

My style guide for working in JavaScript. Each item exists to support quality, not subjective visual style. Each item has a rationale to back up its existence.

Each style items exists as a recommendtation. Reasons exist to break any style, but they are rare and should provoke thought.

1. Use 4-space indentation.
    1. Not everyone has excellent eyesight. To those with poorer eyesight, figuring out which nesting level a piece of code belongs is harder than when using 4-space indentation. 
    1. The main reason to use less than 4-space indentation is to conserve horizontal space for additional indentation. If you are indenting more than 4 times, you code is harder read. Rather than spave space by using narrower indentations, indent less. There are many tools to avoid excessive indentation: objects, modules, functions, async frameworks - use them.
1. Don't Repeat Yourself (DRY).
    1. Have one piece of code in exactly one place. Reuse through copy-and-paste is an anti-pattern, it duplicates bugs significantly increases maintenance costs.
    1. If you see a few lines repeated a dozen times throughout your code, consolidate it into a function, object, module - it will be easier to test and maintain.
1. Create all code to be tested.
    1. If you make code modular, either through OOP or procedural code, that can be included in anywhere, it can be included in a testing framework.
    1. If you write code that is tightly coupled to either global objects or larger frameworks, the code becomes harder to test in isolation. Design your code for functional testing in isolation.
1. Always use descriptive variable names.
    1. Arguably, using i, j, k and l for loop iterators are descriptive because the pattern is prevalent. However using i for a boolean flag to signal early terminal from a loop is cryptic.
    1. There is a point, however, when overly long names reduce clarity. Strive for both descriptive clarity in names and brevity.
1. Comment your code.
    1. Comment often, but not so often that the code itself is hard to read.
    1. Use JSDoc style comments.
    1. Make your comments descriptive to answer "Why is this here?" It's the first question, programmers looking at your code will ask.
    1. Don't answer "What is happening?" when looking at the code answers the question instantly.
    1. Don't be too busy to comment code. You'll end up not saving you or the organization andy time.