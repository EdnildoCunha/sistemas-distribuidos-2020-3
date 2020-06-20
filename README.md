# sistemas-distribuidos-2020-3
Disciplina de férias EAD de Sistemas Distribuído. 2020-3. UFMA


# Sistemas Distribuídos atv-s01e03
## Características de um Sistema Distribuído
### Definição de um Sistema Distribuído:
Tanenbaum(2007) descreve um sistema distribuído como __"Coleção de computadores independentes que se apresenta ao usuário
como um sistema único e coerente"__. Essa definição nos dá a idéia de que esse sistema trabalha com computadores
autônomo que dividem recursos entre si, dando ao usuário a impressão de que se trata de um sistema único e coeso sem aparentar
a divisão desses recursos em diferentes máquinas.

### Objetivos de um Sistema Distribuído
Os objetivos desse tipo de sistema são:
* Compartilhamento de recursos


Tal qual a definição esse objetivo nos permite compartilhar os recursos de diferentes máquinas em diferentes locais seja
processamento, dados, armazenamento, funções e etc... isso nos permite expandir a capacidade do que uma máquina permitiria realizar.
* Transparência de distribuição


Essa transparência torna imperceptível, ao software ou ao usuário, de onde está sendo tirado o recurso utilizado, dando uma idéia de 
unidade à máquina utilizada, assim o sistema consegue ser integrado durante o uso apesar de estar dividido em diferentes componentes.
* Abertura


Esta relacionado às regras de sintaxe e semântica que padronizarão estes sistemas.


_exemplo: em redes de computadores existem padrões que governam o formato, o significado e o conteúdo de mensagens enviadas e recebidas._


No caso de sist. distribuídos os serviços são especificados por meio de uma linguagem de definição de interface
__IDLs(Interface Definition Language)__
* Interoperabilidade


Define como as implementações do sistema conseguem coexistir e trabalhar em conjunto, como os componentes conseguem operar
os recursos do sistema agindo com as especificações de um padrão comum.
* Portabilidade


A portabilidade define como e até que ponto de acesso um sistema distribuído A pode ser executado, com as mesmas funcionalidades, em um
diferente sistema B.
* Extensibilidade(Escalabilidade)


A extensibilidade dita a capacidade desse sistema expandir adicionando ou substituíndo componentes sem afetar as funções do sistema e os compenentes que permanecem no lugar.
Como _exemplo temos um banco de dados que dá acesso aos recursos de um site, com este quesito você pode substituir componentes, desligar componentes
e não perder o acesso aos recursos desse banco._
### Técnicas de Escalabilidade
A escalabilidade é uma importante meta na hora de se considerar um sistema distribuído graças à globalização da conectividade da internet.


A Escalabilidade de um sistema pode ser medida segundo três dimensões, em relação ao tamanho, que dita a facilidade de se adicionar usuários e recursos ao sistema, em relação
à geografia, que dita o quão longe os recursos e usuários podem estar e em termos administrativos que dita a facilidade de gerenciamento. Infelizmente um sistema escalável em 
alguma dessas dimensões pode representar perda na capacidade de desempenho à medida em que é ampliado.


Para melhorar o processo de escalabilidade para o usuário, existem algumas técnicas utilizadas, entre elas:


* Esconder a latência (requisição assíncrona): Para esconder esta latência muitas vezes pode-se trazer para o dispositivo final
o processamento de determinada requisição assim ele não precisa buscar em um servidor externo dando a impressão de agilidade 
para o software, como por _exemplo: Validação de CPF feita diretamente na máquina do usuário e não buscando de um banco de dados online._


* Distribuição: Neste quesito temos a forma como um sistema esta distribuído na rede podendo estar em um servidor mais próximo ou mais longe
do usuário o que impacta diretamente na velocidade a qual um recurso pode ser utilizado. Como _exemplo temos o o Sistema de Nomes de Domínio, __DNS (Domain Name System)__,
que dita a partir das terminações de um URL em que zona aquele recurso está diminuindo a distância ao qual o sistema procurará o servidor correspondente._


* Replicação: Este quesito dita uma característica bem importante do sistema distribuído que é a replicação deste sistema, isso funciona tanto para a segurança, evitando perda de dados por
danos físicos ou problemas no software, quanto diminui a velocidade em que um arquivo é carregado ao ser requisitado, este último é comumente percebido com a técnica de caching onde
uma figura, um dado, um arquivo, que é esperado ser utilizado mais de uma vez, é carregado na máquina do usuário assim quando ele acessar este recurso uma próxima vez, ele estará sendo 
acionado de maneira mais rápida. O maior problema deste quesito é quanto à consistência pois como o sistema é replicado em diferentes máquinas, alguma falha de atualização do sistema geral
como falta de internet pode trazer inconsistência nos dados apresentados em ambos os componentes do sistema distribuído.
## Referências
* TANENBAUM, Andrew S.; VAN STEEN, Maarten. Sistemas distribuídos: Princípios e paradigmas, 2 ed. São Paulo: Prentice Hall, 2007,cap 1, pag. 1- 9.
* LOPES, Rafael Fernandes. S01E01 - Caracterização de Sistemas Distribuídos. 2020. (17:04). Disponível em: < https://www.youtube.com/watch?v=cWw4wGQdXn0>. Acesso em: 19 jun. 2020
