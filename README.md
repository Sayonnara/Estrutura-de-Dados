
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

Fila (Queue)
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

