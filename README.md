# templete-picow
Para trabajos de microcontroladores

# Ver el directorio de /code/ para como documentar un programa con sus pantallas, etc.

```C
/*
 * Nombre del Archivo: pulgadas.c
 * Autor:   Rodriguez Cruz Luis Fernando 
 * Correo:  l21210421@tectijuana.edu.mx
 * Fecha:   25/10/2023
 * Curso:   Lenguajes de Interfaz, TECNM Campus ITT
 * 
 * Objetivo:
 * Este programa está diseñado para calcular el número de cm en 32 pulgadas, teniendo en cuenta que una pulgada equivale a 2.5 cm.
 *
 * Historial de Revisiones:
 * 25/10/2023      Rodriguez Cruz Luis Fernando  - Creado
 * 25/10/2023      Rodriguez Cruz Luis Fernando  - Actualizado para añadir [característica/corrección]
 *
 */

#include <stdio.h>
#include "pico/stdlib.h"

int main() {
    stdio_init_all();
    
    // Definir el valor en pulgadas
    float pulgadas = 32.0;
    
    // Calcular el valor en centímetros
    float centimetros = pulgadas * 2.54;
    
    // Imprimir el resultado en la consola serie
    printf("%.2f pulgadas son equivalentes a %.2f centímetros\n", pulgadas, centimetros);
    
    while (true) {
        sleep_ms(5000); // Esperar 5 segundos antes de volver a calcular
    }

    return 0;
}


```
