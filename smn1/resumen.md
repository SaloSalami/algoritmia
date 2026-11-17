# Semana 1 — Introducción a los algoritmos

Esta carpeta contiene las actividades de la primera semana: dos ejercicios de instrucciones, cuatro programas secuenciales principales y tres prácticas complementarias.

Los programas PSeInt están en ``; los diagramas de flujo entregables están en `img/`.

## Actividades

| N.º | Actividad | Archivo o explicación |
|---:|---|---|
| 1 | Cruzar la quebrada | Solución en la sección «Cruzar la quebrada» de este archivo |
| 2 | Preparar un tinto | [tinto.md](tinto.md) |
| 3 | saludo | [saludo.psc](saludo.psc) · [img/saludo.png](img/saludo.png) |
| 4 | Edad en días | [edad.psc](edad.psc) · [img/edad.png](img/edad.png) |
| 5 | Calculadora de propinas | [Propinas.psc](Propinas.psc) · [img/Propinas.png](img/Propinas.png) |
| 6 | Promedio de tres notas | [promedio.psc](promedio.psc) · [img/promedio.png](img/promedio.png) |
| 7 | Área y perímetro de un rectángulo | [rectangulo.psc](rectangulo.psc) · [img/rectangulo.png](img/rectangulo.png) |
| 8 | Celsius a Fahrenheit | [temperatura.psc](temperatura.psc) · [img/temperatura.png](img/temperatura.png) |
| 9 | Dividir una cuenta | [cuenta.psc](cuenta.psc) · [img/cuenta.png](img/cuenta.png) |

## Lógica de los programas

- **saludo:** lee un nombre como cadena y lo concatena con el texto del saludo.
- **Edad en días:** multiplica la edad en años por 365. El resultado es aproximado porque no cuenta los años bisiestos.
- **Propinas:** calcula el porcentaje de propina, lo suma a la cuenta y divide el total entre las personas. En esta primera versión se supone que la cantidad de personas es mayor que cero; la validación se trabaja en la semana 2.
- **Promedio:** suma tres notas y divide el resultado entre tres.
- **Área y perímetro:** usa `base × altura` para el área y `2 × (base + altura)` para el perímetro.
- **Celsius a Fahrenheit:** aplica `(Celsius × 9 / 5) + 32`.
- **Dividir cuenta:** calcula propina y total, y reparte el pago. Como en la primera calculadora, se supone que la cantidad de personas es mayor que cero.

## Pruebas de referencia

La tabla presenta entradas de referencia y las salidas esperadas para cada programa.

| Programa | Entradas | Resultado esperado |
|---|---|---|
| saludo | `Ana`; `Luis` | `Hola, Ana`; `Hola, Luis` |
| Edad en días | 20 años; 18 años | 7.300 días; 6.570 días aproximadamente |
| Propinas | $120.000, 10 %, 4 personas; $84.000, 15 %, 4 personas | Propina $12.000, total $132.000, $33.000 por persona; propina $12.600, total $96.600, $24.150 por persona |
| Promedio de tres notas | 4, 3.5 y 4.5; 3, 3 y 4 | 4; aproximadamente 3.33 |
| Área y perímetro | Base 5, altura 3; base 2.5, altura 4 | Área 15 y perímetro 16; área 10 y perímetro 13 |
| Celsius a Fahrenheit | 0 °C; 25 °C | 32 °F; 77 °F |
| Dividir una cuenta | $120.000, 10 %, 4 personas; $84.000, 15 %, 4 personas | Propina $12.000, total $132.000, $33.000 por persona; propina $12.600, total $96.600, $24.150 por persona |

## Entregables de la semana

- Solución ordenada del cruce de la quebrada.
- Instrucciones precisas para preparar un tinto en `tinto.md`.
- Cuatro programas secuenciales principales en PSeInt y sus diagramas de flujo PNG.
- Tres prácticas complementarias en PSeInt y sus diagramas.
- Dos casos de prueba por programa, con sus entradas y salidas esperadas.

## Cruzar la quebrada

El campesino debe pasar el perro, la gallina y el maíz. La canoa solo lleva al campesino y uno de los tres. No puede dejar solos al perro con la gallina ni a la gallina con el maíz.

1. Llevar la gallina a la otra orilla.
2. Regresar solo.
3. Llevar el perro a la otra orilla.
4. Regresar con la gallina.
5. Llevar el maíz a la otra orilla.
6. Regresar solo.
7. Llevar la gallina a la otra orilla.

La gallina regresa en el paso cuatro para no quedar sola con el perro ni con el maíz.