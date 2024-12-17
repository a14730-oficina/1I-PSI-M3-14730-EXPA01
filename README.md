# Guess The Number.

import random

def gerar_numero():
    return random.randint(1, 20)
def exit():
    print("Bem-vindo vamos começar!")
    print("----------GUESS THE NUMBER----------")
    nome = input("mete o seu nome: ")
    numero = gerar_numero()
    tentativas = 6
    vencedor = False
    while tentativas > 0:
        print(f"\n{nome},tens {tentativas} tentativas restantes.")
        tentativa = int(input("insira um valor (0-20): "))

        if tentativa < numero:
            print("superior.")
        elif tentativa > numero:
            print("inferior.")
        else:
            print(f"Parabéns {nome}, acertas-te!")
            vencedor = True
            break
        tentativas -= 1
    if not vencedor:
        print(f"Que pena! O número certo era {numero}.")

    jogar_novamente = input("queres jogar outra vez? (s/n): ")
    if jogar_novamente.lower() == 's':
        exit()
    else:
        print(f"{nome} espero que tenhas gostado, obrigado(a)!")
if "__exit__":
    exit()
