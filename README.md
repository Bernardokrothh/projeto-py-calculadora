# Calculadora em Python

## 📌 Descrição
Projeto em **Python** que implementa uma **calculadora básica** capaz de realizar **soma, subtração, multiplicação e divisão**.  
Foi desenvolvido como prática de **lógica de programação**, **condicionais**, **loops** e **interação com o usuário no console**.

---

## 🛠 Tecnologias
- Linguagem Python  
- Console/Terminal  
- Estruturas de controle (if/else, while)  

---

## ⚙ Funcionalidades
- Operações matemáticas básicas: soma, subtração, multiplicação e divisão  
- Tratamento de divisão por zero  
- Menu interativo com opção de sair  

---

## 💻 Código

```python
def soma(a, b):
    return a + b

def subtracao(a, b):
    return a - b

def multiplicacao(a, b):
    return a * b

def divisao(a, b):
    if b != 0:
        return a / b
    else:
        return "Erro: divisão por zero!"

def main():
    while True:
        print("\\n--- Calculadora Simples ---")
        print("1. Soma")
        print("2. Subtração")
        print("3. Multiplicação")
        print("4. Divisão")
        print("5. Sair")
        
        opcao = input("Escolha uma opção: ")

        if opcao == "5":
            print("Encerrando calculadora.")
            break

        num1 = float(input("Digite o primeiro número: "))
        num2 = float(input("Digite o segundo número: "))

        if opcao == "1":
            print("Resultado:", soma(num1, num2))
        elif opcao == "2":
            print("Resultado:", subtracao(num1, num2))
        elif opcao == "3":
            print("Resultado:", multiplicacao(num1, num2))
        elif opcao == "4":
            print("Resultado:", divisao(num1, num2))
        else:
            print("Opção inválida!")

if __name__ == "__main__":
    main()
