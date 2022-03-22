# toodots

Implementación de un compilador usando CUP y JLex.

Tras analizar varios lenguajes de programación poco comunes, hemos visto uno que nos ha llamado especialmente la atención: [*Chef*](http://progopedia.com/language/chef/).  
*Chef* es un lenguaje de programación extremadamente esquemático en cuanto a su estructura pero se expresa con una retórica en demasiado alto nivel.  
Vamos a desarrollar un lenguaje similar pero atajando el uso excesivo de lenguaje natural con simbología más abreviada –con muchos puntos– y respetando ciertas reglas intuitivas que iremos describiendo a lo largo del [siguiente documento](https://github.com/martinfdezdg/Custom-Programming-Language/blob/main/toodots_doc.pdf).

## Procedimiento de compilación
> Abrir terminal en el directorio /toodots

Compilación AnalizadorLexicoTiny.l:
```shell
sh compile/compila_alex.sh
```

Compilación Tiny.cup:
```shell
sh compile/compila_asint.sh
```

Compilación proyecto completo:
```shell
sh compile/compila.sh
```

## Procedimiento de ejecución
> Abrir terminal en el directorio /toodots

Pruebas automáticas de muestreo
```shell
sh tests/basicos/"nombre".sh
sh tests/clases/"nombre".sh
```

Pruebas automáticas de comprobación y vinculación
```shell
sh tests/errores/test_tipos.sh
sh tests/errores/test_vinculacion.sh
```

Pruebas automáticas de generación de código
```shell
sh tests/codigo/"nombre".sh
```
