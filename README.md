# 1I-PSI-M3-14730-EXPA01
def calcula_area_triagulo():
    base = float(input("Introduza a base do triângulo: "))
    altura = float(input("Introduza a altura do triângulo: "))
    area = (base * altura) / 2
    return area
def calcula_area_circulo():
    raio = float(input("Introduza o raio do círculo: "))
    area = 3.14 * raio ** 2
    return area
def calcula_area_retangulo():
    base = float(input("Introduza a base do retângulo: "))
    altura = float(input("Introduza a altura do retângulo: "))
    area = base * altura
    return area
opcao = int(input("Qual figura deseja calcular a área? \n1. Triângulo \n2. Círculo \n3. Retângulo \n"))
if opcao == 2:
    area = calcula_area_circulo()
    print(f"A área do círculo é: {area}")
elif opcao == 1:
    area = calcula_area_triagulo()
    print(f"A área do triângulo é: {area}")
elif opcao == 3:
    area = calcula_area_retangulo()
    print(f"A área do retângulo é: {area}")
