Ejercicio 1 
#include <iostream>

using namespace std;

// Función para calcular el subsidio
double calcularSubsidio(int numHijos, int edadMadre, int numHijosEscolar) {
    double monto = 0.0;
    
    // Verificar el número de hijos
    if (numHijos <= 2) {
        monto = 70.0;
    } else if (numHijos <= 5) {
        monto = 90.0;
    } else {
        monto = 120.0;
    }
    
    // Calcular el monto adicional por hijos en edad escolar
    monto += numHijosEscolar * 10.0;
    
    // Verificar si la madre es viuda
    if (edadMadre == -1) {
        monto += 20.0;
    }
    
    return monto;
}

Ejercicio 2 
int main() {
    int numHijos, edadMadre, numHijosEscolar;
    
    cout << "Ingrese el número de hijos: ";
    cin >> numHijos;
    
    cout << "Ingrese la edad de la madre (-1 si es viuda): ";
    cin >> edadMadre;
    
    cout << "Ingrese el número de hijos en edad escolar (entre 6 y 18 años): ";
    cin >> numHijosEscolar;
    
    double subsidio = calcularSubsidio(numHijos, edadMadre, numHijosEscolar);
    
    cout << "El monto mensual que recibirá la familia es: Q" << subsidio << endl;
    
    return 0;
}

#include <iostream>
#include <vector>
#include <cstdlib>
#include <ctime>

using namespace std;

// Función para llenar un vector con valores aleatorios entre 1 y 100
void llenarVector(vector<int>& vec, int longitud) {
    vec.clear(); // Limpiar el vector si ya tenía elementos
    
    for (int i = 0; i < longitud; i++) {
        vec.push_back(rand() % 100 + 1); // Generar un valor aleatorio entre 1 y 100
    }
}

// Función para calcular la suma de los elementos de un vector
int sumarVector(const vector<int>& vec) {
    int suma = 0;
    for (int elemento : vec) {
        suma += elemento;
    }
    return suma;
}

int main() {
    srand(time(0)); // Inicializar la semilla para los números aleatorios
    
    int longitud;
    vector<int> vectorA, vectorB;
    
    cout << "Ingrese la longitud de los vectores: ";
    cin >> longitud;
    
    llenarVector(vectorA, longitud);
    llenarVector(vectorB, longitud);
    
    int sumaA = sumarVector(vectorA);
    int sumaB = sumarVector(vectorB);
    
    cout << "Vector A: ";
    for (int elemento : vectorA) {
        cout << elemento << " ";
    }
    cout << endl;
    
    cout << "Vector B: ";
    for (int elemento : vectorB) {
        cout << elemento << " ";
    }
    cout << endl;
    
    cout << "Suma de los elementos del vector A: " << sumaA << endl;
    cout << "Suma de los elementos del vector B: " << sumaB << endl;
    
    if (sumaA == sumaB) {
        cout << "Los vectores son iguales." << endl;
    } else if (sumaA < sumaB) {
        cout << "El vector A es menor que el vector B." << endl;
    } else {
        cout << "El vector B es menor que el vector A." << endl;
    }
    
    return 0;
}

Ejercicio 3

#include <iostream>
#include <vector>
#include <algorithm>

using namespace std;

int main() {
    int numDatos;

    // Preguntar al usuario cuántos datos serán ingresados
    cout << "Ingrese la cantidad de datos: ";
    cin >> numDatos;

    // Verificar que el número de datos sea válido
    if (numDatos <= 0) {
        cout << "La cantidad de datos debe ser mayor que cero." << endl;
        return 1; // Salir del programa con un código de error
    }

    // Declarar un vector para almacenar los datos
    vector<double> datos;

    // Solicitar al usuario ingresar los datos uno por uno
    for (int i = 0; i < numDatos; i++) {
        double dato;
        cout << "Ingrese el dato #" << (i + 1) << ": ";
        cin >> dato;
        datos.push_back(dato);
    }

    // Calcular el rango de los datos
    double minDato = *min_element(datos.begin(), datos.end());
    double maxDato = *max_element(datos.begin(), datos.end());
    double rango = maxDato - minDato;

    // Mostrar el resultado
    cout << "El rango de los datos es: " << rango << endl;

    return 0;
}

Ejercicio 4

#include <iostream>

using namespace std;

int main() {
    int lado;

    // Solicitar al usuario ingresar el lado del cuadrado
    cout << "Ingrese el lado del cuadrado: ";
    cin >> lado;

    // Verificar que el lado sea válido (mayor o igual a 2)
    if (lado < 2) {
        cout << "El lado del cuadrado debe ser mayor o igual a 2." << endl;
        return 1; // Salir del programa con un código de error
    }

    // Dibujar el cuadrado
    for (int i = 1; i <= lado; i++) {
        for (int j = 1; j <= lado; j++) {
            if (i == 1 || i == lado || j == 1 || j == lado) {
                cout << "* ";
            } else {
                cout << "  "; // Espacio en blanco para el interior del cuadrado
            }
        }
        cout << endl;
    }

    return 0;
}

Python 
Ejercicio 1
def calcularSubsidio(num_hijos, edad_madre, num_hijos_escolar):
    monto = 0.0
    
    # Verificar el número de hijos
    if num_hijos <= 2:
        monto = 70.0
    elif num_hijos <= 5:
        monto = 90.0
    else:
        monto = 120.0
    
    # Calcular el monto adicional por hijos en edad escolar
    monto += num_hijos_escolar * 10.0
    
    # Verificar si la madre es viuda
    if edad_madre == -1:
        monto += 20.0
    
    return monto

# Solicitar entrada de usuario
num_hijos = int(input("Ingrese el número de hijos: "))
edad_madre = int(input("Ingrese la edad de la madre (-1 si es viuda): "))
num_hijos_escolar = int(input("Ingrese el número de hijos en edad escolar (entre 6 y 18 años): "))

# Calcular el subsidio utilizando la función
subsidio = calcularSubsidio(num_hijos, edad_madre, num_hijos_escolar)

# Mostrar el monto mensual que recibirá la familia
print(f"El monto mensual que recibirá la familia es: Q{subsidio:.2f}")

Ejercicio 2 

import random

# Función para llenar un vector con valores aleatorios entre 1 y 100
def llenar_vector(longitud):
    return [random.randint(1, 100) for _ in range(longitud)]

# Función para calcular la suma de los elementos de un vector
def sumar_vector(vector):
    return sum(vector)

# Solicitar al usuario la longitud de los vectores
longitud = int(input("Ingrese la longitud de los vectores: "))

# Verificar que la longitud sea válida (mayor que 0)
if longitud <= 0:
    print("La longitud de los vectores debe ser mayor que 0.")
else:
    # Llenar los vectores con valores aleatorios
    vectorA = llenar_vector(longitud)
    vectorB = llenar_vector(longitud)

    # Calcular las sumas de los vectores
    sumaA = sumar_vector(vectorA)
    sumaB = sumar_vector(vectorB)

    # Comparar las sumas y determinar los escenarios
    if sumaA == sumaB:
        print("Los vectores son iguales en cuanto a la suma.")
    elif sumaA < sumaB:
        print("El vector A es menor que el vector B en cuanto a la suma.")
    else:
        print("El vector B es menor que el vector A en cuanto a la suma.")

    # Mostrar los vectores y sus sumas (opcional)
    print("Vector A:", vectorA)
    print("Vector B:", vectorB)
    print("Suma del vector A:", sumaA)
    print("Suma del vector B:", sumaB)

Ejercicio 3 
# Función para calcular el rango de un conjunto de datos
def calcular_rango(datos):
    if len(datos) == 0:
        return None
    
    min_dato = min(datos)
    max_dato = max(datos)
    rango = max_dato - min_dato
    return rango

# Solicitar al usuario la cantidad de datos
num_datos = int(input("Ingrese la cantidad de datos: "))

# Verificar que la cantidad de datos sea válida
if num_datos <= 0:
    print("La cantidad de datos debe ser mayor que cero.")
else:
    datos = []

    # Solicitar al usuario ingresar los datos uno por uno
    for i in range(num_datos):
        dato = float(input(f"Ingrese el dato #{i + 1}: "))
        datos.append(dato)

    # Calcular el rango de los datos utilizando la función
    rango = calcular_rango(datos)

    # Mostrar el resultado
    if rango is not None:
        print(f"El rango de los datos es: {rango:.2f}")
    else:
        print("No se ingresaron datos válidos.")

Ejercicio 4 

# Solicitar al usuario ingresar el lado del cuadrado
lado = int(input("Ingrese el lado del cuadrado: "))

# Verificar que el lado sea válido (mayor o igual a 2)
if lado < 2:
    print("El lado del cuadrado debe ser mayor o igual a 2.")
else:
    # Dibujar el cuadrado
    for i in range(lado):
        if i == 0 or i == lado - 1:
            print("* " * lado)  # Dibujar la primera y última fila con asteriscos
        else:
            print("*" + " " * (lado - 2) + " *")  # Dibujar las filas intermedias con espacios en blanco en el medio

