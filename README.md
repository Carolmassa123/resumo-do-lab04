# resumo-do-lab04
Este repositório contém o resumo das lições aprendidas durante o desenvolvimento do lab Componentes de Arquitetura no Azure na DIO.

Arquitetura do Azure:
- Regiões e zonas de disponibilidade: arquitetura física do Azure, entender como criar os recursos de nuvem.
- Assinaturas e grupos de recursos: organização de recursos na cloud.
Componentes de arquitetura
- Regiões: onde podemos criar clouds. Quanto mais parto, mais rápido. Nem todos os recursos estão disponíveis em todas as regiões.
* Azure tem mais de 60 regiões.
Regiões têm um ou mais datacenters próximos, isso fornece felixibilidade e escala para reduzir latência (ter alta performance). Regiões preservam a residência dos dados com abrangência de conformidade. São como uma sala com vários armários (zonas de disponibilidades) que possuem várias gavetas (datacenters). 
* LGPD: os dados sensíveis não podem sair do território naional.
- Zonas de disponibilidades: enorme datacenter. Fornece proteção contra tempo de inatividade por falha de datacenter e separa fisicamente os datacenters. Cada datacenter é equipado com alimentação, resfriamento e rede independentes, conectados por redes privadas.
- Pares de regiões: pelo menos 300 milhas de separação entre elas. Região par para caso de falha de região original. A troca pode ser automática. Atualizações são distribuidas para minimizar inatividade. Brasil não replica para dentro do próprio Brasil. Desaster recovery.
Regiões soberanas:
- EUA: segurança e conformidade de agências federais.
Azure governamentais: acessível para autorizados.
- Azure China: primeiro provedor estrangiero de serviços de nuvem pública da China, operada por internet própria (21Vianet). Dados permanecem na China.

- Recursos Azure: armazenamento, máquinas virtuais e redes para soluções de nuvem. Serviços de aplicativos, SQL, funções.
- Grupo de recursos: maneira de organizar as coisas. Web, banco de dados; máquina virtual; armazenamento. Informações podem mudar, mas não podem renomear após criado. Os recursos não precisam estar na mesma região.
Portanto, temos que grupo de rescursos é um CONTÊINER usado para gereciar e agregar recursos em uma unidade. Podem existir em apenas um grupo e podem existir em várias regiões. Recursos podem ser movidos e aplicativos podem usar vários grupos.
- Assinaturas do Azure: desenvolvimento, teste e produção. TOdas podem estar numa mesma conta. É importante que cada grupo de trabalho tenha uma assinatura diferente, para gerenciamento de custos e segurança.
Uma assinatura fornece acesso auteticado e autorizado.
- Limite de cobrança: gere relatórios de cobrança e faturas separados para cada assinatura.
- Limite do controle de acesso: cada um tem apenas o acesso que precisa.

- Hierarquia: Grupos de gerenciamento -> Assinaturas -> grupos de recursos -> recursos
- Grupos de gerenciamento: trabalhar as padronizações de assinaturas, elas herdam as condiões aplcadas ao grupo de gerenciamento.

* Uma conta pode ter várias assinaturas, assinatura responde por uma conta.
* Zonas de disponibilidade permitem a execução de aplicativos em alta disponibilidade e replicação de baixa latência.
