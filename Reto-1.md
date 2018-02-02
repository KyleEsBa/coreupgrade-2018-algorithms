## 1. ¿Cual es la complejidad de tiempo de la función example()?

```c++
int example(int n)
{
  int count = 0;
  for (int i = n; i > 0; i /= 2)
     for (int j = 0; j < i; j++)
        count += 1;
  return count;
}
```
##Respuesta: O(log(n))
##Sustentación: El ciclo exterior es de complejidad O(log(n)) y el ciclo interior es de complejidad O(1), este ultimo aceptado en la complejidad del ciclo externo.
## 2. ¿Cual es la complejidad de tiempo de la función example2()?

```c++
void example2(int n, int arr[])
{
    int i = 0, j = 0;
    for(; i < n; ++i)
        while(j < n && arr[i] < arr[j])
            j++;
}
```
##Respuesta: O(n)
##Sustentación: El ciclo 'for' es de complejidad O(n) pues el incremento ++i cumple la misma función que i+=1; el ciclo 'while' es de complejidad O(1), esta ultima aceptada en la complejidad O(n).
## 3. ¿Cuál es la mejor complejidad de tiempo de bubbleSort?
##Respuesta: O(1)
##Sustentación: El mejor de los casos para este algoritmo, seria encontrar el elemento buscado en la primera posición del arreglo. Por lo tanto la mejor complejidad seria O(1).

