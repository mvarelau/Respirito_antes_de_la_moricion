# Respirito_antes_de_la_moricion
La paz mental del reto #10
## Punto 1
Desarrollar un algoritmo que calcule el promedio de un arreglo de reales.
* Bueno, primero hice una función que hiciera la suma de todos lo npumeros que el ususario ingresa y que despues se agregan a una lista. Posteriormente defino una variable com la función de esa lista y después la divido en 5 (Tal vez no era necesario hacer todo eso por separado, pero a mi me encanta complicarme:)). Y por último le pido al código que imprima ese resultado
```python
def Suma(Lista):
  n=0
  for i in Lista:
    n+=i
  return(n)

print("Ingrese 5 números reales: ")
Lista=[]
a=float(input("a: "))
b=float(input("b: "))
c=float(input("c: "))
d=float(input("d: "))
e=float(input("e: "))
Lista.append(a)
Lista.append(b)
Lista.append(c)
Lista.append(d)
Lista.append(e)
Suma= Suma(Lista)
Promedio= Suma/5
print(f"Este es el promedio de los números que ingresó: {Promedio}")
```
Ver documento:[Punto1_10.ipynb](Punto1_10.ipynb)
## Punto 2
Desarrollar un algoritmo que calcule el producto punto de dos arreglos de números enteros (reales) de igual tamaño.
* El producto punto funciona asi:
![image](https://github.com/mvarelau/Respirito_antes_de_la_moricion/assets/141885396/701fc8d1-16cf-4a1c-9bf9-b3544b7204f6)
Teniendo en cuenta eso, hoce dos arreglos en los que el usuario puede ingresar lo números para cada uno de ellos. Después lo que hago es una lista donde se guarda la multiplicación de número uno a uno. Y posteriormente con un ciclo for, hago la suma de todos lo números de la lista de las multiplicdaciones y por último imroimo ese resultado.
```python
print("Ingrese 3 números reales: ")
Lista_1=[]
a=float(input("a: "))
e=float(input("e: "))
i=float(input("i: "))
Lista_1.append(a)
Lista_1.append(e)
Lista_1.append(i)
print("Ingrese 3 números reales: ")
Lista_2=[]
x=float(input("x: "))
y=float(input("y: "))
z=float(input("z: "))
Lista_2.append(x)
Lista_2.append(y)
Lista_2.append(z)
Lista_de_multiplicacion=[Lista_1[i]*Lista_2[i] for i in range(len(Lista_1))]
print(f"Esta es la lista de las multiplucaciones uno a uno: {Lista_de_multiplicacion}")
n=0
for i in Lista_de_multiplicacion:
  n+=i
print(f"El producto punto entre esos dos vectores es: {n}")
```
Ver documento: Ver documento:[Punto2_10.ipynb](Punto2_10.ipynb)
## Punto 3
Hacer un algoritmo que deje al final de un arreglo de números todos los ceros que aparezcan en dicho arreglo.
* En el principio es el mismo procedimiento que con los otros algoritmos, el usuario ingresa los números de el arreglo ( Yo se que no era necesario, pero así me parece más divertido).
En un ciclo for, si el número de la lista es igual a 0 entonces lo saca, y despues lo vuelve a insertar con un apend (cuadno se usa append siempre se agregan los números al final de la lista según entendí)
```python
print("Ingrese 4 números, dos de ellos que sean cero: ")
Lista_1=[]
a=float(input("a: "))
e=float(input("e: "))
i=float(input("i: "))
o=float(input("o: "))
Lista_1.append(a)
Lista_1.append(e)
Lista_1.append(i)
Lista_1.append(o)
Lista_Arregada=[]
for i in Lista_1:
  if i==0:
    Lista_1.remove(i)
    Lista_1.append(i)
print(Lista_1)
```
Ver documento: Ver documento:[Punto3_10.ipynb](Punto3_10.ipynb)
## Punto 3
Revisar que son los algoritmos de sorting, entender bubble-sort 
* Definitivamente fue el punto más largo de hacer de este reto.
- Para empezar hay que definir lo que es un algoritmo de sorting. Según entendí un algoritmo de soarting es un algoritmo que ordena lo elementos de una lista de menor a mayor, lo genial de estos algorirtmos es que cada uno lo hace de una manera distina, y algunos pueden ser más convenientes que otros teniendo en cuenta, la cantidad de elementos que tenga la lista y el almacenamiento con el que se disponga. Tambiénentendí que pueden estar clasificados según la cantidada de intercambios, el número de comparaciones, el uso de recursividad, y por estabilidad(si mal no entiendo esto depende de el órden).
- Bubble-sort es un algoritmo de ordenamiento que empieza comparando con el número anterior, si no cumple la condición se mueve al siguiente lugar y se compara con el siguiente  y así susesivamente hasta que cumpla con la condición.

