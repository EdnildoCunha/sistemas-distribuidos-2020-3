# sistemas-distribuidos-2020-3
Disciplina de férias EAD de Sistemas Distribuído. 2020-3. UFMA
## Classificação de Hardwares com várias CPUs

A criação de arquiteturas paralelas se deu com a necessidade de aumentar o desempenho das máquinas.

### Classificação quanto ao nível de compartilhamento de memória

Observa-se tipo de computadores de acordo com o formato do barramento e também o nível de 
compartilhamento da memória (Conceito de espaço de enderaçamento - Sist Op), Sistemas Multiprocessados.

* Multicomputadores: cada processador possui sua própria memória local.
* Multiprocessadores: os processadores compartilham memória.

### Sistemas Baseados em Barramento
* Sistema com barramento onde os vários processadores acessam diversos memórias(memória compartilhada).
Melhora o acesso a dados compartilhados entre diferentes processos. Problema do Gargalo de Von Neumann
um único barramento de acesso sendo bloqueado por vários processadores, faz com que a taxa de 
transmissão do processador que está executando um programa e a 
memória tenha a a velocidade limitada pelo barramento, Agravamento contenção de barramento.

* Sistema com barramenta com memória privada onde cada processador tem acesso à sua própria
memória. (Contra: Compartilhamento de dados complicado, Pró: Melhor Gerenciamento).

### Sistemas Baseados em comutadores
* Sistema com um comutador que interliga
Memórias(memória compartilhada) Processadores, origina níveis de arquitetura mais complexo
* Sistema de comutador com memórias privadas.

### Em sistemas multiprocessadores
Geralmente tem-se uma memória e várias CPUs, cada CPU possui uma memória cache dentro da CPU
que ajuda a diminuir o acesso à memória principal, aumentando a velocidade do processamento
armazenando instruções e dados mais utilizados. Porém a cache introduz um problema de consistência
uma vez que o cache precisa estar sincronizado com a memória. Barramento limita a escalabilidade.

Com chaveamento temos esquemas de dois ou mais comutadores que permitem arquiteturas mais complexas.

Temos o Cross-bar com barramento cruzado que é um sistema um pouco caro pelo número de chaves
( Para n CPUs são necessários n² pontos de cruzamento), porém que melhora o acesso com a intrudução
de diversos caminhos de acesso do processador às memórias.

Também temos a chamada rede ômega (b) que cria uma malha acesso que minimiza aquele gasto, criando
caminhos que se interligam entre as memórias e processadores com comutadores. Toda CPU pode acessar
qualquer memória, porém pode haver diversos roteamentos entre uma CPU e uma memória.

### Em sistemas multicomputadores
* Multicomputador Homogênio
A ideia de ter dispositivos similares para processamento paralelo. Mensagens roteadas pela rede que
interconecta os processadores. Grande Variedade de máquinas como MPPs (Massively Parallel Processors)
e COW (Cluster of Workstations), como Beowulf.

Dois padrões mais usados são: em Grade e Hipercubo.

* Multicomputador Heterogênio
Juntar diferentes dispositivos com diferentes características heterogêneas como processadores,
tamanho das memórias e largura de banda entrada e saída diferentes. São o tipo mais comum de
multicomputadores
### Taxonomia de Flynn
* SISD: único fluxo de instruções e um único fluxo de dados. Todos os
computadores monoprocessados tradicionais estão nesta categoria;
* SIMD: um único fluxo de instruções e múltiplos fluxos de dados;
* MISD: múltiplo fluxo de instruções e um único fluxo de dados. Nenhuma máquina funciona 
neste modelo;
* MIMD: múltiplo fluxo de instruções e múltiplo fluxo de dados: _Multiprocessadores_ e
_Multicomputadores_
