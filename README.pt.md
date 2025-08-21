**Conteúdo Principal**  
Olá! este repositório contém a implementação de grafos direcionais e não direcionais em linguagem C, usando o método de lista de adjacências.

**O que são listas de adjacências ?**  
Um grafo é uma estrutura que representa relações entre objetos — no caso, vértices.
Esses vértices se conectam por “caminhos” (arestas) que ligam um ao outro.
A lista de adjacências armazena, para cada vértice, todos os vértices aos quais ele está conectado.
Isso nos permite implementar algoritmos de busca a partir do grafo e das relações entre os vértices.

**Vantagens e Desvantagens da implementação por lista de adjacências**  
**Vantagens:**

- Uso de structs torna o código mais legível.

- Manutenção e compreensão mais fáceis.

- Implementação relativamente simples.

**Desvantagens:**

- Maior uso de memória comparado a matrizes de adjacência.

- Requer mais processamento em alguns casos.

*Alternativa:* Matriz de adjacência — mais leve e rápida em certos cenários, mas mais difícil de manter e implementar.

**Algoritmos de busca implementados**  

Os grafos podem utilizar diferentes algoritmos de busca para encontrar o caminho mais curto entre dois vértices ou verificar alcance (quais vértices são acessíveis a partir de outro). Nesta implementação, o grafo direcional utiliza o algoritmo DFS (Depth-First Search), que consiste em ir o mais fundo possível em um caminho antes de voltar e explorar outros. Esse algoritmo é ótimo para verificar conexões e detectar ciclos. O DFS nos permite acessar todos os vértices do grafo, mesmo aqueles que não possuem ligação com nenhum outro vértice, o que pode gerar várias árvores ao final da busca; por isso diz-se que o algoritmo DFS gera uma floresta.  

Já o grafo não direcional utiliza o algoritmo BFS (Breadth-First Search), que funciona visitando todos os vizinhos de um vértice antes de aprofundar a busca. Isso permite determinar o caminho mais curto (em número de arestas) entre o vértice inicial e os demais vértices acessíveis. Diferente do DFS, o BFS gera como resultado apenas a árvore formada pelos vértices que são acessíveis a partir do vértice inicial, predefinido no começo da busca.  

Os algoritmos DFS e BFS não são exclusivos de grafos direcionais ou não direcionais; ambos funcionam em qualquer tipo de grafo. A escolha entre eles depende do objetivo da busca: DFS é mais indicado para explorar completamente a estrutura do grafo e detectar ciclos, enquanto BFS é mais indicado para determinar distâncias mínimas e caminhos mais curtos.  

[Leia isso em Inglês](README.en.md)
