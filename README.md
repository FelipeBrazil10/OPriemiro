personagens = []
limite = 0

def PersoName():
    global personagens
    nome = input ("Escolha um nome para seu personagem: ")
    personagens.append(nome)
    return print ("Olá", nome)

def PersoClasse():
    classes = ["Mago", "Cavaleiro", "Arqueiro"]
    klasse = int (input ("Qual classe você deseja para seu personagem: Digite 1 para Mago, 2 para Cavaleiro, 3 para Arqueiro "))
    if klasse == 1:
        print ("Seu personagem é um", classes [0])
        personagens.append(classes[0])
    if klasse == 2:
        print ("Seu personagem é um", classes [1])
        personagens.append(classes[1])
    if klasse == 3:
        print ("Seu personagem é um", classes [2])
        personagens.append(classes[2])

while limite <= 3:
    PersoName()
    PersoClasse()
    limite += 1

print (personagens)
