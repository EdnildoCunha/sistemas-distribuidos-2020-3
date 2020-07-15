# sistemas-distribuidos-2020-3
Disciplina de férias EAD de Sistemas Distribuído. 2020-3. UFMA
## Tipos de Sistemas Distribuídos
### Sistemas de Computação Distribuídos
Esses sistemas têm foco em computação de alto desempenho.
Dentre esses sistemas temos:


Cluesters (que são aglomerados de computadores) que estão ligados compartilhando dados e processamento para realizar uma tarefa de alto desempenho.
São essencialmente sistemas conectados através de uma LAN.São geralmente sistemas homogêneos (hardware, SO idênticos ou muito similares).
Possui um um único nó de gerenciamento, uma máquina que coordena as tarefas.


Existem diversos tipos de sistemas distribuídos como a computação em Grade, que é um sistema oportunistas que pega diversos sistemas hetorogêneos de computadores 
ociosos para realizar o processamento de uma tarefa. Estes podem ser dispersos através de várias organizações e podem compreender uma grande área(wide-area) por
WiFi, o que permite diversas organizações virtuais.

### Sistemas de Informação Distribuídos

Arquitetura distribuída para integrar bases de dados com informações relevantes para uma finalidade.
Muitos sistemas utilizam essa arquitetura distribuída seja para manter replicação dos dados por conta
da segurança ou por conta da disponibilidade entre outros aspectos parte desses sistemas distribuídos 
em uso integram sistemas legados atualmente.
Dá-se destaque ultimamente à sistemas de processamento de transações que realizam trasações de qualquer
espécie.


<b>As características desse sistema são:</b>


* _Atomicidade:_ todas as operações serão bem sucedidas ou apresentarão falha;
* _Consistência:_ a transação não viola invariantes do sistema (exemplo: lei 
da conservação do dinheiro em transferências bancárias);
* _Isolamento:_ transações concorrentes não interferem umas com as outras: o resultado final para cada uma
delas se apresentará como se todas as transações fossem executadas em sequência em uma certa ordem;
* _Durabilidade:_ uma vez confirmada a transação confirmada está é permanente.


<b>Sistemas Distribuídos Pervasivos</b>
Muito comum atualmente, recente e surgiu através da computação móvel e pervasiva.


Requisitos diferenciados:
* Ciência de contexto;
* Heterogeneidade de rede e de dispositivos;
* Uso de baterias;
* Interface com o usuário;
* Problemas com segurança.


### Middleware 
Middleware é uma camada intermediária de serviços que está entre o SO e as aplicações distribuídas. Estas aplicações podem pegar recursos dessas middlewares que fornecem diversos serviços sem que
precise acessar APIs de mais baixos níveis.


<b>Alguns casos comuns de uso de middleware no desenvolvimento moderno.</b>

* Desenvolvimento de novas aplicações:


O middleware viabiliza o uso de ambientes de execução modernos e populares em uma ampla gama de
casos de uso. Desenvolvedores e arquitetos podem trabalhar com agilidade em diferentes plataformas, 
seguindo conjuntos de ambientes de execução, frameworks e linguagens de programação fundamentais.
Além disso, o middleware oferece funcionalidades comumente utilizadas, como servidores web, servidor
de SSO, sistema de mensageria e armazenamento em cache em memória;
* Otimização das aplicações existentes:


Com o middleware, os desenvolvedores podem transformar aplicações monolíticas legadas em aplicações
nativas em nuvem com mais facilidade, conferindo mais desempenho e portabilidade a ferramentas
valiosas;
* Integração abrangente:


As ferramentas de integração de middleware conectam sistemas internos e externos críticos. 
Os recursos de integração, como de transformação, conectividade, composibilidade e mensageria
corporativa, combinados à autenticação por SSO tornam mais fácil para os desenvolvedores estender
os recursos do sistema a aplicações diferentes;
* Interfaces de programação de aplicações (APIs):


Muitos serviços de middleware podem ser acessados por meio de APIs, que são conjuntos de ferramentas,
definições e protocolos para que as aplicações se comuniquem entre si. Com as APIs, é possível 
conectar completamente produtos e serviços diferentes usando uma camada comum.
* Transmissão de dados:


Além das APIs, outra abordagem para compartilhar dados entre aplicações é a transmissão de dados 
assíncrona. O conjunto de dados é replicado em um repositório intermediário, onde os dados podem 
ser compartilhados entre várias aplicações. Uma ferramenta de middleware popular open source para 
transmissão de dados em tempo real é o Apache Kafka.
* Automação corporativa inteligente:


Com o middleware, desenvolvedores, arquitetos, profissionais de TI e líderes de negócios podem 
automatizar decisões manuais. A automação também ajuda a aprimorar o gerenciamento de recursos 
e aumentar a eficiência em geral.
