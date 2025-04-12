# Comparación de Métodos de Evaluación de Polinomios

Este programa en C++ evalúa polinomios utilizando dos métodos diferentes y compara su rendimiento:
  
- **Método Estándar:** Calcula el polinomio sumando cada término, donde se utiliza `std::pow` para elevar x a la potencia correspondiente.
- **Método de Horner:** Emplea el algoritmo de Horner, que reestructura el polinomio en forma anidada para reducir el número de operaciones costosas.

El programa genera, para cada grado de polinomio (de 10 a 1000, en incrementos de 10), coeficientes aleatorios y un valor aleatorio para x (excluyendo el cero). Luego mide, promediando 1000 repeticiones por grado, el tiempo de ejecución de cada método. Los resultados se almacenan en un archivo CSV denominado `resultados.csv`.

---

## Autora

**ALONDRA RODRIGUEZ ROBLES**

---

## Requisitos del Sistema

- **Compilador C++:**  
  Se recomienda utilizar *g++* versión 7.0 o superior, ya que es necesario contar con soporte para C++11 o versiones posteriores.
- **Plataforma:**  
  Este código es multiplataforma; funciona en Windows, Linux, macOS y otros sistemas compatibles con compiladores modernos de C++.

---

## Instrucciones de Compilación y Ejecución

### Compilación

1. Abre la terminal y ubícate en el directorio donde se encuentra el archivo fuente (por ejemplo, `main.cpp`).
2. Ejecuta el siguiente comando:

   ```bash
   g++ -O2 -std=c++11 main.cpp -o polinomios
