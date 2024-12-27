# resumo-do-lab
## Este repositório contém o resumo das lições aprendidas durante o desenvolvimento do lab na DIO

Aprendi até o momento sobre:

- O que é a nuvem?
É a tecnologia utilizada para armazenar dados em servidores remotos, que podem ser acessados de qualquer lugar com a utilização da internet

- Quais são os tipos de nuvem?
1. Nuvem Privada, ou como conhecida a Intranet, nesse tipo de nuvem a empresa tem seu próprio servidor, onde ficam armazenadas as informações e elas só são acessadas naquela rede.
2. Nuvem Pública, nesse tipo de serviço um servidor remoto é utilizado, muitas vezes de grandes players do mercado como Microsoft, Google e Amazon, basicamente a internet como conhecemos é armazenada nesses servidores e por isso pode ser acessada de qualquer dispositivo com conexão
3. Nuvem Híbrida, pegando o melhor dos dois mundos, as nuvens híbridas são capazes de fazer combos entre a nuvem pública e a nuvem privada, os servidores locais e remotos são capazes de se comunicar nesse formato e é o que da sentido a modalidade
4. MultCloud, conceito não abordado no curso, mas pesquisando entendi que é a utilização de vários desses serviços de servidores e que também podem se comunicar.

- Qual a diferença entre CapEx e OpEx?
CapEx são gastos com investimentos com longo prazo, geralmente para comprar, melhorar um equipamento, os benefícios duram mais, pois uma vez comprado dura por anos, porém o investimento inicial é maior
OpEx são os gastos com a operação da empresa, como o custo para manter um servidor em nuvem, contas de energia, salários, os investimentos iniciais são baixos mas recorrentes.

- SLA, ou tempo de disponibilidade, é o quanto o aquele produto vai ficar fora do ar
Os SLA's são: 99%, 99,9%, 99,95%, 99,99% e 99,999%

- Benefícios da nuvem
Existem diversos benefícios da nuvem que foram citados, alguns deles são: Alta Disponibilidade, Elasticidade, Gerenciamento, Escalabilidade, entre outros.

- IaaS, PaaS, SaaS
Modelo Iaas é a Infraestrutura como serviço, é o modelo que permite maior controle sobre personalizações, o mais caro e mais trabalhoso, exemplos são: banco de dados, firewall, servidores.
Modelos PaaS é Plataforma como serviço, esse modelo é mediano sobre valores, personalizações, além de abranger os tópicos da infraestrutura, o modelo plataforma também abrange Sistemas Operacionais e ferrametas de gerenciamento
Modelo SaaS é o menos volátil, se baseia em serviços por assinaturas, são softwares prontos.

- Zonas de Região
Aprendi que uma região é composto de 3 ou mais datacenters, que existem as zonas pares de desastre recovery, que no Brasil temos apenas um datacenter localizado em São Paulo e quem tem como desaster recovery a zona dos Estados Unidos, as zonas de desaster recovery podem ficar no mínimo a 300 milhas de distancia uma da outra.

- Grupo de recursos
No Lab foi criado um grupo de recursos onde nele iniciamos uma rede virtual, o arquivo Json encontra-se upado em "ip.json"

- Computação e rede
Foi passado conceitos de criação de VM's, conjuntos que disponibilidade e domínio de falha que são basicamente a quantidade de VM's que serão distribuídas nos racks de um datacenter, quanto mais máquinas maior o SLA,
Conceitos da area de trabalho virtual do Azure, que são idênticas as nossas máquinas convencionais porém armazenadas em nuvem, existem diversos benefícios como a escalabilidade (onde você pode aumentar os recursos daquela máquina conforme necessário e sem requerer um grande investimento inicial), outro benefício é que com apenas 1 VM em uma area de trabalho você pode fazer um pool de computadores e assim ter várias pessoas utilizando a mesma VM sem que uma saiba da outra (isso ajuda a controlar gastos), a flexibilidade de acesso, visto que é uma máquina virtual, você consegue acessa-la de qualquer computador (lógico, tendo a sua autenticação)


- Azure functions
São pequenos trechos de códigos que são reproduzidos em resposta a eventos ocorridos na aplicação.

- Migrations
A Microsoft oferece diversas formas de migrações para nuvem, dentre elas existem a AzCopy e Gerenciador de Armazenamento do Azure (que são utilizados para uma quantidade de arquivos menos cargosa, essas duas formas são basicamente a mesma coisa, porém a AzCopy é efetuada por linha de comando e o Gerenciador de Armazenamento do Azure é através de uma Interface Gráfica, que é mais simpática a iniciantes.
Temos também 3 opcões de databox para uma quantidade maior de dados, são elas:
  1. Azure DataBox Disk - Para até 35TB de dados
  2. Azure DataBox - Para até 80TB de dados
  3. Azure DataBox Heavy - Para até 800TB de dados

- Camadas de Acesso
Existem algumas camadas de acesso que podem ser configuradas para obter melhores resultados em nossos trabalhos, são elas:
  1. Frequente (para arquivos que você acessa com frequência, terá um custo maior para criação e um valor menor para consulta)
  2. Esporádico (para arquivos que vocÊ acessa com pouca frequência e armazenados até 30 dias)
  3. Frio (para arquivos que você acessa com pouca frequência e armazenados em até 90 dias)
  4. Arquivo Morto (para arquivos acessados raramente e armazenados em até 180 dias)

- Redundância
Existem 4 principais opções de redundância, são elas:
  1. LRS (faz 3 cópias em um único datacenter)
  2. ZRS (faz 3 cópias, porém cada uma delas estará em um datacenter)
  3. GRS (faz 3 cópias no datacenter da região primária e outra cópia na região par)
  4. GZRS (faz 3 cópias, uma em cada um dos datacenters da região primária e uma outra cópia em um datacenter na região par)

  
