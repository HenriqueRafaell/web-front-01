# web-front-01
git status- pra saber o que eu to fazendo 
git add . pra adicionar
git checkout -b"" para criar a branch
git comit -m"adicionado arquivo"
git push origin nome_brach - pra subir o arquivo


CABEÇALHO DE DO JAVASCRIPT
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    
</body>
</html>

AULA DE PYTHON DIA 01/11/2023
'''
#1
def soma_elementos(numeros):
    soma = 0
    for num in numeros:
        soma+= num
    return soma

#2
def conta_praes(numeros):
    print(numeros)
    pares = []
    for  num in  numeros:
        print(f"Vou ver se o {num} é par ")
        if num%2 == 0:
            pares.append(num)
            print(pares)
        return pares
#3 a sequencia de nuemeros na liosta tem uma lógica a ser seguida, onde o primeiro numero é o ponto de partida,
# o segundo item é até onde ele vai e o ultimo é de quantos em quantos números ele vai ser contado.
def ivertida_ruinzao(lista):

    invertida = []
    for i in range(len(lista)-1,-1,-1):
     invertida.append(lista[i])
    return invertida

lista = [1,2,3,4,5]
print(lista)
def inverte_lista(lista):
    ultimo = len(lista) - 1
ultimo = len(lista) - 1
    for i in range(len(lista)//2):
     aux = lista[i]
     lista[i] = lista[ultimo - i]
     lista[ultimo - i] = aux
    return lista

def meu_len(lista):
  comprimento = 0
  for elemento in lista:
    comprimento += 1
    print(comprimento)


#5

A = [1,2,3,2,4,5,4]
def remove_repeticoes(lista):
    B = []
    for elemen_a in A:
     encontrei = False
     for elemen_b in B:
        if elemen_b == elemen_a:
            encontrei = True
     if encontrei == False:
        B.append(elemen_a)
     print(B)
'''

#7
def acha_maior(lista):
    indice_maior = 0
    maior = lista[0]
    for i in range(len(lista)):
        candidato = lista[i]
        if candidato > maior:
            maior = candidato
            indice_maior = i
    return indice_maior
lista = [1,2,3,4,5,6]

#6- Jeito de fazer por elemento
def interseccao(lista1,lista2):
    lista1 = [2,4,7,1,0,3]
    lista2 = [9,1,6,0,4,5]
    lista = []
    for elem1 in lista1:
        for elem2 in lista2:
            print(elem1,elem2)
            if elem1 == elem2:
                lista.append(elem1)
                print(lista)
    return  lista
lista1 = [2,4,7,1,0,3]
lista2 = [9,1,6,0,4,5]
inter = interseccao(lista1,lista2)


#Jeito de fazer por indice
print("Novo jeito : \n")
lista = []
for i in range(len(lista1)):
    for j in range(len(lista2)):
        print(lista1[i],lista2[j])
        if lista1[i] == lista2[j]:
            lista.append(lista2[j])
            print(lista)





