# fbfc (Flame.Brainfuck)
fbfc is a brainfuck front-end for the [Flame compiler framework](https://github.com/jonathanvdc/Flame).
It currently supports compiling brainfuck code (*.bf) for the .Net CLR.

## Compiling fbfc
You'll need dsc, which you can obtain at [Flame's releases page](https://github.com/jonathanvdc/Flame/releases).
Make sure your PATH environment variable is set to a value that allows the 'dsc' command to be used anywhere.
Now you can compile fbfc with:

    fbfc_build.sh
    
--OR--
    
    fbfc_build.bat
    
Both of these files instruct dsc to compile fbfc and then dump all Flame libraries that shipped with dsc in fbfc's bin/ folder.

## Compiling brainfuck with fbfc
fbfc can be used like any (Flame) console compiler.

For now, compile brainfuck with:
    
    fbfc <source file.bf> -platform clr/release-console
