# Ejercicios_Grupo5Tarea4

````markdown
# API-Ciclos-Java

## Integración de ciclos y controles de datos

Repositorio correspondiente a la práctica de programación en Java sobre
estructuras de repetición, validación de datos, contadores, acumuladores,
series numéricas y ciclos anidados.

---

## 👥 Integrantes

- Sandra Alulema
- Anthony Armas
- Joselyn Guaman
- Valentina Ortiz
- Andrés Vayas

**Grupo 5**

---

## 🎯 Objetivo

Desarrollar programas en Java utilizando estructuras de repetición y
control de datos, aplicando ciclos `for`, `while` y `do-while`, además
de validaciones, contadores, acumuladores y ciclos anidados para resolver
diferentes problemas de programación.

---

## 📝 Descripción de los ejercicios

### Ejercicio 1: Control de calificaciones

El programa permite ingresar el número de estudiantes y posteriormente
registrar la calificación de cada estudiante.

El sistema realiza las siguientes operaciones:

- Valida que el número de estudiantes sea mayor que cero.
- Solicita las calificaciones de cada estudiante.
- Valida que las calificaciones estén entre 0 y 10.
- Determina si cada estudiante está aprobado o reprobado.
- Cuenta la cantidad de estudiantes aprobados.
- Cuenta la cantidad de estudiantes reprobados.
- Calcula la suma de todas las calificaciones.
- Calcula el promedio general.
- Determina la calificación más alta.
- Determina la calificación más baja.

### Ejercicio 2: Ciclos anidados

Se utiliza un ciclo `for` dentro de otro ciclo `for` para representar
filas y columnas.

Ejemplo:

```text
* * * *
* * * *
* * * *
````

El ciclo exterior controla las filas y el ciclo interior controla las
columnas.

---

## 🔧 Estructuras utilizadas

Durante los ejercicios se utilizaron las siguientes estructuras:

### Ciclo `for`

Se utiliza cuando conocemos previamente la cantidad de repeticiones.

```java
for (int i = 1; i <= n; i++) {
    // instrucciones
}
```

### Ciclo `while`

Se utiliza principalmente para realizar validaciones mientras una
condición sea verdadera.

```java
while (n <= 0) {
    // solicitar nuevamente el dato
}
```

### Ciclo `do-while`

Permite ejecutar las instrucciones al menos una vez y repetirlas
mientras se cumpla una condición.

```java
do {
    // instrucciones
} while (condicion);
```

### Condicional `if-else`

Permite tomar decisiones dependiendo de una condición.

```java
if (nota >= 7) {
    aprobados++;
} else {
    reprobados++;
}
```

### Contadores

Permiten contabilizar elementos.

```java
aprobados++;
reprobados++;
```

### Acumuladores

Permiten sumar o acumular valores.

```java
suma += nota;
```

### Ciclos anidados

Consisten en colocar un ciclo dentro de otro.

```java
for (int fila = 1; fila <= 3; fila++) {

    for (int columna = 1; columna <= 4; columna++) {
        System.out.print("* ");
    }

    System.out.println();
}
```

---

## ▶️ Instrucciones de ejecución

### Requisitos

Para ejecutar los programas se necesita:

* Java JDK instalado.
* Un editor de código como IntelliJ IDEA, NetBeans, Eclipse o Visual Studio Code.
* Git instalado para trabajar con el repositorio.

### Ejecución

1. Clonar el repositorio:

```bash
git clone URL_DEL_REPOSITORIO
```

2. Ingresar a la carpeta del proyecto:

```bash
cd API-Ciclos-Java
```

3. Abrir el proyecto en el IDE.

4. Seleccionar el archivo `.java` que se desea ejecutar.

5. Ejecutar el programa.

6. Ingresar los datos solicitados por consola.

---

## 🧪 Casos de prueba

### Caso de prueba 1: Datos normales

**Entrada:**

```text
Número de estudiantes: 5

Calificaciones:
8
6
10
7
5
```

**Resultado esperado:**

```text
Número de estudiantes: 5
Suma de calificaciones: 36.00
Promedio general: 7.20
Cantidad de aprobados: 3
Cantidad de reprobados: 2
Nota más alta: 10.00
Nota más baja: 5.00
```

---

### Caso de prueba 2: Número de estudiantes inválido

**Entrada:**

```text
Número de estudiantes: -2
Número de estudiantes: 0
Número de estudiantes: 3
```

El programa debe rechazar los valores `-2` y `0` y solicitar
nuevamente el número hasta recibir un valor mayor que cero.

---

### Caso de prueba 3: Calificación fuera del rango

**Entrada:**

```text
Número de estudiantes: 3

Calificación:
8
15
7
```

El valor `15` debe ser rechazado porque las calificaciones permitidas
están entre `0` y `10`.

El programa debe solicitar nuevamente la calificación.

---

### Caso de prueba 4: Todos aprobados

**Entrada:**

```text
Número de estudiantes: 4

Calificaciones:
7
8
9
10
```

**Resultado esperado:**

```text
Promedio general: 8.50
Aprobados: 4
Reprobados: 0
Nota más alta: 10.00
Nota más baja: 7.00
```

---

### Caso de prueba 5: Todos reprobados

**Entrada:**

```text
Número de estudiantes: 4

Calificaciones:
2
4
5
6
```

**Resultado esperado:**

```text
Promedio general: 4.25
Aprobados: 0
Reprobados: 4
Nota más alta: 6.00
Nota más baja: 2.00
```

---

## 📸 Capturas o evidencias

En esta sección se deben colocar las capturas de pantalla que demuestren
la ejecución de los programas.

### Evidencia 1: Código fuente

Captura del código Java utilizado para resolver los ejercicios.

### Evidencia 2: Ejecución del programa

Captura de la consola mostrando los datos ingresados y los resultados
obtenidos.

### Evidencia 3: Pruebas de validación

Captura donde se observe el ingreso de datos incorrectos y el mensaje
de error correspondiente.

### Evidencia 4: Prueba de ciclos anidados

Captura de la ejecución del programa que muestra las filas y columnas
generadas mediante ciclos `for` anidados.

> Las imágenes pueden colocarse en una carpeta llamada `evidencias/`.

Ejemplo:

```text
evidencias/
├── ejecucion-control-calificaciones.png
├── validacion-datos.png
├── ciclos-anidados.png
└── prueba-escritorio.png
```

---

## 📊 Prueba de escritorio

Se realizaron pruebas de escritorio para verificar el funcionamiento
de los contadores, acumuladores, validaciones y condiciones.

Ejemplo:

| Estudiante | Nota | Suma | Aprobados | Reprobados | Nota alta | Nota baja |
| ---------- | ---- | ---- | --------- | ---------- | --------- | --------- |
| 1          | 8    | 8    | 1         | 0          | 8         | 8         |
| 2          | 6    | 14   | 1         | 1          | 8         | 6         |
| 3          | 10   | 24   | 2         | 1          | 10        | 6         |
| 4          | 7    | 31   | 3         | 1          | 10        | 6         |
| 5          | 5    | 36   | 3         | 2          | 10        | 5         |

---

## 📌 Conclusiones

* Los ciclos de repetición permiten ejecutar instrucciones varias veces
  de manera eficiente y organizada.
* El ciclo `for` resulta útil cuando se conoce el número de repeticiones,
  mientras que `while` y `do-while` permiten trabajar con condiciones
  y validaciones.
* Los contadores permiten llevar un registro de cantidades y los
  acumuladores permiten obtener sumas o resultados acumulados.
* La validación de datos permite evitar que el programa procese valores
  incorrectos.
* Los ciclos anidados permiten trabajar con estructuras organizadas
  en filas y columnas.
* La integración de ciclos, condiciones, validaciones, contadores y
  acumuladores permite desarrollar programas más completos y funcionales.

---

## 📚 Tecnologías utilizadas

* Java
* Git
* GitHub
* Visual Studio Code / IDE de Java

---

## 👨‍💻 Proyecto académico

**Asignatura:** Programación
**Tema:** Integración de ciclos y controles de datos
**Lenguaje:** Java
**Grupo:** 5

````

