
# Estrutura-de-Dados

- Estruturas de dados são fundamentais para organizar, armazenar e gerenciar dados de forma eficiente, permitindo que algoritmos realizem operações com maior performance e clareza. Em programação, elas ajudam a resolver problemas específicos ao definir como os dados são representados e manipulados no código.

# Por que Estruturas de Dados Existem?
As estruturas de dados existem para otimizar o uso da memória, simplificar operações complexas e tornar o código mais eficiente. Cada tipo de estrutura é projetado para resolver certos problemas melhor do que outras alternativas. 

Por exemplo:

 - Listas são ótimas para armazenar e acessar uma sequência de dados.
 - Pilhas e filas são ideais para operações onde a ordem de entrada e saída importa.
 - Árvores e grafos são usadas para representar hierarquias ou redes de dados complexos, como redes sociais ou mapas.

#  Benefícios das Estruturas de Dados

Eficiência: Usar a estrutura certa economiza tempo e recursos.

Organização: Estruturas bem escolhidas tornam o código mais legível e organizado.

Escalabilidade: Algumas estruturas são melhores para grandes volumes de dados, ajudando o programa a lidar com crescimento sem perda de performance.

# Principais Estruturas de Dados e Como Usá-las no Código

Arrays ou Listas
   
Definição: Conjuntos de elementos armazenados em posições contínuas de memória.

Uso no Código: Em Python, uma lista pode ser criada assim:

python

Lista = [1, 2, 3, 4]

Aplicação: Para armazenar itens de forma sequencial.

# Pilha (Stack)

Definição: Estrutura LIFO (Last In, First Out), onde o último elemento inserido é o primeiro a ser removido.

Uso no Código:

python

Copiar código

pilha = []

pilha.append(1)  # Insere na pilha

pilha.pop()      # Remove o último elemento inserido

- Aplicação: Utilizada em algoritmos de navegação, como o "desfazer" em editores de texto.

# Fila (Queue)

Definição: Estrutura FIFO (First In, First Out), onde o primeiro elemento inserido é o primeiro a sair.

Uso no Código:
python

from collections import deque

fila = deque([1, 2, 3])

fila.append(4)     # Insere no final

fila.popleft()     # Remove o primeiro elemento

- Aplicação: Usada em processamento de tarefas, como sistemas de impressão.

  # Dicionários (Hash Maps)
  
Definição: Estrutura que armazena pares de chave-valor, permitindo acesso rápido aos valores pela chave.

dicionario = {"chave1": "valor1", "chave2": "valor2"}

valor = dicionario["chave1"]

- Aplicação: Ideal para buscas rápidas, como em sistemas de inventário.

# Árvores

Definição: Estrutura hierárquica com um nó raiz e subnós, representando relações de "pai e filho".

Uso no Código: Representada como uma classe onde cada nó aponta para os nós filhos

class No:

    def __init__(self, valor):
        self.valor = valor
        self.filhos = []
        
- Aplicação: Útil em bancos de dados, sistemas de arquivos e algoritmos de busca.

# Grafos

Definição: Conjunto de nós conectados por arestas, representando redes ou conexões.

Uso no Código: Representado por listas de adjacência ou matrizes

grafo = { "A": ["B", "C"], "B": ["A", "D"], "C": ["A", "D"], "D": ["B", "C"] }

 #DICA

## Como Usar Estruturas no Código e Entender a Escolha
- Ao escolher uma estrutura de dados, pergunte-se:

1- Qual é o volume de dados?

Para grandes volumes, prefira estruturas eficientes em espaço e tempo.

2 -Qual a frequência das operações?

Se você precisa inserir ou deletar constantemente, pilhas e filas são ótimas opções.

3 -Quais operações são mais usadas?

Se buscas rápidas são essenciais, os dicionários podem ser uma boa escolha.

Cada estrutura vem com suas vantagens, e o uso eficiente delas otimiza a solução e contribui para um código de qualidade.

 # 1. Lista
Uma lista em Python pode armazenar elementos em sequência e é ideal para acessar dados por índice.

python
Copiar código
### Criando uma lista de números
lista = [10, 20, 30, 40]

### Adicionando um elemento
lista.append(50)

### Acessando elementos
print(lista[0])  # Saída: 10

### Removendo o último elemento
lista.pop()

print(lista)  # Saída: [10, 20, 30, 40]

# Pilha (Stack)
Uma pilha usa a abordagem LIFO (Last In, First Out). O último elemento adicionado é o primeiro a ser removido.

python

### Criando uma pilha
pilha = []

### Adicionando elementos
pilha.append("a")
pilha.append("b")
pilha.append("c")

### Removendo o último elemento
print(pilha.pop())  # Saída: "c"

### Visualizando a pilha
print(pilha)  # Saída: ["a", "b"]

# Fila (Queue)

Uma fila segue a ordem FIFO (First In, First Out), onde o primeiro elemento inserido é o primeiro a sair.

from collections import deque

### Criando uma fila
fila = deque()

### Adicionando elementos na fila
fila.append("primeiro")

fila.append("segundo")

fila.append("terceiro")

### Removendo o primeiro elemento
print(fila.popleft())  # Saída: "primeiro"

### Visualizando a fila
print(fila)  # Saída: deque(['segundo', 'terceiro'])

# Dicionário (Hash Map)

Os dicionários armazenam pares de chave-valor, permitindo acessar valores rapidamente por sua chave.

### Criando um dicionário
dicionario = {"nome": "Alice", "idade": 25, "cidade": "São Paulo"}

### Acessando um valor
print(dicionario["nome"])  # Saída: "Alice"

### Adicionando um novo par chave-valor
dicionario["profissão"] = "Engenheira"

### Removendo uma chave
del dicionario["cidade"]

print(dicionario)  # Saída: {'nome': 'Alice', 'idade': 25, 'profissão': 'Engenheira'}

# Árvore
Uma árvore pode ser representada por uma classe com um nó raiz que contém referências para seus filhos.

class No:
    def __init__(self, valor):
        self.valor = valor
        self.filhos = []

### Criando nós
raiz = No("raiz")

filho1 = No("filho1")

filho2 = No("filho2")

### Adicionando filhos ao nó raiz

raiz.filhos.append(filho1)

raiz.filhos.append(filho2)

### Visualizando a árvore

print(raiz.valor)  # Saída: "raiz"

for filho in raiz.filhos:

    print(filho.valor)  # Saída: "filho1" e "filho2"

# Grafo
Um grafo pode ser representado como um dicionário, onde cada chave é um nó e seu valor é uma lista dos nós conectados.

### Criando um grafo com lista de adjacência
grafo = {

    "A": ["B", "C"],
    
    "B": ["A", "D"],
    
    "C": ["A", "D"],
    
    "D": ["B", "C"]
    
}

### Visualizando conexões do nó "A"

print(grafo["A"])  # Saída: ['B', 'C']

### Conexões de "D"

print(grafo["D"])  # Saída: ['B', 'C']

