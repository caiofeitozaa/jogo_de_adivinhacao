from random import randint
from time import sleep

print("-=" * 20)

total_vitorias = 0
computador = randint(0, 20)

while True:

    print("A máquina pensou em um número")
    sleep(0.5)
    usuario = int(input("Você consegue adivinhar ? "))
    sleep(0.3)

    print("Verificando resultados...")
    sleep(2)

    print(f"A máquina pensou no número {computador}.")
    sleep(0.5)

    print("-=" * 20)

    if usuario == computador:
        print("Parabéns, você ganhou :)\nContinue...")
        total_vitorias += 1

    else:
        print("Que pena, você perdeu :(")
        break

if total_vitorias > 0:
    if total_vitorias == 1:
        print("Você venceu 1 vez.")

    else:
        print(f"Você venceu {total_vitorias} vezes seguidas")
  
