---
title: "Desarrollo Web Entorno Cliente: JavaScript"
date: 2024-11-20T18:46:47+08:00
draft: false
summary: "Esta página es un resumen de JavaScript de la asignatura Desarrollo Web en entorno cliente"
math: true
---

# Introducción

JavaScript es un lenguaje de programación dinámico y versátil, utilizado principalmente en el desarrollo web. Es esencial para crear páginas web interactivas y mejorar la experiencia del usuario. Aquí tienes los conceptos básicos:

- Lenguaje interpretado: Se ejecuta directamente en el navegador sin necesidad de compilación.
- Multiparadigma: Soporta programación funcional, orientada a objetos y procedimental.
- Basado en eventos: Ideal para manejar interacciones del usuario.

# Tipos de datos:

- String: Cadenas de texto. Ejemplo: "Hola, mundo"
- Number: Números. Ejemplo: 42, 3.14
- Boolean: Valores lógicos. Ejemplo: true, false
- Undefined: Variable declarada pero no inicializada.
- Null: Ausencia de valor.
- Symbol y BigInt: Introducidos en versiones más recientes.
- Objetos: Colecciones de datos clave-valor. Ejemplo: { nombre: "Juan", edad: 30 }.

# Declaración de variables:

- var (obsoleto en muchos casos).
- let (para variables con ámbito de bloque).
- const (para constantes).

# Diferencias principales entre var y let:

Cuando declaramos una variable con var se inicializa automaticamente a undefined mientras que las variables con let no lo hacen, las variables declaradas con var dentro de una funcion existen solo dentro de esta y si no son declaradas dentro de una función son variables globales mientras que las variables con let tienen ámbito de bloque y las variables declaradas con var permiten hoisting mientras que las declaradas con let no.

# Operadores:

- Aritméticos: +, -, *, /, %
- Comparación: ==, ===, !=, <, >
- Lógicos: && (AND), || (OR), ! (NOT)

# Estructuras de control:

- Condicionales:

if (edad > 18) {
  console.log("Mayor de edad");
} else {
  console.log("Menor de edad");
}

ternarios:

let mensaje = (edad >= 18) ? "Eres mayor de edad" : "Eres menor de edad";

- Bucles:

for (let i = 0; i < 5; i++) {
  console.log(i);
}

# Funciones:

- Declaración básica:

function sumar(a, b) {
  return a + b;
}
Funciones flecha (ES6+):

const sumar = (a, b) => a + b;

# Arrays y objetos:

Array: Lista ordenada de elementos.
let frutas = ["manzana", "banana", "pera"];
console.log(frutas[0]); // "manzana"

Objeto: Colección de propiedades.
let persona = { nombre: "Luis", edad: 25 };
console.log(persona.nombre); // "Luis"

#  Manipulación del DOM:

Permite interactuar con elementos HTML:

document.getElementById("miElemento").innerText = "Hola!";