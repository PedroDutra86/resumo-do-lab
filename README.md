# Resumo do Lab

## Este repositório contém o resumo das lições aprendidas durante o desenvolvimento do lab na DIO.

### Aprendi até o momento sobre:

#### O que é a nuvem?  
A nuvem é a tecnologia utilizada para armazenar dados em servidores remotos, que podem ser acessados de qualquer lugar com o uso da internet.

#### Quais são os tipos de nuvem?  
1. **Nuvem Privada**:  
   Conhecida como Intranet, nesse tipo de nuvem a empresa tem seu próprio servidor, onde as informações são armazenadas e acessadas exclusivamente dentro da rede interna.  
2. **Nuvem Pública**:  
   Utiliza servidores remotos, frequentemente oferecidos por grandes players do mercado como Microsoft, Google e Amazon. A internet, como conhecemos, está em grande parte armazenada nesses servidores, sendo acessível de qualquer dispositivo conectado.  
3. **Nuvem Híbrida**:  
   Combina características da nuvem pública e privada. Nesse modelo, servidores locais e remotos se comunicam, oferecendo flexibilidade e eficiência.  
4. **MultCloud**:  
   Embora não abordado no curso, é o uso de múltiplos serviços de nuvem que podem interagir entre si.  

#### Qual a diferença entre CapEx e OpEx?  
- **CapEx (Capital Expenditure)**:  
  Gastos com investimentos de longo prazo, geralmente para aquisição ou melhoria de equipamentos. Os benefícios são duradouros, mas o investimento inicial é maior.  
- **OpEx (Operational Expenditure)**:  
  Gastos com a operação diária da empresa, como manutenção de servidores em nuvem, energia elétrica e salários. Esses custos são menores inicialmente, mas recorrentes.  

#### SLA (Service Level Agreement)  
Representa o tempo de disponibilidade de um serviço. Os principais níveis de SLA são:  
- 99%, 99.9%, 99.95%, 99.99% e 99.999%.  

#### Benefícios da nuvem  
Alguns benefícios da nuvem incluem:  
- Alta disponibilidade  
- Elasticidade  
- Gerenciamento simplificado  
- Escalabilidade  

#### IaaS, PaaS, SaaS  
1. **IaaS (Infraestrutura como Serviço)**:  
   Proporciona maior controle e personalização, sendo mais caro e trabalhoso. Exemplos incluem bancos de dados, firewalls e servidores.  
2. **PaaS (Plataforma como Serviço)**:  
   Intermediário em custo e personalização, abrange infraestrutura e sistemas operacionais, além de ferramentas de gerenciamento.  
3. **SaaS (Software como Serviço)**:  
   Baseia-se em assinaturas e oferece softwares prontos, sendo o modelo menos personalizável.  

#### Zonas de Região  
Uma região é composta por 3 ou mais datacenters. No Brasil, há apenas um datacenter (São Paulo), com desastres recuperados na zona dos Estados Unidos. As zonas de recuperação de desastres ficam, no mínimo, a 300 milhas de distância uma da outra.  

#### Grupo de Recursos  
No Lab, foi criado um grupo de recursos no qual iniciamos uma rede virtual. O arquivo JSON encontra-se disponível em `ip.json`.  

#### Computação e Rede  
- Conceitos de criação de VMs, conjuntos de disponibilidade e domínios de falha: quanto mais VMs distribuídas, maior o SLA.  
- Máquinas virtuais armazenadas em nuvem têm benefícios como escalabilidade e flexibilidade de acesso, permitindo uso compartilhado e controle de custos.  

#### Azure Functions  
São pequenos trechos de código que respondem a eventos na aplicação.  

#### Migrações  
Formas de migração para a nuvem:  
1. **AzCopy**:  
   Linha de comando para migração de arquivos menos pesados.  
2. **Gerenciador de Armazenamento do Azure**:  
   Interface gráfica, mais amigável para iniciantes.  
3. **DataBox**:  
   - **Azure DataBox Disk**: Até 35TB.  
   - **Azure DataBox**: Até 80TB.  
   - **Azure DataBox Heavy**: Até 800TB.  

#### Camadas de Acesso  
1. **Frequente**:  
   Para arquivos acessados frequentemente; custo maior para criação, mas menor para consulta.  
2. **Esporádico**:  
   Para arquivos acessados ocasionalmente, armazenados por até 30 dias.  
3. **Frio**:  
   Para arquivos pouco acessados, armazenados por até 90 dias.  
4. **Arquivo Morto**:  
   Para arquivos raramente acessados, armazenados por até 180 dias.  

#### Redundância  
1. **LRS (Local Redundancy Storage)**:  
   Três cópias em um único datacenter.  
2. **ZRS (Zone Redundancy Storage)**:  
   Três cópias em datacenters diferentes.  
3. **GRS (Geo-Redundancy Storage)**:  
   Três cópias no datacenter primário e uma em outra região.  
4. **GZRS (Geo-Zone Redundancy Storage)**:  
   Três cópias em datacenters primários e uma em outra região.  

#### Microsoft Entra ID  
Antigo Azure AD, é responsável pelo controle de permissões de usuários.  

#### Domain Servers  
Sincronizam usuários locais (on-premises) com a nuvem.  

#### Acesso Condicional  
Analisa sinais, como IPs diferentes, para verificar se o usuário está autorizado a acessar determinados dados.  
