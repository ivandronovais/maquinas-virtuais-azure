# Desafio: Criando Máquinas Virtuais na Microsoft Azure

Este repositório documenta minha jornada de aprendizado e os passos práticos realizados durante o desafio "Criando Máquinas Virtuais na Azure", proposto pela DIO. O objetivo é consolidar os conhecimentos adquiridos, servindo como um guia de referência para futuras consultas e implementações na plataforma Azure.

## Sobre o Desafio

O laboratório prático focou no processo de criação e configuração de uma Máquina Virtual (VM) no Microsoft Azure. Este `README.md`, juntamente com quaisquer outros artefatos neste repositório, visa registrar os resumos, anotações e dicas relevantes sobre o uso do Azure, especialmente no que tange a VMs, mas também abrangendo conceitos fundamentais da nuvem.

## Objetivos de Aprendizagem Cumpridos

* Aplicação prática dos conceitos de computação em nuvem e serviços Azure.
* Documentação estruturada de processos técnicos.
* Utilização do GitHub para versionamento e compartilhamento de documentação técnica.

## Resumo dos Aprendizados

Minha experiência neste lab me permitiu aprofundar nos seguintes tópicos:

### 1. Conceitos Fundamentais da Computação em Nuvem e Azure

Antes de iniciar a criação da VM, foi essencial revisar e compreender:

* **Categorização de Serviços no Azure:** Aprendi a localizar e entender a organização dos diversos serviços oferecidos pela Azure através do portal, facilitando a identificação das ferramentas necessárias para cada demanda.
* **Modelos de Nuvem:** Relembrei as diferenças e casos de uso para IaaS (Infraestrutura como Serviço), PaaS (Plataforma como Serviço) e SaaS (Software como Serviço). A criação de VMs se encaixa predominantemente no modelo IaaS.
* **CapEx vs. OpEx:** Entendi a transição de despesas de capital (investimento em infraestrutura física) para despesas operacionais (pagamento pelo uso de serviços em nuvem) e como isso impacta a estratégia de TI.
* **SLA (Service Level Agreement):** Compreendi a importância dos Acordos de Nível de Serviço, que definem as garantias de tempo de atividade e desempenho para os serviços Azure, incluindo VMs.
* **Elasticidade:** Percebi como a nuvem permite adaptar recursos (como os de uma VM) dinamicamente para atender a variações de demanda, garantindo agilidade.
* **Gerenciabilidade:** Explorei como o Portal Azure e as ferramentas de linha de comando (como Azure CLI ou PowerShell) facilitam o gerenciamento centralizado e remoto dos recursos na nuvem.
* **Alta Disponibilidade e Confiabilidade:** Conceitos importantes que garantem a continuidade e a robustez das aplicações hospedadas na nuvem.

### 2. Criação e Configuração de Máquina Virtual (VM) no Azure

O foco prático do laboratório foi a criação de uma VM, envolvendo os seguintes passos e considerações principais:

* **Planejamento da VM:**
    * **Escolha do Sistema Operacional:** Seleção da imagem do SO (ex: Windows Server, Linux - Ubuntu, CentOS, etc.) adequada à necessidade.
    * **Dimensionamento (Tamanho da VM):** Escolha da série e tamanho da VM (ex: Séries B, D, E) com base nos requisitos de CPU, RAM e IOPS. Compreensão das implicações de custo.
    * **Região:** Seleção da região do Azure para hospedar a VM, considerando latência para os usuários e conformidade.
* **Configurações Iniciais no Portal Azure:**
    * Nome da VM, grupo de recursos, credenciais de administrador (usuário/senha ou chave SSH para Linux).
    * Licenciamento (ex: Benefício Híbrido do Azure para Windows Server).
* **Configurações de Rede:**
    * **Rede Virtual (VNet):** Criação ou seleção de uma VNet e sub-rede para isolamento e comunicação.
    * **Endereço IP Público:** Configuração de um IP público para acesso externo (se necessário).
    * **Grupo de Segurança de Rede (NSG):** Definição de regras de entrada e saída para controlar o tráfego da VM (ex: liberar porta RDP/3389 para Windows ou SSH/22 para Linux).
* **Configurações de Disco:**
    * **Disco do SO:** Configuração do tipo de disco (HDD Standard, SSD Standard, SSD Premium).
    * **Discos de Dados (Opcional):** Adição e configuração de discos de dados para armazenamento adicional.
* **Gerenciamento e Monitoramento (Básico):**
    * Visão geral das opções de monitoramento (métricas de CPU, rede, disco).
    * Opções de backup e recuperação de desastres (introdução).
* **Conexão com a VM:**
    * Para Windows: via RDP (Remote Desktop Protocol).
    * Para Linux: via SSH (Secure Shell).

### 3. Uso do GitHub para Documentação

* Criação de um repositório público para armazenar o `README.md` e outros artefatos do projeto.
* Utilização de Markdown para formatação clara e estruturada do conteúdo.
* Importância do versionamento para manter um histórico das evoluções da documentação.

## Dicas e Anotações sobre o Uso do Azure

* **Grupos de Recursos:** Sempre organize seus recursos em Grupos de Recursos para facilitar o gerenciamento, o controle de custos e a limpeza do ambiente.
* **Nomenclatura:** Adote uma convenção de nomenclatura clara para seus recursos no Azure. Isso facilita a identificação e a administração.
* **Azure Cost Management:** Explore as ferramentas de gerenciamento de custos do Azure para monitorar e otimizar seus gastos desde o início.
* **Documentação Oficial da Microsoft:** É uma fonte indispensável e sempre atualizada para aprender sobre os serviços e melhores práticas do Azure.
* **Azure CLI e PowerShell:** Para automação e gerenciamento avançado, invista tempo em aprender essas ferramentas de linha de comando.
* **Segurança:** Sempre revise as configurações de NSG e aplique o princípio do menor privilégio ao configurar o acesso às suas VMs. Considere o uso do Azure Security Center para recomendações.

## Conclusão

Este desafio proporcionou uma experiência prática valiosa na criação e configuração de Máquinas Virtuais no Azure, além de reforçar conceitos essenciais da computação em nuvem. A documentação deste processo no GitHub não apenas cumpre os requisitos do desafio, mas também cria um recurso útil para referência futura.
