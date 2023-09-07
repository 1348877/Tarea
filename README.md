ejercicio 1

# Definir una función que recibe la edad como parámetro
def verificar_edad(edad):
  # Comparar la edad con el valor 18
  if edad >= 18:
    # Si la edad es mayor o igual a 18, imprimir "Mayor de edad"
    print("Mayor de edad")
  else:
    # Si la edad es menor que 18, imprimir "Menor de edad"
    print("Menor de edad")

# Solicitar al usuario que ingrese su edad
edad = int(input("Ingrese su edad: "))

# Llamar a la función con la edad ingresada
verificar_edad(edad)




 ejercicio 2

# Definir una función que recibe dos números como parámetros
def verificar_divisibilidad(a, b):
  # Verificar si el segundo número es cero
  if b == 0:
    # Si el segundo número es cero, imprimir "No se puede dividir por cero"
    print("No se puede dividir por cero")
  else:
    # Si el segundo número no es cero, calcular el resto de la división
    resto = a % b
    # Comparar el resto con el valor cero
    if resto == 0:
      # Si el resto es cero, imprimir "Los números son divisibles"
      print("Los números son divisibles")
    else:
      # Si el resto no es cero, imprimir "Los números no son divisibles"
      print("Los números no son divisibles")

# Solicitar al usuario que ingrese dos números
a = int(input("Ingrese el primer número: "))
b = int(input("Ingrese el segundo número: "))

# Llamar a la función con los dos números ingresados
verificar_divisibilidad(a, b)



 ejercicio 3


# Definir una función que recibe un número como parámetro
def verificar_paridad(n):
  # Calcular el resto de la división del número entre 2
  resto = n % 2
  # Comparar el resto con el valor cero
  if resto == 0:
    # Si el resto es cero, imprimir "El número es par"
    print("El número es par")
  else:
    # Si el resto no es cero, imprimir "El número es impar"
    print("El número es impar")

# Solicitar al usuario que ingrese un número
n = int(input("Ingrese un número: "))

# Llamar a la función con el número ingresado
verificar_paridad(n)


ejercicio 4


# Definir una función que recibe el año como parámetro
def verificar_bisiesto(año):
  # Verificar si el año es divisible por 4
  if año % 4 == 0:
    # Si el año es divisible por 4, verificar si es divisible por 100
    if año % 100 == 0:
      # Si el año es divisible por 100, verificar si es divisible por 400
      if año % 400 == 0:
        # Si el año es divisible por 400, imprimir "El año es bisiesto"
        print("El año es bisiesto")
      else:
        # Si el año no es divisible por 400, imprimir "El año no es bisiesto"
        print("El año no es bisiesto")
    else:
      # Si el año no es divisible por 100, imprimir "El año es bisiesto"
      print("El año es bisiesto")
  else:
    # Si el año no es divisible por 4, imprimir "El año no es bisiesto"
    print("El año no es bisiesto")

# Solicitar al usuario que ingrese el año
año = int(input("Ingrese el año: "))

# Llamar a la función con el año ingresado
verificar_bisiesto(año)


 ejercicio 5 

# Definir una función que recibe 4 notas como parámetros
def calcular_promedio(nota1, nota2, nota3, nota4):
  # Sumar las 4 notas y dividir por 4 para obtener el promedio
  promedio = (nota1 + nota2 + nota3 + nota4) / 4
  # Redondear el promedio al entero más cercano
  promedio_redondeado = round(promedio)
  # Verificar si el promedio redondeado es mayor o igual a 11
  if promedio_redondeado >= 11:
    # Si el promedio redondeado es mayor o igual a 11, imprimir "Aprobado"
    estado = "Aprobado"
  else:
    # Si el promedio redondeado es menor que 11, imprimir "Desaprobado"
    estado = "Desaprobado"
  # Imprimir el promedio, el promedio redondeado y el estado
  print(f"El promedio es {promedio}")
  print(f"El promedio redondeado es {promedio_redondeado}")
  print(f"El alumno está {estado}")

# Solicitar al usuario que ingrese las 4 notas
nota1 = float(input("Ingrese la primera nota: "))
nota2 = float(input("Ingrese la segunda nota: "))
nota3 = float(input("Ingrese la tercera nota: "))
nota4 = float(input("Ingrese la cuarta nota: "))

# Llamar a la función con las 4 notas ingresadas
calcular_promedio(nota1, nota2, nota3, nota4)


ejercicio 6 

# Definir una función que recibe 3 números enteros como parámetros
def determinar_mayor_menor(a, b, c):
  # Inicializar el mayor y el menor con el primer número
  mayor = a
  menor = a
  # Comparar el segundo número con el mayor y el menor
  if b > mayor:
    # Si el segundo número es mayor que el mayor, actualizar el mayor
    mayor = b
  elif b < menor:
    # Si el segundo número es menor que el menor, actualizar el menor
    menor = b
  # Comparar el tercer número con el mayor y el menor
  if c > mayor:
    # Si el tercer número es mayor que el mayor, actualizar el mayor
    mayor = c
  elif c < menor:
    # Si el tercer número es menor que el menor, actualizar el menor
    menor = c
  # Imprimir en pantalla el mayor y el menor
  print(f"El número mayor es {mayor}")
  print(f"El número menor es {menor}")

# Solicitar al usuario que ingrese los 3 números enteros
a = int(input("Ingrese el primer número: "))
b = int(input("Ingrese el segundo número: "))
c = int(input("Ingrese el tercer número: "))

# Llamar a la función con los 3 números ingresados
determinar_mayor_menor(a, b, c)


ejercicio 7

# Definir una función que recibe 3 números enteros como parámetros
def ordenar_numeros(a, b, c):
  # Crear una lista vacía para almacenar los números ordenados
  lista_ordenada = []
  # Encontrar el número menor entre los 3 números
  menor = min(a, b, c)
  # Agregar el número menor a la lista ordenada
  lista_ordenada.append(menor)
  # Encontrar el número mayor entre los 3 números
  mayor = max(a, b, c)
  # Encontrar el número medio entre los 3 números
  medio = a + b + c - menor - mayor
  # Agregar el número medio a la lista ordenada
  lista_ordenada.append(medio)
  # Agregar el número mayor a la lista ordenada
  lista_ordenada.append(mayor)
  # Imprimir en pantalla la lista ordenada
  print(f"Los números ordenados de menor a mayor son: {lista_ordenada}")

# Solicitar al usuario que ingrese los 3 números enteros
a = int(input("Ingrese el primer número: "))
b = int(input("Ingrese el segundo número: "))
c = int(input("Ingrese el tercer número: "))

# Llamar a la función con los 3 números ingresados
ordenar_numeros(a, b, c)



 ejercicio 8

# Definir una función que recibe 3 números enteros como parámetros
def ordenar_numeros(a, b, c):
  # Crear una lista vacía para almacenar los números ordenados
  lista_ordenada = []
  # Encontrar el número mayor entre los 3 números
  mayor = max(a, b, c)
  # Agregar el número mayor a la lista ordenada
  lista_ordenada.append(mayor)
  # Encontrar el número menor entre los 3 números
  menor = min(a, b, c)
  # Encontrar el número medio entre los 3 números
  medio = a + b + c - menor - mayor
  # Agregar el número medio a la lista ordenada
  lista_ordenada.append(medio)
  # Agregar el número menor a la lista ordenada
  lista_ordenada.append(menor)
  # Imprimir en pantalla la lista ordenada
  print(f"Los números ordenados de mayor a menor son: {lista_ordenada}")

# Solicitar al usuario que ingrese los 3 números enteros
a = int(input("Ingrese el primer número: "))
b = int(input("Ingrese el segundo número: "))
c = int(input("Ingrese el tercer número: "))

# Llamar a la función con los 3 números ingresados
ordenar_numeros(a, b, c)


ejercicio 9

# Definir las variables usuario y contraseña con los valores deseados
usuario = "admin"
contraseña = "1234"

# Solicitar al usuario que ingrese su usuario y contraseña
usuario_ingresado = input("Ingrese su usuario: ")
contraseña_ingresada = input("Ingrese su contraseña: ")

# Comparar el usuario y la contraseña ingresados con las variables
if usuario_ingresado == usuario and contraseña_ingresada == contraseña:
  # Si el usuario y la contraseña son correctos, imprimir "Puede ingresar al sistema"
  print("Puede ingresar al sistema")
else:
  # Si el usuario o la contraseña son incorrectos, imprimir "No puede ingresar al sistema"
  print("No puede ingresar al sistema")



















