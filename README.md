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

