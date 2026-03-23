# 🔁 Práctica de Control de Flujo: Bucle `for`

**Tema:** Estructuras Iterativas Exactas (`for`).
**Contexto:** Ejercicios progresivos basados en aplicaciones reales.

---

## 🟢 Reto 1: Generador de Tablas de Estudio (Nivel Básico)

**Estructura a practicar:** Uso fundamental del ciclo `for` (Inicialización, condición e incremento).

Una escuela primaria necesita una herramienta rápida para que los profesores puedan generar las tablas de multiplicar de cualquier número en la pantalla para sus alumnos.

### 📝 Descripción del Problema

Desarrolla un programa en Java que solicite al usuario un **número entero**. Utilizando un ciclo `for`, el programa debe calcular e imprimir la tabla de multiplicar de ese número desde el 1 hasta el 10.

### 📤 Salida Esperada

* **Ejemplo Entrada (`Número: 7`):**

```text
--- Tabla de Multiplicar del 7 ---
7 x 1 = 7
7 x 2 = 14
7 x 3 = 21
...
7 x 10 = 70
----------------------------------
```

## 🟡 Reto 2: Control de Calidad de Aguacates (Nivel Intermedio)

**Estructura a practicar:** Ciclo `for` combinado con condicionales (`if-else`) y variables contadoras.

Una empacadora agrícola necesita un programa para muestrear lotes de aguacate. El supervisor indicará cuántos aguacates va a pesar en la muestra, y el sistema debe clasificar cuántos se van a exportación y cuántos se quedan para venta nacional.

### 📝 Descripción del Problema

1. El programa debe preguntar primero: **"¿Cuántos aguacates vas a revisar en este lote?"** (Esta será la cantidad de vueltas de tu ciclo).
2. Usar un bucle `for` que se repita exactamente esa cantidad de veces.
3. En cada iteración, el programa debe pedir el **peso del aguacate en gramos**.
4. Usar un `if-else` adentro del ciclo: Si el peso es mayor o igual a `210` gramos, sumar 1 a la variable de Exportación. Si es menor, sumar 1 a la variable Nacional.
5. Al terminar el ciclo, imprimir el resumen del lote.

### 📤 Salida Esperada

* **Ejemplo Entrada (`Cantidad a revisar: 4`):**

```text
Muestreo de Lote iniciado...
Peso del aguacate 1 (g): 220
Peso del aguacate 2 (g): 195
Peso del aguacate 3 (g): 250
Peso del aguacate 4 (g): 205

--- RESUMEN DEL LOTE ---
Total revisados: 4
Calidad Exportación: 2 piezas
Calidad Nacional: 2 piezas
```

## 🔴 Reto 3: Reporte Climático del Nevado de Colima (Nivel Avanzado)

**Estructuras a practicar:** Ciclo `for`, variables acumuladoras y búsqueda de valores máximos y mínimos.

Los guardabosques del Parque Nacional Nevado de Colima registran la temperatura exacta una vez al día. Al final de la semana, necesitan un reporte automático que les indique el promedio, así como el día que hizo más frío y el día más cálido.

### 📝 Descripción del Problema

Crea un programa que utilice un ciclo `for` para iterar exactamente **7 veces** (representando los 7 días de la semana).
1. En cada iteración, solicitar la **temperatura del día** (puede tener decimales).
2. El programa debe ir sumando las temperaturas para calcular el **promedio semanal** al final.
3. Adentro del ciclo, debes utilizar la lógica necesaria para ir guardando la **temperatura máxima** y la **temperatura mínima** registradas.

### 📤 Salida Esperada

* **Ejemplo de Ejecución:**

```text
--- Registro Climático Semanal ---
Ingresa la temperatura del Día 1: 12.5
Ingresa la temperatura del Día 2: 9.0
Ingresa la temperatura del Día 3: 15.2
Ingresa la temperatura del Día 4: 8.5
Ingresa la temperatura del Día 5: 11.0
Ingresa la temperatura del Día 6: 14.3
Ingresa la temperatura del Día 7: 10.1

--- REPORTE FINAL ---
Temperatura Promedio: 11.51 °C
Temperatura MÁS ALTA: 15.2 °C
Temperatura MÁS BAJA: 8.5 °C
