# Practica Auxiliatura 

[Entregar practica](#cabecera1) 

***
## Matrices
## Ejercicio Nº #1 Cuadrado magico
Escriba un programa que lea un número impar del teclado y genere una matriz cuadrada donde, sin repetir
ningún numero,la suma de las filas, columnas y diagonales da el mismo número. Por ejemplo en la matriz
siguiente la suma es 15.
|  |  |  |
|-|-|-|
|6|1|8|
|7|5|3|
|2|9|4|

***
## Ejercicios con cadenas
## Ejercicio Nº #1:  Buscando el Oro
### Descripcion 

En este programa debes buscar la primera palabra ORO en una cadena.
Luego imprimir la posición donde comienza y conde acaba.

Por ejemplo en la cadena "abcdefOrOefg" la palabra oro se encuentra posisición 6 hasta la 8.

### Entrada

La entrada consiste de una cadena en letras mayusculas y minusculas.

### Salida

Imprima en la salida la posición donde esta la palabra ORO, puede ser en mayusculas y minusculas indistintamente.
Sino existe la palabra imprima -1.
|     Ejemplo Entrada                                  |      Ejemplo Salida           |
|  --------------------------------------------------- |   --------------------------  |
|                   abcdefOrOefg                       |            6 8                |
|      NingunProblemaOrODeberiaResolverseOrOdosVeces   |            14 16              |


## Ejercicio Nº #2 : Cifrado Cesar
### Descripcion 
Escriba un programa que codifique mensajes de Cesar, Este cifrado lo utilizo Julio Cesar
 para comunicarse con sus generales.

Dada una constante K, cada letra del mensaje original se remplaza por una letra que esta
alfabeticamente K posiciones a la derecha, en forma circular si pasa la ultima letra del
 alfabeto.

Por ejemplo si K=5 debemos cambiar la letra **a** por **f** por  **b**  por  **g** , ... y **z** por **e**.

### Entrada 
La entrada consiste de varios casos de prueba. Cada caso de prueba comienza con un numero 
natural k > 0, suguido de una cadena 1<= |cadena| <=50 de solo letras minusculas. Existe
 un separador de palabras pero no un espacio. El separador puede ser una caracter que no
  sea una letra minúscula.

### Salida
Para cada caso de prueba escriba una linea con el texto cifrado en minúsculas, Remplace 
los guiones bajos por espacio. Deje los caracteres de separación de palabras sin cambio.

|     Ejemplo Entrada           |      Ejemplo Salida           |
|  ---------------------------  |   --------------------------  |
| 1   ingenieria_de_sistemas    |  JOHFOJFSJB EF TJTUFNBT       |
| 5   inteligencia_artificial   |  NSYJQNLJHNF FWYNKNHNFQ       |
Donde los numeros 1 y 5 del ejemplo son valores de K 


## Ejercicio Nº #3 : Jackiado
### Descripción
Le jackiaron su contraseña de Facebook a Botas, y publicaron en Infoamigos que es gay, Ahora debe crear una nueva contraseña y esta vez no debe ser tan obvia.
Se dice una contraseña es segura cuando tiene almenos una letra mayúscula, una minuscula, un número y un caracter especial. Ayuda a verificar si la nueva contraseña de Botas es segura o no.
### Entrada 
La entrada comienza con T casos de prueba (1<=T<=100000). Cada caso de preuba es una contraseña con maximo 30 caracteres (1<= |contraseña|<30), y que solo consta de minusculas, mayusculas, numeros y los caracteres especiales '@', punto '.', barra baja '_', menor '<', mayor '>' y guion '-'.

### Salida
Si la contraseña es segura, imprimir "Dale no te jackiaran esta vez." sin comillas. Caso contrario imprimir "No va dar Botas."
|     Ejemplo Entrada                                  |      Ejemplo Salida                        |
|  --------------------------------------------------- |   ---------------------------------------  |
|                   5                                  |                                            |
|      Botas123                                        |      No va dar Botas                       |
|      75803727                                        |      No va dar Botas                       |
|     B0t45_Rul35                                      |      Dale no te jackiaran esta vez         |
|      31-06-1996                                      |      No va dar Botas                       |
|      D0R4_l4_Expl0r4D0r4_I_<3_U                      |      Dale no te jackiaran esta vez         |

***
## Ejercicios con Pilas
## Ejercicio Nº #1
### ¿Cuál es la salida de este segmento de código, teniendo en cuenta que el tipo de dato de la pila es int?
    Pila p=new Pila();
    int x=4, y;
    p.insertar(x);
    System.out.println("\n"+p.cimaPila());
    y=p.quitar();
    p.insertar(32);
    p.insertar(p.quitar());
    do{
        System.out.println("\n"+p.quitar());
    }while(!p.pilaVacia());

## Ejercicio Nº #2
### Descripcion
 Escribir un programa en el que se manejen un total de n=5 pilas: P1, P2, P3, P4 y P5.  

### Entrada
La entrada de datos serán pares de enteros (i,j) tal que 1≤abs(i)≤n. De tal forma que el criterio de selección de pila será:
* Si i es positivo, debe insertarse el elemento j en la pila Pi. (Pila sub i)
* Si i es negativo, debe eliminarse el elemento j de la pila Pi.
* Si i es cero, fin del proceso de entrada. Los datos de entrada se introducen por teclado.

### Salida
Cuando termina el proceso el programa debe escribir el contenido de las n Pilas en pantalla(Ventana) o consola.

## Ejercicio Nº #3: Sombrero de la pila
### Descripcion
Se dice que una Pila dada es sombre de otra si todos los datos de la pila p aparecen en la otra en el mismo orden y ocupando las pisiciones más próximas a su tope.
* **Nota** Una pila vacía es sombrero de cualquier otra pila

![Con titulo](https://github.com/isaacaruquipa/PracticasAuxiliatura_2019/blob/master/SombreroPila.PNG "Sombreo de la pila")

### Entrada 
Como entrada de datos llenar la pila A y la pila B. (Los tipos de datos es a criterio).
### Salida
* Desplegar la pila A y la pila B
* Mostrar "Es sombrero de la pila B" si todos los datos ocupan posiciones mas proximas a su tope.
* Mostrar "No es sombreo de la pila B" cuando algun dato no ocupe las mismas posiciones proximas a su tope.

## Ejercicio Nº #4
### Descripcion
Crear una pila para almacenar datos de **N** Alumnos utilizando las siguiente clase:
    
     public class Alumno{
      private int codigo;
      private String nombre;
      private int nota;
      private char sexo;

      public Alumno(int codigo, String nombre, int nota){
        this.nombre=nombre;
        this.codigo=codigo;
        this.nota=nota;
      }
      public void setCodigo(int codigo){
        this.codigo=codigo;
      }
      public void getCodigo(){
        return this.codigo;
      }

      public void setNombre(String nombre){
        this.nombre=nombre;
      }
      public void getNombre(){
        return this.nombre;
      }

      public void setNota(int nota){
        this.nota=nota;
      }
      public void getNota(){
        return this.nota;
      }

      public void setSexo(char sexo){
        this.sexo=sexo;
      }
      public void getSexo(){
        return sexo;
      }
    }
### Entrada 
Registrar n alumnos en la pila implementada para almacenar Objetos de tipo alumno.

### Salida
* Desplegar(consola) codigo, nombre, nota del Alumno que tiene la nota mas alta.
* Desplegar codigo, nombre, nota del Alumno que tiene la nota mas baja.
* Desplegar La cantidad de aprobados.
* Desplegar la cantidad de reprobados.
* Desplegar el promedio de calificacion de todo los alumnos.
* Mostrar la cantidad de varones y cantidad mujeres.

***
## Ejercicios con Colas
## Ejercicio Nº #1:  Eliminando registros
### Descripción
Implementar una cola para registrar Datos de alumnos del anterior ejercicio.
* Implementar Un metodo para realizar una busqueda de alumn@s
* Implementar un metodo para ** Eliminar** de la cola alumn@s  cuyo(s) nombre(s) inicie(n)  con la **Letra inicial que es pedido del usuario.**
### Entrada
Registrar **N** alumnos en la cola.
### Salida
* Mostrar todos los alumnos de la registrados en la cola.
* Realizar la busqueda del alumn@(s) y desplegar todos los campos.
* Eliminar Alumn@(s) de la cola y mostrar todos los alumn@s registrados en la cola.
***
***
## Formato de cabecera  de la practica.
![Con titulo](FormatoCabecera.png "FormatoCabecera")


## Adjuntar en documento pdf lo siguiente.
1. Adicionar numero  de ejercicio y descripcion del ejercicio.
2. Codigo fuente.
3. Capturas de pantalla de corrida del programa.
## La entrega del documento debe ser en digital  con las inicales de los apellidos, nombre y CI **AP_AM_NOMBRE_CI.pdf**.
### Ejemplo mi nombre y apellido es: Isaac Santos Aruquipa Machaca
## **A_M_ISAAC_9257004.pdf**.
***
### Entregar practica 
{#cabecera1}
### Enviar por correo [Isaac Aruquipa ](emailto:isaac2019aruquipa@gmail.com "Correo electronico")
### Enviar por whatsapp [Isaac Aruquipa ]("")









