# Legibilidad

## Códigos

| Retos       | Enlace |
|------------------|--------|
| *VisicCalc* | [Code1](https://github.com/LavinAguado/23-24-eda1/blob/main/entregas/lavinDaniel/VisiCalc.java) |
| *Reto002Eda1*  | [Code2](https://github.com/LavinAguado/23-24-eda1/blob/main/entregas/lavinDaniel/reto002/Main.java) |
| *Reto003Eda1* | [Code3](https://github.com/LavinAguado/23-24-eda1/blob/main/entregas/lavinDaniel/reto-003/Ejemplo.java) |
| *Reto006PRG1* | [Code4](https://github.com/LavinAguado/23-24-prg1/blob/main/entregas/lavinDaniel/reto002/reto-006/Main.java) |
| *Reto004PRG1* | [Code5](https://github.com/LavinAguado/23-24-prg1/blob/main/entregas/lavinDaniel/reto002/reto004/generadorNumero.java) |

## Nombrado

 Cambiar hoja por hojaDeCalculo para mayor claridad. [Code1]((https://github.com/LavinAguado/23-24-eda1/blob/190f0d380d887f47c44a3746e88f719acc6f6560/entregas/lavinDaniel/VisiCalc.java#L10))

Cambiar edicion por modoEdicion para que sea más expresivo. [Code1]((https://github.com/LavinAguado/23-24-eda1/blob/190f0d380d887f47c44a3746e88f719acc6f6560/entregas/lavinDaniel/VisiCalc.java#L9))

leerDireccion() se está utilizando para leer texto, lo que no es coherente con su propósito. [Code2](hhttps://github.com/LavinAguado/23-24-eda1/blob/190f0d380d887f47c44a3746e88f719acc6f6560/entregas/lavinDaniel/reto002/Main.java#L15)

Nombrado inconsistente. [Code5](https://github.com/LavinAguado/23-24-prg1/blob/6e743b42e46835391f859fef86b5162ba5febf3f/entregas/lavinDaniel/reto002/reto004/generadorNumero.java#L3)

Uso de nombres de variables poco descriptivos . [Code5](https://github.com/LavinAguado/23-24-prg1/blob/6e743b42e46835391f859fef86b5162ba5febf3f/entregas/lavinDaniel/reto002/reto004/generadorNumero.java#L9)

## Comentarios

Ausencia de comentarios en todos los códigos.

## Formato y Consistencia 

El bloque para imprimir el encabezado de las columnas podría tener más claridad con una separación visual y simplificación. [Code1](https://github.com/LavinAguado/23-24-eda1/blob/190f0d380d887f47c44a3746e88f719acc6f6560/entregas/lavinDaniel/VisiCalc.java#L65)

La lógica para leer la respuesta y el número se repite. Esto debería encapsularse en un método para simplificar la lectura.. [Code4](https://github.com/LavinAguado/23-24-prg1/blob/6e743b42e46835391f859fef86b5162ba5febf3f/entregas/lavinDaniel/reto002/reto-006/Main.java#L12)

Mensaje de salida poco claro. [Code2](https://github.com/LavinAguado/23-24-prg1/blob/6e743b42e46835391f859fef86b5162ba5febf3f/entregas/lavinDaniel/reto002/reto-006/Main.java#L149)



## Código Muerto 

Esto es redundante porque el modo edición ya se gestiona en el bloque anterior. [Code1](https://github.com/LavinAguado/23-24-eda1/blob/190f0d380d887f47c44a3746e88f719acc6f6560/entregas/lavinDaniel/VisiCalc.java#L55).

El último viewLine(nephews); podría eliminarse si no aporta información nueva tras el delete(). [Code3](https://github.com/LavinAguado/23-24-eda1/blob/190f0d380d887f47c44a3746e88f719acc6f6560/entregas/lavinDaniel/reto-003/Ejemplo.java#L24)



## DRY

Los métodos moverArriba, moverAbajo, moverIzquierda, y moverDerecha son muy similares y repetitivos. Esto podría unificarse en un solo método. [Code1](https://github.com/LavinAguado/23-24-eda1/blob/190f0d380d887f47c44a3746e88f719acc6f6560/entregas/lavinDaniel/VisiCalc.java#L91)

El método movimiento.moverse() se llama dos veces con parámetros ligeramente diferentes. Esto podría simplificarse. [Code2](https://github.com/LavinAguado/23-24-eda1/blob/190f0d380d887f47c44a3746e88f719acc6f6560/entregas/lavinDaniel/reto002/Main.java#L20)

El método viewLine(nephews); se repite varias veces. [Code3](https://github.com/LavinAguado/23-24-eda1/blob/190f0d380d887f47c44a3746e88f719acc6f6560/entregas/lavinDaniel/reto-003/Ejemplo.java#L6)

## YAGNI

El modo edición complica innecesariamente el flujo. Se podría editar directamente sin alternar modos. [Code1](https://github.com/LavinAguado/23-24-eda1/blob/190f0d380d887f47c44a3746e88f719acc6f6560/entregas/lavinDaniel/VisiCalc.java#L9)

El Scanner se declara pero nunca se cierra, lo cual puede causar fugas de recursos [Code4](https://github.com/LavinAguado/23-24-prg1/blob/6e743b42e46835391f859fef86b5162ba5febf3f/entregas/lavinDaniel/reto002/reto-006/Main.java#L5)