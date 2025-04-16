# icc — Indent-C Compiler

`icc` is the compiler for **Indent-C**, a clean, indentation-based language inspired by Python but powered like C. It compiles `.ic` source files directly to native executables, just like `gcc` does for `.c`.

## Usage

```bash
icc [--keep-c] [-o outputfile] <source.ic>
```

### Arguments

- `<source.ic>`: Your Indent-C source file.
- `-o <outputfile>`: Optional. Specify the name of the final executable.
- `--keep-c`: Optional. Retains the intermediate C file for inspection or debugging.

## Examples

Basic compile:

```bash
icc hello.ic
./hello
```

Custom output name:

```bash
icc -o greet hello.ic
./greet
```

Keep intermediate C file:

```bash
icc --keep-c hello.ic
```

## Similarity to `gcc`

| Feature         | `icc`               | `gcc`             |
|----------------|---------------------|-------------------|
| Input file     | `file.ic`           | `file.c`          |
| Output default | `file`              | `a.out`           |
| `-o` flag      | Custom executable   | Custom executable |
| Optional flag  | `--keep-c` (extra)  | `-save-temps`     |
