# Reto-9
1. De los retos anteriores selecione 3 funciones y escribalas en forma de lambdas.
```
#Funciones seleccionadas 
def valor_final_prestamo(c, i, n):
  a = c*(1+i)**n
  return a


def cant_carne_aves(N, M, K):
    carne_de_aves = (6*N+7*M+K)
    return carne_de_aves

def promedio(a, b, c, d, e):
    n = (a+b+c+d+e)/5
    return n 
#Funciones como lambdas
valor_ = lambda c,i,n : c(1+i)**n
ñ = valor_(1,2,3)
print(ñ)

carne_ = lambda N,M,K : 6*N+7*M+K
ññ = carne_(1,2,3)
print(ññ)

promedio_ = lambda a,b,c,d,e: (a+b+c+d+e)/5
ñññ = (1,2,3,4,5)
print(ñññ) 
```
2. De los retos anteriores selecione 3 funciones y escribalas con argumentos no definidos (*args).
```
#Funciones seleccionadas 
def valor_final_prestamo(c, i, n):
  a = c*(1+i)**n
  return a


def cant_carne_aves(N, M, K):
    carne_de_aves = (6*N+7*M+K)
    return carne_de_aves

def promedio(a, b, c, d, e):
    n = (a+b+c+d+e)/5
    return n 
# Escritas con *args. Los argumentos están almacenados en la tupla (*args)

def valor_(*args):
   if len(args)!=3 :
       print("Se requieren 3 parámetros")
   c,i,n = args
   a = c*(1+i)**n
   return a 



def cant_carne_aves(*args):
    if len(args) != 3: #En este caso probé esto y el codigo queda más completo, entonces lo repliqué en las otras 2 xd
        print ("Se requieren exactamente 3 argumentos: N, M y K")
    N, M, K = args
    carne_de_aves = 6 * N + 7 * M + K
    return carne_de_aves

def promedioo_ (*args):
    if len(args) != 5:
        print ("Se requieren 5 parámetros")
    a,b,c,d,e = args
    n = (a+b+c+d+e)/5
    return n 
```
3. Escriba una función recursiva para calcular la operación de la potencia.
```
n = int(input("Ingrese un numero para la base: "))
y = int(input("Ingrese un numero para el exponente: "))
def potenciaRecursiva(n,y):
    if y ==0: #Caso base
        return 1
    else:
        a = n* potenciaRecursiva(n,y-1) #Llamado a la funcion recursiva
    return a    
print("El resultado de {n} elevado a la {y} es",potenciaRecursiva(n,y))
```
5. Utilice la siguiente plantilla de code para contar el tiempo:
```
import time

start_time = time.time()
# instrucciones sobre las cuales se quiere medir tiempo de ejecución
end_time = time.time()

timer = end_time - start_time
print(timer)
```
Realice pruebas para calcular fibonacci con iteración o con recursión. Determine desde que número de la serie la diferencia de tiempo se vuelve significativa. Importante: Revisar este hil

```
import time
n = int(input("Ingrese un numero: "))
def fiboRecursivo(n):
    if n <= 1:
        return 1
    else:
        return fiboRecursivo(n - 1) + fiboRecursivo(n - 2) #Definiendo la función a utilizar


diferencia_sign = 10    #Aquí la diferencia va a estar en segundos, en mi caso creo que es a los 10 segundos 

for n in range(1, 1000): #Siguiendo las intrsucciones de uso adjuntadas en el repo de la clase
    start_time = time.time()
    serieFibo = fiboRecursivo(n) 
    end_time = time.time()

    timer = end_time - start_time
    print("n = {n}, Tiempo de ejecución: {timer} segundos")

    if timer > diferencia_sign: #En este momento se va a romper la iteración
        print("La diferencia de tiempo se volvió significativa en n = {n}")
        break
```

5. Crear cuenta en stackoverflow y adjuntar imagen en el repo
![image](https://github.com/Santi1019/Reto-9/assets/141860536/be170f8f-2230-4ab3-81ab-d06054378819)


6. Cosas de adultos....ir a linkedin y crear perfil...
- Adjunto link
https://www.linkedin.com/in/santiago-avendano-cely-745000297/ 
