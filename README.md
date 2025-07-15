# Projeto: Ordenação de Pessoas por Nome

Este projeto implementa e compara três algoritmos de ordenação para organizar um vetor de 100 pessoas (com nomes e idades) por ordem alfabética do nome. As ordenações são feitas utilizando os algoritmos **Bubble Sort**, **Selection Sort** e **Quick Sort**, com medição de tempo médio, número de comparações e trocas realizadas.


## Algoritmos Implementados

###  Bubble Sort

O Bubble Sort percorre repetidamente a lista, comparando pares de elementos adjacentes e trocando-os se estiverem fora de ordem. Esse processo se repete até que a lista esteja ordenada.

**Funcionamento:**
- Passa pelo vetor diversas vezes.
- A cada passagem, o maior elemento “bolha” para o final da lista.

**Vantagens:** Simples de entender e implementar.  
**Desvantagens:** Ineficiente para grandes conjuntos de dados.

###  Selection Sort

O Selection Sort divide o vetor em duas partes: a ordenada e a não ordenada. A cada iteração, ele seleciona o menor elemento da parte não ordenada e o move para o final da parte ordenada.

**Funcionamento:**
- Localiza o menor elemento no vetor.
- Troca esse elemento com o elemento na posição inicial da parte não ordenada.
- Repete até ordenar todo o vetor.

**Vantagens:** Menor número de trocas que o Bubble Sort.  
**Desvantagens:** Muitas comparações, independente da ordenação inicial.

### Quick Sort

O Quick Sort é um algoritmo eficiente de ordenação baseado na técnica de divisão e conquista. Escolhe um pivô e reorganiza os elementos de modo que os menores fiquem antes do pivô e os maiores, depois. Esse processo é repetido recursivamente para as sublistas.

**Funcionamento:**
- Escolhe um pivô.
- Divide o vetor em dois grupos: menores e maiores que o pivô.
- Ordena recursivamente os dois grupos.

**Vantagens:** Muito eficiente para grandes volumes de dados.  
**Desvantagens:** Pode ter desempenho ruim no pior caso (pivot ruim).

 Complexidade dos Algoritmos

| Algoritmo     | Melhor Caso | Médio Caso | Pior Caso | Complexidade de Espaço |
|:---------------|:--------------|:--------------|:--------------|:-----------------------|
| Bubble Sort    | O(n)        | O(n²)      | O(n²)      | O(1)                    |
| Selection Sort | O(n²)       | O(n²)      | O(n²)      | O(1)                    |
| Quick Sort     | O(n log n)  | O(n log n) | O(n²)      | O(log n) (recursão)     |


 Resultados Obtidos (para 100 pessoas)

| Algoritmo     | Comparações | Trocas | Tempo Médio (ms) |
|:---------------|:---------------|:-----------|:------------------|
| **Bubble Sort**    | 4950          | 2626      | 0.148             |
| **Selection Sort** | 4950          | 93        | 0.050             |
| **Quick Sort**     | 490           | 185       | 0.018             |

