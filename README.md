# N-meros-pares-ou-mpares
Programa que identifica se números são pares ou ímpares.
pares = 0
impares = 0

print("=== Verificador de Números Pares e Ímpares ===")
print("Digite números inteiros. Para encerrar, digite 'fim'.\n")

while True:
    entrada = input("Digite um número inteiro ou 'fim' para encerrar: ")

    # Verifica se o usuário quer encerrar
    if entrada.lower() == 'fim':
        break

    try:
        numero = int(entrada)

        # Verifica se o número é par ou ímpar
        if numero % 2 == 0:
            print(f"{numero} é par.\n")
            pares += 1
        else:
            print(f"{numero} é ímpar.\n")
            impares += 1

    except ValueError:
        print("⚠️ Entrada inválida! Digite um número inteiro válido.\n")

# Exibe o resultado final
print("\n=== Resultado Final ===")
print(f"Quantidade de números pares: {pares}")
print(f"Quantidade de números ímpares: {impares}")
print("Programa encerrado.")
