# x86_64-assembly-python-AOT-compiler-and-bindings

These python bindings for x86 assembly enable you to generate, compile, and run assembly instructions during the runtime of your python program.  The bindings also include a python function compiler that can compile decorated functions by traversing the AST (abstract syntax tree) of the function and generating statically typed equivalent assembly functions.  The compiler is limited in functionality, but is capable of utilizing different scalar types such as int, boolean, and float.  All basic operators mimic the behavior of their python equivalent such as div(/), floordiv(//), mul(*), mod(%), add(+), sub(-), lt(<), gt(>), eq(==), ne(!=), and(and), or(or), ge(>=), and le(<=).  Three way comparisons are also supported, for example: -10 < x < 10.  Template functions are also supported and generate different assembly for different template calls to the function.  Array size type hint values can also be passed via template.

To use the compiler, you must have the yasm assembler and gcc (for the ld linker) installed.

## For Contributions

 - This project uses ruff formatter.

