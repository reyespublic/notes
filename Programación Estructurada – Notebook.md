---
pinned: true
tags: [Notebook, School]
title: Programación Estructurada – Notebook
created: '2020-02-16T06:43:09.625Z'
modified: '2020-02-19T22:32:11.971Z'
---

# Programación Estructurada – Notebook

Libreta de apuntes para la clase de *Programación Estructurada*.

## Índice <a name="index"></a>

1. [Definiciones](#definitions)
2. [Apuntadores](#pointer)

***

## Definiciones <a name="definitions"></a> <small>[:arrow_heading_up:](#index)</small>

+ **Modularidad:** es la capacidad que tiene un sistema de ser estudiado, visto o entendido como la unión de varias partes que interactúan entre sí y que trabajan para alcanzar un objetivo común, realizando cada una de ellas una tarea necesaria para la consecución de dicho objetivo.

+ **Acoplamiento:** se refiere al grado de independencia entre módulos. Es preciso minimizar el acoplamiento entre módulos, es decir, minimizar su interdependencia.

+ **Cohesión:** es la propiedad que se refiere a la fortaleza interna de un módulo, es decir, lo fuertemente relacionados que están entre sí las partes de un módulo.

+ **Funciones:** es un segmento de programa que realiza una determinada tarea. *(En C una de las funciones se debe de llamar main(), ya que todo programa de C inicia su ejecución en esa función)*

+ **Pase por Referencia:** se envía la dirección de memoria en la que está almacenada la variable, por ende se puede afectar.

+ **Pase por Valor:** se envía una copia de la variable original, por ende si se modifica el valor no perjudica la variable pasada.

## Apuntadores <a name="pointer"></a> <small>[:arrow_heading_up:](#index)</small>

Un puntero es una **variable que contiene la dirección de memoria** de un dato o de otra variable que contiene al dato en un arreglo. Esto quiere decir, que el puntero apunta al espacio físico donde está el dato o la variable.

```c
char a;
scanf ("%c",&a);
```

> En este caso se le pasa la dirección de memoria de la variable a, la cual tiene reservado un espacio en la memoria por el compilador.

&nbsp;

Ejemplo de uso de punteros.

```c
#include <stdio.h>

int main()
{

int array[10]={0,2,3,5,5,6,7,8,9,10}; // Declarar e inicializar un array.
int *puntero = &array[0]; // Le damos la dirección de inicio del array
int i; // Variable contadora

for (i=0;i<10;i++) {
  printf("%d\n",*(puntero+i)); // Imprimimos los valores del puntero.
}

return 0;
}
```


