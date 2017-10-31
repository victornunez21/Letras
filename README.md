# Letras

import asyncio
import random
import string

def letra():
    yield "Letras"

def generar_secuencia():
    letra = 'a'
    while True:
        yield 'a'
        yield 'b'
        yield 'c'
        yield 'd'
        yield 'e'
        yield 'f'
        yield 'g'
        yield 'h'
        yield 'i'
        yield 'j'
        yield 'k'
        yield 'l'
        yield 'm'

if __name__ == "__main__":
    generador = letra()
    print(next(generador))

    alfabeto = generar_secuencia()
    for letra in alfabeto:
        print(letra)
        if letra == 'm':
            break
