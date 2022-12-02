# Teoria dos Grafos

## Sobre :
&nbsp;&nbsp;&nbsp;Esse repositorio tem como conteudo os algoritmos necessarios para a segunda avaiação da materia de Teoria dos Grafos.

## Dupla :
+ Carlos Eduardo Noslin Tenório Galvão
+ Maurício Mateus dos Santos

## Estrutura :
+ A estrutura principal desse repositorio é: 
  + Um diretório para cada algoritmo:
    + Um codigo .cpp para cada algoritmo.
    + Um arquivo de entrada para cada algoritmo.
    + Um makefile.

## Makefile :
+ O Makefile tem apenas dois comandos:
  + make: Quando você estiver em um dos diretórios do algoritmo, o comando "make" no prompt ira gerar o arquivo binário do aplicativo juntamente com o arquivo .o .

  + make clean: Ao declarar o comando "make clean" no prompt você irá deletar todos os arquivos gerados com o comando make, revertendo o diretório para ter apenas seus arquivos originais.

# Algoritmos :

## Algoritmo Dijkistra :

### Estrutura de entrada : 
---
&nbsp;&nbsp;&nbsp;A entrada para o algoritmo dijkstra é: 

&nbsp;&nbsp;&nbsp;A primeira linha para o número de vértices e arestas seguida por um número de linhas, correspondente ao número de arestas, onde cada linha corresponde à lista de adjacências do grafo. Na ultima linha recebemos duas variáveis ​​inteiras referentes ao vértice inicial e ao vértice destino.
```
7 9
5 3 9
2 0 24
0 3 3
1 2 4
0 1 5
1 5 20
5 2 1
5 4 6
2 6 18
1 3
```

### Executando :
---
&nbsp;&nbsp;&nbsp;Para executaro algoritmo Dijkistra o localizando em seu diretório e executando o make para gerar seu bin. Com o arquivo bin <span style="color:#747ee8">dijkstra</span> gerado, execute o seguinte comando no prompt:<span style="color:#747ee8"> ./dijkstra</span>, depois digite sua entrada de acordo com a configuração acima.

### Executando com o arquivo de Entrada:
---
&nbsp;&nbsp;&nbsp;Para executar o algoritmo Dijkstra com a entrada do arquivo de exemplo, siga as etapas acima, mas na chamada do arquivo bin, digite<span style="color:#747ee8">./dijkstra < nome do arquivo de entrada</span>, para a nossa entrada usamos o nome: <span style="color:#747ee8">./dijkstra < dijkstraInput</span>.

### Exemplo de Saida: 
---
&nbsp;&nbsp;&nbsp;A saida do algoritmo Dijkstra é uma mensagem mostrando qual a menor distancia entre os dois vetores recebidos ao final.

<span style="color:#747ee8">A menor distancia entre os vértices: 1 e 3 é 8</span>

---
</br>

## Algoritmo de Ford Fulkerson : 

### Estrutura de Entrada : 
---
&nbsp;&nbsp;&nbsp;A entrada para o algoritmo Ford Fulkerson é:

&nbsp;&nbsp;&nbsp;A primeira linha contendo o numero de vertices e arestas seguido pelo numero de linhas, correspondente ao numero de arestas, onde cada um é uma linha para a lista de adjacencia do grafo. Na ultima linha recebemos duas variáveis ​​inteiras referentes ao vértice inicial e ao vértice destino.

```
5 6
0 2 5
0 3 3
3 1 5
2 1 2
1 4 7
2 4 2
0 4
```

### Executando :
---
&nbsp;&nbsp;&nbsp;Para executar o algoritmo Ford Fulkerson o localizando em seu diretório e executando o make para gerar seu bin. Com o arquivo bin <span style="color:#747ee8">fordFulkerson < dijkstraInput</span> gerado, execute o seguinte comando no prompt:<span style="color:#747ee8"> ./fordFulkerson</span>, depois digite sua entrada de acordo com a configuração acima.

### Executando com o arquivo de Entrada:
---
&nbsp;&nbsp;&nbsp;Para executar o algoritmo Ford Fulkerson com a entrada do arquivo de exemplo, siga as etapas acima, mas na chamada do arquivo bin, digite <span style="color:#747ee8">./fordFulkerson < nome do arquivo de entrada</span>, para a nossa entrada usamos o nome: <span style="color:#747ee8">./fordFulkerson < fordFulkersonInput</span>.

### Exemplo de Saida: 
---
&nbsp;&nbsp;&nbsp;A saida do algoritmo Ford Fulkerson é uma mensagem mostrando <<span style="color:#747ee8">O fluxo máximo do vetor x é: y</span>.

---
</br>

## Kruskal algoritmo :

### Estrutura de Entrada : 
---
&nbsp;&nbsp;&nbsp;A entrada para o algoritmo Kruskal é:

&nbsp;&nbsp;&nbsp;O numero correspondente as arestas e vetores e um numero correspondente ao numero de entradas,onde cada uma será uma lista de adjacências do grafo. 
```
8 16
0 2 4
0 3 6
0 4 2
1 5 3
1 6 3
2 0 4
3 0 6
3 5 1
4 0 2
4 6 6
4 7 8
5 1 3
5 3 1
6 1 3
6 4 6
7 4 8
```

### Executando :
---
&nbsp;&nbsp;&nbsp;Para executar o algoritmo Kruskal o localizando em seu diretório e executando o make para gerar seu bin. Com o arquivo bin <span style="color:#747ee8">kruskal</span> gerado, execute o seguinte comando no prompt: <span style="color:#747ee8">./kruskal</span>, depois digite sua entrada de acordo com a configuração acima.

### Executando com o arquivo de entrada :
---
&nbsp;&nbsp;&nbsp;Para executar o algoritmo Kruska com a entrada do arquivo de exemplo, siga as etapas acima, mas na chamada do arquivo bin, digite <span style="color:#747ee8">./kruskal < nome do arquivo de entrada</span>, para a nossa entrada usamos o nome: <span style="color:#747ee8">./kruskal < kruskalInput</span>

### Exemplo de Saida: 
---
&nbsp;&nbsp;&nbsp;A saida do algoritmo Kruskal é uma mensagem mostrando <<span style="color:#747ee8">As Bordas da Árvore geradora são: (x, y)</span>.

---
```
As Bordas da Árvore geradora são: 
(3, 5)
(0, 4)
(1, 5)
(1, 6)
(0, 2)
(0, 3)
(4, 7)
```
---
</br>

## Prim algoritmo :

### Estrutura de Entrada : 
---
&nbsp;&nbsp;&nbsp;A entrada para o algoritmo Prim é:

&nbsp;&nbsp;&nbsp;A primeira linha para o número de vértices e arestas seguida de um número de linhas, correspondente ao número de arestas, sendo cada uma delas uma linha para a lista de adjacências do grafo.
```
9 13
0 1 4
0 7 8
1 2 8
1 7 11
2 3 7
2 8 12
2 5 4
3 4 9
3 5 14
4 5 2
5 6 10
6 7 9
7 8 6
```

### Executando : 
---
&nbsp;&nbsp;&nbsp;Para executar o algoritmo Prim o localizando em seu diretório e executando o make para gerar seu bin. Com o arquivo bin <span style="color:#747ee8">prim</span>  gerado, execute o seguinte comando no prompt: <span style="color:#747ee8">./prim</span> depois digite sua entrada de acordo com a configuração acima.

### Executando com o arquivo de entrada :
---
&nbsp;&nbsp;&nbsp;Para executar o algoritmo Prim com a entrada do arquivo de exemplo, siga as etapas acima, mas na chamada do arquivo bin, digite <span style="color:#747ee8">./prim < nome do arquivo de entrda</span>, para a nossa entrada usamos o nome: <span style="color:#747ee8">./prim < primInput</span>.

### Output example :
---
&nbsp;&nbsp;&nbsp;A saida do algoritmo Prim algoritmo é uma mensagem que mostra o resultado do algoritmo aplicado para cada aresta como ponto inicial e em seguida o peso das arestas formadas pelo algoritmo.<br>
```
Começando do vértice x : y
.
.
.
.
...
total: z
```

