# Projeto: Programa de Cálculo de IMC em Python

## 📚 Descrição
Este projeto foi desenvolvido durante o **1º semestre** do curso de **Cibersegurança - UNOPAR** como parte da disciplina de **Linguagem de Programação**. O objetivo foi criar um programa em Python para calcular o **Índice de Massa Corporal (IMC)**, utilizando o **Google Cloud Shell Editor** como ambiente de desenvolvimento.

O programa solicita ao usuário suas informações básicas (nome, peso e altura), realiza o cálculo do IMC e exibe a classificação correspondente (abaixo do peso, peso saudável, sobrepeso ou obesidade).

---

## 🛠️ Ferramentas Utilizadas
- **Google Cloud Shell Editor** (ambiente de nuvem para codificação)
- **Python 3** (linguagem principal)

---

## 🗂️ Estrutura do Projeto
- Relatório completo (PDF) [Projeto-Linguagem de Programação-Unopar-1ºSemestre.pdf](https://github.com/user-attachments/files/19130757/Projeto-Linguagem.de.Programacao-Unopar-1.Semestre.pdf)

- Código-fonte do programa em Python (`calculadora_imc.py`)

---

## 🔎 Aprendizados e Competências Desenvolvidas
- Manipulação de entrada de dados com `input()`
- Operações matemáticas básicas e operadores aritméticos
- Uso de estruturas condicionais (`if`, `elif`, `else`)
- Impressão formatada com `print()`
- Prática de desenvolvimento em ambiente de nuvem (Google Cloud Shell)

---

## 📊 Principais Funcionalidades
- Solicitação de nome, peso e altura do usuário
- Cálculo do IMC com fórmula: `peso / (altura ** 2)`
- Classificação automática com base no valor do IMC
- Exibição personalizada do resultado incluindo nome do usuário e categoria de peso

---

## 📅 Semestre
1º Semestre - Curso de Cibersegurança - UNOPAR

---

## 👨‍🎓 Autor
Silvio Rodrigues Gouvêa

---

## 🔗 Referências
- [Google Cloud Shell Editor](https://cloud.google.com/shell?hl=pt-br)
- [Guia do Iniciante em Python](https://wiki.python.org/moin/BeginnersGuide)
- [Cálculo do IMC](https://encurtador.com.br/fgizM)

---

## 📁 Código Fonte - calculadora_imc.py

```python
# Solicita ao usuário que insira seu nome
nome = input("Digite seu nome: ")

# Solicita ao usuário que insira seu peso em quilogramas
peso = float(input(f"Agora, {nome}, por favor digite seu peso em quilogramas: "))

# Solicita ao usuário que insira sua altura em metros
altura = float(input(f"Agora por favor digite sua altura em metros: "))

# Calcula o IMC (Índice de Massa Corporal)
imc = peso / (altura**2)

# Exibe o IMC com 2 casas decimais
print(f"\n{nome}, seu IMC é: {imc:.2f}")

# Determina a categoria do IMC
if imc < 18.5:
    print("Você está abaixo do peso.")
elif 18.5 <= imc < 24.9:
    print("Seu peso está saudável.")
elif 25 <= imc < 29.9:
    print("Você está com sobrepeso.")
elif 30 <= imc < 34.9:
    print("Você está com obesidade grau 1.")
elif 35 <= imc < 39.9:
    print("Você está com obesidade grau 2.")
else:
    print("Você está com obesidade grau 3 (Mórbida).")
```
