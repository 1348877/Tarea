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
    # Comparar el resto con el valor c



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







