# Calculadora-# Definindo a função de adição
def adicao(x, y):
    return x + y

# Definindo a função de subtração
def subtracao(x, y):
    return x - y

# Definindo a função de multiplicação
def multiplicacao(x, y):
    return x * y

# Definindo a função de divisão
def divisao(x, y):
    return x / y

print("Selecione o tipo de operação:")
print("1. Adição")
print("2. Subtração")
print("3. Multiplicação")
print("4. Divisão")

# Solicitando ao usuário que escolha uma opção
escolha = input("Digite a opção (1/2/3/4): ")

# Solicitando os números de entrada
num1 = float(input("Digite o primeiro número: "))
num2 = float(input("Digite o segundo número: "))

# Executando a operação selecionada
if escolha == '1':
    print(num1, "+", num2, "=", adicao(num1, num2))
elif escolha == '2':
    print(num1, "-", num2, "=", subtracao(num1, num2))
elif escolha == '3':
    print(num1, "*", num2, "=", multiplicacao(num1, num2))
elif escolha == '4':
    if num2 == 0:
        print("Erro: Divisão por zero!")
    else:
        print(num1, "/", num2, "=", divisao(num1, num2))
else:
    print("Opção inválida!")
