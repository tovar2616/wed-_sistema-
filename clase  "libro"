def es_anagrama(palabra1, palabra2):
    if len(palabra1) != len(palabra2):
        return False
    return sorted(palabra1.lower()) == sorted(palabra2.lower())

def invertir_cadena(cadena):
    return cadena[::-1]

def fibonacci(n):
    if n <= 0:
        return 0
    elif n == 1:
        return 1
    else:
        return fibonacci(n-1) + fibonacci(n-2)

def eliminar_duplicados(lista):
    return list(set(lista))

def es_palindromo(cadena):
    cadena = cadena.lower().replace(" ", "")
    return cadena == cadena[::-1]

def contar_palabras(texto):
    palabras = texto.lower().split()
    conteo = {}
    for palabra in palabras:
        if palabra in conteo:
            conteo[palabra] += 1
        else:
            conteo[palabra] = 1
    return conteo

def encontrar_mayor(lista):
    return max(lista)

def invertir_lista(lista):
    return lista[::-1]

def filtrar_pares(lista):
    return [num for num in lista if num % 2 == 0]

def encontrar_segundo_mayor(lista):
    if len(lista) < 2:
        return None
    lista.sort(reverse=True)
    return lista[1]

def contar_vocales(texto):
    vocales = "aeiou"
    cuenta = 0
    for letra in texto.lower():
        if letra in vocales:
            cuenta += 1
    return cuenta

def ordenar_tuplas(lista_tuplas):
    return sorted(lista_tuplas, key=lambda x: x[1])

def contar_unicos(cadena):
    return len(set(cadena))

def palabras_mas_largas(texto, n):
    palabras = texto.split()
    palabras.sort(key=len, reverse=True)
    return palabras[:n]

def es_primo(n):
    if n < 2:
        return False
    for i in range(2, int(n ** 0.5) + 1):
        if n % i == 0:
            return False
    return True

def primos_hasta(n):
    primos = []
    i = 2
    while len(primos) < n:
        if es_primo(i):
            primos.append(i)
        i += 1
    return primos

def menu():
    while True:
        print("\nSeleccione una opción:")
        print("1. Anagrama")
        print("2. Invertir una cadena")
        print("3. Fibonacci")
        print("4. Eliminar duplicados")
        print("5. Palíndromo")
        print("6. Contar palabras")
        print("7. Encontrar el mayor elemento")
        print("8. Invertir una lista")
        print("9. Filtrar números pares")
        print("10. Encontrar el segundo mayor")
        print("11. Contar vocales")
        print("12. Ordenar una lista de tuplas")
        print("13. Contar caracteres únicos")
        print("14. Encontrar palabras más largas")
        print("15. Encontrar números primos")
        print("0. Salir")

        opcion = input("Ingrese el número de la opción: ")

        if opcion == "0":
            break

        if opcion == "1":
            palabra1 = input("Ingrese la primera palabra: ")
            palabra2 = input("Ingrese la segunda palabra: ")
            print(es_anagrama(palabra1, palabra2))
        elif opcion == "2":
            cadena = input("Ingrese la cadena a invertir: ")
            print(invertir_cadena(cadena))
        elif opcion == "3":
            n = int(input("Ingrese el número de términos de Fibonacci: "))
            print([fibonacci(i) for i in range(n)])
        elif opcion == "4":
            lista = input("Ingrese una lista de elementos separados por comas: ").split(",")
            print(eliminar_duplicados(lista))
        elif opcion == "5":
            cadena = input("Ingrese la cadena a verificar si es palíndromo: ")
            print(es_palindromo(cadena))
        elif opcion == "6":
            texto = input("Ingrese el texto para contar palabras: ")
            print(contar_palabras(texto))
        elif opcion == "7":
            lista = list(map(int, input("Ingrese una lista de números separados por comas: ").split(",")))
            print(encontrar_mayor(lista))
        elif opcion == "8":
            lista = input("Ingrese una lista de elementos separados por comas: ").split(",")
            print(invertir_lista(lista))
        elif opcion == "9":
            lista = list(map(int, input("Ingrese una lista de números separados por comas: ").split(",")))
            print(filtrar_pares(lista))
        elif opcion == "10":
            lista = list(map(int, input("Ingrese una lista de números separados por comas: ").split(",")))
            print(encontrar_segundo_mayor(lista))
        elif opcion == "11":
            texto = input("Ingrese el texto para contar vocales: ")
            print(contar_vocales(texto))
        elif opcion == "12":
            lista_tuplas = eval(input("Ingrese una lista de tuplas (ejemplo: [(1,2), (3,1)]): "))
            print(ordenar_tuplas(lista_tuplas))
        elif opcion == "13":
            cadena = input("Ingrese la cadena para contar caracteres únicos: ")
            print(contar_unicos(cadena))
        elif opcion == "14":
            texto = input("Ingrese el texto para encontrar palabras más largas: ")
            n = int(input("Ingrese el número de palabras más largas a encontrar: "))
            print(palabras_mas_largas(texto, n))
        elif opcion == "15":
            n = int(input("Ingrese el número de primos a generar: "))
            print(primos_hasta(n))
        else:
            print("Opción no válida. Intente de nuevo.")

menu()
