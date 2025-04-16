# Indent-C: C Syntax with Pythonic Indentation

Indent-C is a minimal extension of the C language that replaces braces with indentation and colons, offering a streamlined syntax familiar to Python developers. It preserves C’s performance and ecosystem while simplifying the writing and reading of structured code.

## Why Indent-C?

Many developers coming from Python subconsciously use indentation and colons to express structure. This often causes friction when switching to C’s brace-heavy syntax. Indent-C reduces that context-switching by aligning C’s control structures with Python’s visual clarity, without sacrificing low-level control.

### Benefits

- Familiar indentation-based syntax
- No brace delimiting for control flow
- Easier visual parsing and cleaner diffs
- Fully compatible with C semantics

## Syntax Comparison

### Standard C

```c
#include <stdio.h>

int main() {
    int x = 5;
    if (x > 0) {
        printf("Positive\n");
    } else {
        printf("Non-positive\n");
    }
    return 0;
}
```

### Indent-C

```c
#include <stdio.h>

int main():
    int x = 5;
    if (x > 0):
        printf("Positive\n");
    else:
        printf("Non-positive\n");
    return 0;
```

## Use Cases

- C programmers seeking a cleaner syntax for prototyping or scripting.
- Python developers writing embedded code, systems utilities, or high-performance modules.
- Teaching environments bridging the gap between Python and C.

Indent-C focuses on reducing syntactic overhead while retaining the power, performance, and familiarity of C.
