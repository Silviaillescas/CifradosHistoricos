# Implementación de Cifrados Históricos

## Descripción

La presente tarea tiene como finalidad implementar de forma manual distintos cifrados históricos, aplicando los fundamentos básicos de la criptografía clásica.

Aunque estos algoritmos no se utilizan actualmente para proteger información real, su estudio permite comprender conceptos esenciales como:

- Representación de la información  
- Transformaciones reversibles  
- Confusión y difusión  
- Análisis criptográfico básico  

---

## Contenido del Proyecto

El notebook incluye las siguientes implementaciones:

### 1. Cifrado César

Algoritmo de sustitución simple que desplaza cada letra del mensaje un número fijo de posiciones dentro del alfabeto.

**Funciones implementadas:**

- `cesar_cifrar(mensaje, desplazamiento)`
- `cesar_descifrar(mensaje, desplazamiento)`

**Características:**

- Soporta letras mayúsculas y minúsculas.
- Conserva espacios y caracteres no alfabéticos.
- Implementación manual usando operaciones aritméticas modulares.

---

### 2. Cifrado ROT13

Caso particular del cifrado César con un desplazamiento fijo de 13 posiciones.

**Función implementada:**

- `rot13(mensaje)`

**Características:**

- No requiere clave.
- Aplicar ROT13 dos veces devuelve el mensaje original.
- Implementación independiente.

---

### 3. Cifrado Vigenère

Cifrado polialfabético que utiliza una clave alfabética para generar desplazamientos variables.

**Funciones implementadas:**

- `vigenere_cifrar(mensaje, clave)`
- `vigenere_descifrar(mensaje, clave)`

**Características:**

- La clave se repite automáticamente cuando es necesario.
- Solo las letras consumen caracteres de la clave.
- Conserva signos y espacios.
- Implementación manual sin uso de librerías externas.

---

### 4. Análisis de Frecuencia

Herramienta auxiliar para el estudio de cifrados por sustitución simple.

**Función implementada:**

- `analisis_frecuencia(mensaje)`

**Características:**

- Cuenta ocurrencias de cada letra.
- Normaliza a mayúsculas.
- Calcula porcentaje relativo respecto al total de letras.
- Permite observar patrones útiles para criptoanálisis básico.

---

## Restricciones Cumplidas

- No se utilizaron librerías criptográficas.
- No se emplearon funciones nativas de cifrado.
- No se usaron funciones externas de conversión.
- La lógica fue implementada manualmente utilizando estructuras básicas del lenguaje.

---

## Estructura del Desarrollo

El trabajo se encuentra organizado en un notebook que incluye:

- Secciones explicativas.
- Implementación de cada algoritmo.
- Pruebas básicas de verificación.

