# 🚀 Proyecto Integrador: Panel de Servidor Cloud (Uso de Funciones)

**Temas a practicar:** Creación e invocación de funciones (métodos), parámetros, valores de retorno, integrados con `do-while`, `for`, `switch` y condicionales.
**Contexto:** Gestión de infraestructura tecnológica y servidores web.

Al desarrollar software real, no podemos escribir todo el código de corrido. Debemos dividir los problemas grandes en piezas más pequeñas y reutilizables llamadas **funciones** (o métodos en Java).

### 📝 Descripción del Problema

Eres el administrador de sistemas de una empresa de alojamiento web (hosting). Necesitas crear un panel de control interactivo en consola que permita monitorear el estado de los servidores. 

Para mantener el código limpio y organizado, el programa principal (`main`) será solo el "director de la orquesta". La lógica pesada y los cálculos deben realizarse en **funciones personalizadas** que tú mismo vas a declarar.

### 🛠️ Funciones a Desarrollar (Fuera del `main`)

Debes programar los siguientes métodos estáticos (`public static`):

1. **`mostrarMenu()`**: Función `void` (sin valor de retorno). Su única tarea es imprimir en pantalla el menú de opciones. No recibe parámetros.
2. **`calcularConsumo(int usuarios, double megasPorUsuario)`**: Función que recibe dos parámetros, los multiplica y retorna el total de megas consumidos (tipo `double`).
3. **`evaluarSalud(double temperatura)`**: Función que recibe la temperatura del CPU y retorna un `String` con el diagnóstico:
   * Si es menor a 60, retorna `"Óptimo"`.
   * Si está entre 60 y 85 (inclusive), retorna `"Advertencia: Calor elevado"`.
   * Si es mayor a 85, retorna `"PELIGRO: Apagado térmico inminente"`.

### 📋 Flujo del Programa Principal (`main`)

1. Utiliza un ciclo `do-while` para mantener el panel activo.
2. Adentro del ciclo, **invoca tu función** `mostrarMenu()`.
3. Lee la opción del usuario y usa una estructura `switch`:
   * **Opción 1 (Calcular Tráfico):** Pide la cantidad de usuarios conectados y los megas por usuario. **Llama a la función** `calcularConsumo()` pasándole esos datos y muestra el resultado en pantalla.
   * **Opción 2 (Diagnóstico de Granja):** Pide al usuario cuántos servidores físicos quiere analizar. Usa un ciclo `for` que gire esa cantidad de veces. Por cada vuelta, pide la temperatura del servidor e **invoca a la función** `evaluarSalud()`, imprimiendo el texto que esta te devuelva.
   * **Opción 3 (Salir):** Termina la ejecución del sistema.
   * **Default:** Imprime un mensaje de error si elige una opción inexistente.

### 📤 Salida Esperada (Ejemplo de Ejecución)

```text
--- PANEL DE CONTROL CLOUD ---
1. Calcular Tráfico de Red
2. Diagnóstico de Granja de Servidores
3. Salir del Panel
Elige una opción: 1

Usuarios activos: 150
Megas promedio por usuario: 2.5
>> Consumo total de red: 375.0 MB.

--- PANEL DE CONTROL CLOUD ---
1. Calcular Tráfico de Red
2. Diagnóstico de Granja de Servidores
3. Salir del Panel
Elige una opción: 2

¿Cuántos servidores vas a analizar?: 3
Temperatura Servidor 1: 55.5
>> Estado: Óptimo
Temperatura Servidor 2: 78.0
>> Estado: Advertencia: Calor elevado
Temperatura Servidor 3: 92.5
>> Estado: PELIGRO: Apagado térmico inminente

--- PANEL DE CONTROL CLOUD ---
...
Elige una opción: 3
>> Cerrando conexión con el servidor.
