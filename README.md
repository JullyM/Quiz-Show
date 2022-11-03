import time
p = 0
print("Ola! Bem vindo ao Quiz Show!")
time.sleep(1)
print("Iremos fazer algumas perguntas de conhecimentos gerais com tres alternativas e lhes diremos se sua resposta esta correta ou nao, boa sorte!")
time.sleep(4)
print("Devo lembrar que nas respostas, voce deve escrever 'a' ou 'b' ou 'c'")
time.sleep(2)
nome = input("Mas primeiramente, gostaria de saber seu nome: ")
print(f"Perfeito {nome}! Vamos começar!")
contagem = [3, 2, 1, "Vamos la!"]
for i in contagem:
    time.sleep(1)
    print(i)
time.sleep(2)
#perguntas-------------
#pergunta1-------------
print("1. Quantos estados tem o Brasil?")
print("a) 28  b)26  c)24")
r1 = input("Resposta: ")
if r1 == "a" or r1 == "c":
    print("Resposta errada!")
    time.sleep(1)
    print("A resposta correta seria: b)26")
elif r1 == "b":
    print("Resposta certa!")
    p = p + 1
#pergunta2-------------
time.sleep(2)
print("2. Quem inventou o chuveiro eletrico?")
print("a) Evaristo Engelberg  b)Santos Dumont  c)Francisco Canhos")
r2 = input("Resposta: ")
if r2 == "a" or r2 == "b":
    print("Resposta errada!")
    time.sleep(1)
    print("A resposta correta seria: c)Francisco Canhos")
elif r2 == "c":
    print("Resposta certa!")
    p = p + 1
#pergunta3-------------
time.sleep(2)
print("3. Qual o valor de x na expressão: 4x + 2 = 16")
print("a)4,5  b)3,5  c)5,5")
r3 = input("Resposta: ")
if r3 == "a" or r3 == "c":
    print("Resposta errada!")
    time.sleep(1)
    print("A resposta correta seria: b)3,5")
elif r3 == "b":
    print("Resposta certa!")
    p = p + 1
#pergunta4-------------
time.sleep(2)
print("4. Qual é o menor e o maior pais do mundo?")
print("a)Vaticano e Rússia  b)Vaticano e China  c)Mônaco e Rússia")
r4 = input("Resposta: ")
if r4 == "b" or r4 == "c":
    print("Resposta errada!")
    time.sleep(1)
    print("A resposta correta seria: a)Vaticano e Rússia")
elif r4 == "a":
    print("Resposta certa!")
    p = p + 1
#pergunta5-------------
time.sleep(2)
print("5. Qual o livro mais vendido no mundo depois da Biblia?")
print("a)O Senhor dos Aneis  b)O Pequeno Principe  c)Dom Quixote")
r4 = input("Resposta: ")
if r4 == "a" or r4 == "b":
    print("Resposta errada!")
    time.sleep(1)
    print("A resposta correta seria: c)Dom Quixote")
elif r4 == "c":
    print("Resposta certa!")
    p = p + 1
#resultado-------------
time.sleep(2)
print("Fim das perguntas! Analisando seus dados...")
a = [".", ".", ".",]
for j in a:
    time.sleep(1)
    print(j)
if p < 3:
    print(f"E uma pena, {nome} voce obteve {p} pontos, mais sorte da proxima vez!")
elif p == 3 or p == 4:
    print(f"Muito bem, mas foi quase! {nome} voce obteve {p} pontos, mais sorte na proxima vez!")
elif p == 0:
    print("Vamos estudar imediatamente! {nome} voce obteve {p} pontos, mais sorte da proxima vez!")
elif p == 5:
    print(f"Parabens gênio! {nome} voce obteve {p} pontos!")
