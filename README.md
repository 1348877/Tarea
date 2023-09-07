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







