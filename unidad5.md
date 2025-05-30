
# 🧠 Evaluación de Conceptos de C y Arreglos

Este documento contiene un resumen con las respuestas correctas a un conjunto de preguntas teóricas sobre arreglos, estructuras, cadenas y funciones en lenguaje C.

---

## 1. Búsqueda en Arreglos

**Pregunta:**  
La búsqueda de un elemento en un arreglo consiste en:

**✅ Respuesta correcta:**  
`b. Recorrer el arreglo a fin de encontrar el valor buscado`

---

## 2. Definición de un Arreglo

**Pregunta:**  
Un arreglo es “un conjunto finito ordenado de elementos homogéneos”.

**✅ Significados:**  
- **Homogéneo:** Todos los elementos del arreglo son del mismo tipo.  
- **Ordenado:** Los elementos están dispuestos en un orden lógico (índice).  
- **Finito:** Hay un número específico de elementos en el arreglo.

---

## 3. Relaciones en la Búsqueda Binaria

- El **ordenamiento de un arreglo** → se realiza mediante un determinado criterio de ordenamiento.  
- El arreglo **debe estar ordenado** → para realizar la búsqueda binaria.  
- La **búsqueda binaria no se puede aplicar** → si el arreglo no está ordenado.

---

## 4. Ordenamiento de Cadenas

**Pregunta:**  
Una cadena no se puede ordenar aplicando cualquier método de ordenamiento que se utiliza para ordenar un arreglo.

**✅ Respuesta correcta:**  
`Falso`

---

## 5. Estructura o Registro

**Pregunta:**  
Una estructura o registro es una estructura de datos que agrupa variables que pueden tener tipos diferentes.

**✅ Respuesta correcta:**  
`Verdadero`

---

## 6. Ventajas de las Funciones

**Pregunta:**  
La o las ventajas de las funciones son:

**✅ Respuestas correctas:**  
- `a. Cuando cada módulo está bien probado se lo puede usar las veces que sea necesario sin volver a revisarlo.`  
- `b. El programa no es más simple de comprender ya que cada módulo se dedica a realizar una tarea en particular.`

---

## 7. Funciones y su Significado

| Función            | Significado                                                         |
|--------------------|---------------------------------------------------------------------|
| `islower(caracter)`| Verifica si un carácter es una letra minúscula                     |
| `strchr()`         | Localiza la primera instancia de un carácter dentro de un string   |
| `strcmp()`         | Compara una cadena con otra                                        |

---

## 8. Tipos de Funciones en C

**Pregunta:**  
En C las funciones pueden ser:

**✅ Respuesta correcta:**  
`a) Definidas por el usuario`

---

---

## 9. Tipos de Funciones en C

**Pregunta:**  
En C las funciones pueden ser:

**✅ Respuesta correcta:**  
`a) Definidas por el usuario`

---

## 10. Uso de la sentencia RETURN

**Pregunta:**  
La sentencia RETURN fuerza la salida inmediata del cuerpo de la función y se vuelve a la siguiente sentencia después de la llamada.

**✅ Respuesta correcta:**  
`Verdadero`

---

## 11. Proposición no asociada con arreglos

**Pregunta:**  
¿Qué proposición no está asociada con arreglos?

**✅ Respuesta correcta:**  
`c. Ninguna de las opciones`  
(Las opciones a y b son correctas para arreglos.)

---

## 12. Evaluación de condición en arreglo

**Código:**
```c
int numeros[] = {1, 3, 5, 7, 9};
int encontrado = 0;
for (int i = 0; i < 5; i++) {
    if (numeros[i] == 5) {
        encontrado = 1;
    }
}
```

**Pregunta:**  
¿Qué valor tendrá la variable `encontrado` si el número fue hallado?

**✅ Respuesta correcta:**  
`1`

---

## 13. Valor por defecto en un arreglo parcialmente inicializado

**Código:**
```c
int arreglo[3] = {7};
```

**Pregunta:**  
¿Qué valor tiene la posición `arreglo[1]`?

**✅ Respuesta correcta:**  
`0`

---

## 14. Función que modifica un arreglo

**Código:**
```c
void asignarValor(int arr[]) {
    arr[0] = 100;
}

int main() {
    int datos[5] = {0};
    asignarValor(datos);
    printf("%d\n", datos[0]);
    return 0;
}
```

**Pregunta:**  
¿Qué valor se imprime?

**✅ Respuesta correcta:**  
`100`

---

## 15. Multiplicación condicional de elementos de un arreglo

**Código:**
```c
int datos[] = {1, 2, 3, 4, 5};
for (int i = 0; i < 5; i++) {
    if (datos[i] % 2 == 0) {
        datos[i] = datos[i] * 10;
    }
}
printf("%d", datos[1]);
```

**Pregunta:**  
¿Qué valor se imprime?

**✅ Respuesta correcta:**  
`20` (porque `datos[1] = 2 * 10`)

---

---

## 16. Multiplicación condicional de elementos (continuación)

**Código:**
```c
int datos[] = {1, 2, 3, 4, 5};
for (int i = 0; i < 5; i++) {
    if (datos[i] % 2 == 0) {
        datos[i] = datos[i] * 10;
    }
}
printf("%d", datos[1]);
```

**✅ Respuesta correcta:**  
`20`

---

## 17. Función `void` con mensaje

**Código:**
```c
void saludar() {
    printf("Hola mundo\n");
    return;
}

int main() {
    saludar();
    return 0;
}
```

**Pregunta:**  
¿Qué hace el programa?

**✅ Respuesta correcta:**  
Imprime `Hola mundo`. No hay error porque aunque es `void`, el `return` sin valor es válido.

---

## 18. Duplicar elementos de un arreglo

**Código:**
```c
void duplicar(int v[], int n) {
    int i = 0;
    while (i < n) {
        v[i] = v[i] * 2;
        i++;
    }
}
```

**Entrada:**  
`{1, 3, 4}`

**✅ Resultado esperado del arreglo:**  
`2, 6, 8`

---

## 19. Recorrido de arreglo de estructuras

**Código:**
```c
struct Producto {
    char nombre[30];
    float precio;
    int stock;
};

struct Producto productos[3];
// Código para cargar datos omitido
for (int i = 0; i < 3; i++) {
    printf("%s - %.2f - %d\n", productos[i].nombre, productos[i].precio, productos[i].stock);
}
```

**✅ Respuesta correcta:**  
`Verdadero`

---

## 20. Buscar todas las posiciones donde aparece un número

**Código:**
```c
int main() {
    int numeros[5] = {3, 7, 9, 1, 9};
    int buscado = 9;
    for (int i = 0; i < 5; i++) {
        if (numeros[i] == buscado) {
            printf("Encontrado en %d\n", i);
        }
    }
}
```

**✅ Respuesta correcta:**  
Este código imprime todas las posiciones donde aparece el número `9`, incluso si se repite.

---

---

## 21. Código para imprimir todas las posiciones donde aparece un número

**Código original (con `break`):**
```c
int numeros[5] = {3, 7, 9, 1, 9};
int buscado = 9;
int encontrado = 0;
for (int i = 0; i < 5; i++) {
    if (numeros[i] == buscado) {
        printf("Encontrado en %d\n", i);
        encontrado = 1;
        break;
    }
}
if (!encontrado) {
    printf("No encontrado.\n");
}
```

**✅ Corrección para imprimir todas las posiciones donde aparece 9:**  
`Eliminar break; dentro del if`

---

## 22. Análisis de matriz

**Código:**
```c
int matriz[2][2];
matriz[0][0] = 1;
matriz[0][1] = 2;
matriz[1][0] = 3;
matriz[1][1] = 4;
```

**✅ Resultado correcto:**  
`b. 1 2 3 4`

---

## 23. Resultado de búsqueda

**Código:**
```c
int numeros[5] = {3, 7, 9, 1, 4};
int buscado = 9;
// búsqueda...
```

**✅ Resultado:**  
`a. Encontrado en la posición 2`

---

## 24. Impresión parcial del arreglo

**Código:**
```c
int valores[] = {3, 6, 9, 12, 15};
for (int i = 0; i < 3; i++) {
    printf("%d ", valores[i]);
}
```

**✅ Resultado:**  
`3 6 9`

---

## 25. Asignación en matriz bidimensional

**Código:**
```c
int mat[3][4];
mat[1][2] = 10;
```

**✅ Significado de la asignación:**  
Se está asignando el valor 10 en la **segunda fila** y **tercera columna**  
(Recordá que los índices comienzan en 0).

---

---

## 26. Función sumar dos números

**Código:**
```c
int sumar(int a, int b) {
    return a + b;
}

int main() {
    int resultado = sumar(3, 4);
    printf("Resultado: %d\n", resultado);
    return 0;
}
```

**✅ Resultado esperado:**  
`7`

---

## 27. Sumar los elementos de un arreglo

**Código:**
```c
int sumar(int arr[], int size) {
    int total = 0;
    for (int i = 0; i < size; i++) {
        total = total + arr[i];
    }
    return total;
}
```

**Entrada:**  
`sumar({1, 2, 3}, 3)`

**✅ Resultado esperado:**  
`6`

---

## 28. Cambiar valor del arreglo desde función

**Código:**
```c
void cambiar(int arr[]) {
    arr[0] = 100;
}

int main() {
    int nums[3] = {5, 10, 15};
    cambiar(nums);
    printf("%d\n", nums[0]);
    return 0;
}
```

**✅ Resultado esperado:**  
`Verdadero` (Se imprime `100`)

---

## 29. Insertar valor en posición específica del arreglo

**Código:**
```c
void insertarValor(int arr[], int pos, int valor) {
    arr[pos] = valor;
}

int main() {
    int numeros[5] = {1, 2, 3, 4, 5};
    insertarValor(numeros, 2, 99);
    printf("%d\n", numeros[2]);
    return 0;
}
```

**✅ Resultado esperado:**  
`d. 99`

---


---

## 30. Impresión de matriz 3x2

**Código:**
```c
void imprimir(int m[][2], int filas) {
    for (int i = 0; i < filas; i++) {
        for (int j = 0; j < 2; j++) {
            printf("%d ", m[i][j]);
        }
    }
}

int main() {
    int datos[3][2] = {{1, 2}, {3, 4}, {5, 6}};
    imprimir(datos, 3);
    return 0;
}
```

**✅ Resultado esperado:**  
`1 2 3 4 5 6`

---

## 31. Suma de cuadrados

**Código:**
```c
int cuadrado(int x) { return x * x; }

int sumaCuadrados(int a, int b) {
    return a + b;
}

int main() {
    int resultado = sumaCuadrados(cuadrado(2), cuadrado(4));
    printf("Resultado: %d\n", resultado);
    return 0;
}
```

**✅ Resultado esperado:**  
`20` (porque 2² + 4² = 4 + 16 = 20)

---

## 32. Comparación entre campos de estructuras

**Código:**
```c
if (p1.edad > p2.edad) {
    printf("%s es mayor que %s", p1.nombre, p2.nombre);
}
```

**✅ Afirmaciones correctas:**  
- `a. Se está comparando un campo específico de la estructura.`  
- `d. La comparación es válida si "edad" es un campo tipo int.`

---
