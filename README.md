# Árvore Binária de Busca

## o que foi feito

Este trabalho foi desenvolvido com base na implementação da árvore binária disponibilizada pelo professor.

O projeto consiste em uma Árvore Binária capaz de:

- inserir elementos;
- percorrer a árvore em pré-ordem;
- percorrer em ordem;
- percorrer em pós-ordem;
- remover elementos da árvore.

A parte principal do trabalho foi a implementação da remoção de nós, tratando todos os casos necessários.

O desenvolvimento foi feito utilizando Java no Cursor durante a escrita e organização do código.


# Tipos de remoção implementados

## Remoção de nó folha

Quando o nó não possui filhos, a remoção é mais simples, pois basta remover a referência daquele nó.

Exemplo:

20

Após remover:

null


## Remoção de nó com um filho

Nesse caso, o nó removido é substituído diretamente pelo seu único filho.

Exemplo:

30
 |
40

Após remover 30:

40


## Remoção de nó com dois filhos

Para nós com dois filhos foi utilizada a estratégia do sucessor.

acontece da seguinte forma:

1. é localizado o menor valor da subárvore direita;
2. esse valor substitui o nó removido;
3. depois o sucessor original é removido da árvore.

assim mantém a estrutura correta da Árvore Binária de Busca.


# Sobre a implementação recursiva

A implementação foi feita utilizando recursão porque combina bastante com a estrutura de árvores binárias.

Como cada nó pode possuir outros nós à esquerda e à direita, a recursão deixa o código mais simples de entender e organizar, principalmente durante a navegação pela árvore.

Na remoção, ela facilitou bastante o tratamento dos três casos pedidos no trabalho:
- nó folha;
- nó com um filho;
- nó com dois filhos.

Além disso, a versão recursiva evita criar estruturas auxiliares para controlar o caminho percorrido na árvore, deixando a implementação mais limpa.

# Tecnologias utilizadas

- Java
- Cursor

# saida do terminal

Árvore Binária criada com sucesso!

O nó -3 foi inserido na Árvore.
O nó -5 foi inserido na Árvore.
O nó -4 foi inserido na Árvore.
O nó 5 foi inserido na Árvore.
O nó 3 foi inserido na Árvore.
O nó 4 foi inserido na Árvore.
O nó 10 foi inserido na Árvore.
O nó 7 foi inserido na Árvore.
O nó 9 foi inserido na Árvore.

PERCURSO EM ORDEM:

-5
-4
-3
0
3
4
5
7
9
10

Removendo nó folha (-4):

-5
-3
0
3
4
5
7
9
10

Removendo nó com um filho (10):

-5
-3
0
3
4
5
7
9

Removendo nó com dois filhos (5):

-5
-3
0
3
4
7
9


# Autor

Mateus Augusto Xavier Pinheiro
