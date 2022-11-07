# Algoritmo: Pesquisa Binária

Este algoritmo também é conhecido como: "Binary Search", "Half-interval Search", "Logaritmic Search" e "Binary Chop".

É um algoritmo utilizado para pesquisar um valor em uma lista ordenada.
Comparativamente, ao se pesquisar item por item (pesquisa linear), leva-se, no pior cenário, O(n) comparações, onde n é o número de itens na lista.
Já utilizando a pesquisa binária, no pior dos casos, leva-se O(log<sub>2</sub>n).

Exemplo 1: Lista com 1.000 elementos
- Pesquisa Linear: 1.000 comparações;
- Pesquisa Binária: 10 comparações (log(2)1000 + 1) Obs. Arredonda-se o resultado de log(2)1000 para baixo.

Exemplo 2: Lista com 1.000.000.000.000 de elementos
- Pesquisa Linear: 1.000.000.000.000 de comparações;
- Pesquisa Binária: 40 comparações.

Assim, observamos que, quanto maior a lista, mais eficiente é a pesquisa binária.

O algoritmo em si é relativamente simples.
Dada uma lista ordenada, ele compara o elemento do meio da lista com o item pesquisado.
Caso este elemento não seja o item procurado, ele verifica se o item prucurado é maior ou menor que o elemento do meio.
Se for maior, ele elimina a menor metade da lista, e se for menor, elimina a maior metade.
Em sequida, compara o elemento do meio desta nova lista, e repete o procedimento até encontrar o elemento.

Desta forma, em uma pesquisa linear, a cada comparação, são eliminados apenas 1 elemento, enqaunto que na pesquisa binária, a cada comparação, é eliminada metade dos elementos da lista.

No arquivo "pesquisa_binaria-EXEMPLO.py", em Python, há uma lista com mil elementos e duas funções (pesquisa_binaria e pesquisa_linear), com o propósito de comparar a quantidade de comparações feitas por cada algoritmo.

Veja o meu artigo completo sobre este algoritmo neste link: [https://www.linkedin.com/pulse/busca-bin%C3%A1ria-um-algoritmo-simples-e-muito-eficiente-lucas-menegatti/](https://www.linkedin.com/pulse/busca-bin%C3%A1ria-um-algoritmo-simples-e-muito-eficiente-lucas-menegatti/)
