def es_anagrama(palabra1, palabra2):
    return sorted(palabra1.lower()) == sorted(palabra2.lower())

def invertir_cadena(cadena):
    return cadena[::-1]

def fibonacci(n):
    if n <= 0:
        return 0
    elif n == 1:
        return 1
    else:
        return fibonacci(n - 1) + fibonacci(n - 2)

def eliminar_duplicados(lista):
    return list(set(lista))

def es_palindromo(cadena):
    cadena = cadena.lower().replace(" ", "")
    return cadena == cadena[::-1]

def contar_palabras(texto):
    palabras = texto.lower().split()
    conteo = {}
    for palabra in palabras:
        conteo[palabra] = conteo.get(palabra, 0) + 1
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
    lista = sorted(set(lista), reverse=True)
    return lista[1] if len(lista) > 1 else None

def contar_vocales(texto):
    return sum(1 for letra in texto.lower() if letra in "aeiou")

def ordenar_tuplas(lista_tuplas):
    return sorted(lista_tuplas, key=lambda x: x[1])

def contar_unicos(cadena):
    return len(set(cadena))

def palabras_mas_largas(texto, n):
    return sorted(texto.split(), key=len, reverse=True)[:n]

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
        print("\n--- Menú de Funciones en Python ---")
        print("1. Verificar anagrama")
        print("2. Invertir cadena")
        print("3. Secuencia Fibonacci")
        print("4. Eliminar duplicados de una lista")
        print("5. Verificar palíndromo")
        print("6. Contar palabras en un texto")
        print("7. Encontrar el número mayor en una lista")
        print("8. Invertir lista")
        print("9. Filtrar números pares")
        print("10. Encontrar el segundo mayor")
        print("11. Contar vocales")
        print("12. Ordenar lista de tuplas por segundo elemento")
        print("13. Contar caracteres únicos en una cadena")
        print("14. Encontrar palabras más largas en un texto")
        print("15. Encontrar primeros N números primos")
        print("16. Salir")
        
        opcion = input("Elige una opción: ")

        if opcion == "1":
            p1 = input("Ingresa la primera palabra: ")
            p2 = input("Ingresa la segunda palabra: ")
            print("Es un anagrama:", es_anagrama(p1, p2))

        elif opcion == "2":
            cadena = input("Ingresa una cadena: ")
            print("Cadena invertida:", invertir_cadena(cadena))

        elif opcion == "3":
            n = int(input("Ingresa el número de términos Fibonacci: "))
            print("Fibonacci:", [fibonacci(i) for i in range(n)])

        elif opcion == "4":
            lista = input("Ingresa una lista de números separados por comas: ")
            lista = list(map(int, lista.split(',')))
            print("Lista sin duplicados:", eliminar_duplicados(lista))

        elif opcion == "5":
            cadena = input("Ingresa una frase: ")
            print("Es palíndromo:", es_palindromo(cadena))

        elif opcion == "6":
            texto = input("Ingresa un texto: ")
            print("Conteo de palabras:", contar_palabras(texto))

        elif opcion == "7":
            lista = list(map(int, input("Ingresa una lista de números separados por comas: ").split(',')))
            print("Número mayor:", encontrar_mayor(lista))

        elif opcion == "8":
            lista = list(input("Ingresa elementos separados por espacio: ").split())
            print("Lista invertida:", invertir_lista(lista))

        elif opcion == "9":
            lista = list(map(int, input("Ingresa una lista de números separados por comas: ").split(',')))
            print("Números pares:", filtrar_pares(lista))

        elif opcion == "10":
            lista = list(map(int, input("Ingresa una lista de números separados por comas: ").split(',')))
            print("Segundo mayor:", encontrar_segundo_mayor(lista))

        elif opcion == "11":
            texto = input("Ingresa una frase: ")
            print("Número de vocales:", contar_vocales(texto))

        elif opcion == "12":
            tuplas = eval(input("Ingresa una lista de tuplas (ejemplo: [(1,3), (2,1), (5,4)]): "))
            print("Lista ordenada:", ordenar_tuplas(tuplas))

        elif opcion == "13":
            cadena = input("Ingresa una cadena de texto: ")
            print("Número de caracteres únicos:", contar_unicos(cadena))

        elif opcion == "14":
            texto = input("Ingresa un texto: ")
            n = int(input("Cantidad de palabras más largas a encontrar: "))
            print("Palabras más largas:", palabras_mas_largas(texto, n))

        elif opcion == "15":
            n = int(input("Ingresa la cantidad de números primos a encontrar: "))
            print("Números primos:", primos_hasta(n))

        elif opcion == "16":
            print("Saliendo del programa...")
            break

        else:
            print("Opción no válida. Intenta de nuevo.")

menu()
