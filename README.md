DerelictMantle
================
*Unofficial Derelict binding.*

A port of [the experimental reverse-engineered header][4] of the [AMD Mantle][1] library for the D Programming Language.
Currently only MS Windows is supported, please make sure that you have a suitable GCN AMD/ATI GPU/APU and the mantle32.dll (latest catalyst driver) is in your system path.

Please see the pages [Building and Linking Derelict][2] and [Using Derelict][3], in the Derelict documentation. In the meantime, here's some sample code.

```D
import derelict.mantle.mantle;

void main() {
    // Load the mantle32 library.
    DerelictMantle.load();

    // Now mantle functions can be called.
    ...
}
```

[1]: http://www.amd.com/en-us/innovations/software-technologies/mantle#downloads
[2]: http://derelictorg.github.io/compiling.html
[3]: http://derelictorg.github.io/using.html
[4]: https://github.com/Overv/MantleHelloTriangle
