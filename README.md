# ☁️ Resumo do Lab: Armazenamento Microsoft Azure AZ-900
Este repositório reúne os principais aprendizados adquiridos durante o laboratório de **Armazenamento na Azure** da plataforma [DIO.me](https://web.dio.me), Módulo 2, do qual estou atualmente participando. O foco está nos benefícios e aplicações práticas da plataforma Microsoft Azure, explorando seus recursos e funcionalidades. O Bootcamp oferece uma base sólida em tecnologias de nuvem, abordando desde os conceitos fundamentais até os componentes essenciais da arquitetura Azure.
Entre os temas estudados estão: criação e gerenciamento de máquinas virtuais, configuração de bancos de dados e soluções de armazenamento, além de tópicos avançados como arquitetura em nuvem, governança, monitoramento e segurança de ambientes cloud.

---

## 📘 Tópicos Abordados
Este repositório contém resumos e referencias sobre o curso armazenamento, serviços e migração da plataforma Microsoft Azure. 
Este material serve como referência para estudos e para a criação de ambientes em nuvem de forma organizada e escalável.

## 📦 Armazenamento no Azure

### 🔁 Redundância e Serviços de Armazenamento

A redundância no armazenamento de dados é um conceito fundamental para garantir a disponibilidade e a durabilidade dos seus arquivos. Ela se refere à prática de criar e manter múltiplas cópias dos seus dados em locais fisicamente separados. O objetivo é proteger os dados contra falhas de hardware, desastres naturais ou interrupções inesperadas, assegurando que, se uma cópia for perdida, outras ainda estarão acessíveis.

No Azure, a redundância é implementada em diferentes níveis, oferecendo opções como:

- **LRS (Locally Redundant Storage):** mantém várias cópias dos dados dentro de um único data center. É a opção mais econômica, mas oferece menos proteção.
- **ZRS (Zone-Redundant Storage):** mantém cópias dos dados em diferentes zonas de disponibilidade dentro de uma mesma região do Azure, protegendo contra falhas em um data center específico.
- **GRS (Geo-Redundant Storage):** mantém cópias dos dados em uma região secundária do Azure, a centenas de quilômetros de distância. Assim, oferece a maior proteção contra desastres regionais.
- **GZRS (Armazenamento Redundante de Zona Geográfica):** combina o ZRS e o GRS, distribuindo os dados em zonas de disponibilidade e também em uma região secundária.
- **Serviços:** Blob Storage (arquivos não estruturados), File Storage (sistema de arquivos compartilhado), Queue Storage (mensageria), Table (dados NoSQL).

---

### 🌐 Pontos de Extremidade Públicos e Camadas de Acesso

- **Públicos:** um ponto de extremidade público é um endereço de rede acessível pela internet que permite a comunicação com um serviço do Azure, como uma conta de armazenamento. Ele funciona como uma porta de entrada para os seus dados. Para o armazenamento de arquivos, o Azure oferece pontos de extremidade públicos para acessar os seus dados de qualquer lugar, desde que tenha as devidas permissões e chaves de acesso.

**🌦️Camadas de Acesso:** as camadas de acesso permitem que se otimize os custos do armazenamento de acordo com a frequência de uso dos dados. No Azure, as principais camadas são:

- **Camada de acesso frequente (Hot):** ideal para dados que são acessados com frequência. O custo de armazenamento é mais alto, porém o custo de acesso é baixo.
- **Camada de acesso esporádico (Cool):** ideal para dados que são acessados com pouca frequência (pelo menos uma vez por mês). O custo de armazenamento é menor do que a camada Hot, mas o custo de acesso é mais alto.
- **Camada de arquivamento (Archive):** ideal para dados que são raramente acessados e que podem tolerar um tempo de recuperação maior. É a opção mais econômica para armazenamento de longo prazo.

---

### 🔖 Migração para o Azure e Opções de Gerenciamento de Arquivos

**Migração:** Migrar arquivos para o Azure pode ser um processo simples ou complexo, dependendo do volume de dados, do tipo de arquivos e dos requisitos do seu negócio. O Azure oferece diversas ferramentas para nos ajudar nesse processo, como:

- **Azure Storage Mover:** ajuda a migrar dados de servidores de arquivos e sistemas de armazenamento de terceiros para o Azure.
- **Azure Data Box:** um serviço físico que ajuda a migrar grandes volumes de dados para a nuvem.

**Opções de Gerenciamento de Arquivos:** Após a migração, o Azure oferece diversas opções para você gerenciar seus arquivos na nuvem:

- **Azure Files:** permite criar compartilhamentos de arquivos que podem ser acessados usando o protocolo SMB (Server Message Block) padrão. Isso significa que podemos montar compartilhamentos de arquivos do Azure em máquinas Windows, Linux e macOS.
- **Azure Blob Storage:** ideal para armazenar grandes quantidades de dados não estruturados, como imagens, vídeos, documentos e backups.
- **Azure NetApp Files:** um serviço de armazenamento de arquivos de alto desempenho para cargas de trabalho de missão crítica, como bancos de dados, aplicações empresariais e sistemas de design e engenharia.

---

### 🚀 Migração para o Azure

**Ferramentas:**

- Azure Migrate: avalia e migra cargas de trabalho.
- AzCopy: copia dados para o Azure.
- Storage Migration Service: migração de arquivos locais para File Storage.

### 🗂️ Opções de Gerenciamento de Arquivos

- Azure File Sync: sincroniza servidores locais com File Storage.
- Azure Storage Explorer: gerencia dados via interface gráfica.
- RBAC (Role-Based Access Control): controle de acesso por função.
- Políticas de ciclo de vida: automatizam movimentação entre camadas.

---
## ✅ Conclusão

O armazenamento na nuvem com Microsoft Azure representa uma solução robusta, escalável e segura para empresas e profissionais que buscam modernizar sua infraestrutura digital.
Ao oferecer múltiplas opções de redundância, camadas de acesso e ferramentas de migração, o Azure permite que os dados sejam protegidos contra falhas, otimizados conforme o uso e facilmente integrados aos sistemas existentes.
Além disso, os serviços como Blob Storage, File Storage e Azure NetApp Files atendem a diferentes necessidades — desde o arquivamento de grandes volumes de dados não estruturados até o suporte a aplicações críticas de alto desempenho. 
A gestão eficiente é garantida por ferramentas como Azure Storage Explorer, Azure File Sync e políticas automatizadas de ciclo de vida, que facilitam o controle e a organização dos dados.
Dominar esses recursos é essencial para quem deseja construir ambientes em nuvem resilientes e preparados para o futuro. O conhecimento adquirido neste laboratório serve como base sólida para projetos reais, certificações profissionais e decisões estratégicas em tecnologia.

> Este conteúdo faz parte do projeto **Armazenamento na Azure - Laboratório** da plataforma [DIO.me](https://web.dio.me).

---
 
### 📚 Recursos Complementares
- [Usar o Gerenciador de Armazenamento do Azure](https://learn.microsoft.com/pt-br/azure/storage/blobs/quickstart-storage-explorer)
- [Visão geral da conta de armazenamento](https://learn.microsoft.com/pt-br/azure/storage/common/storage-account-overview?toc=%2Fazure%2Fstorage%2Fblobs%2Ftoc.json&bc=%2Fazure%2Fstorage%2Fblobs%2Fbreadcrumb%2Ftoc.json)
- [Introdução ao AzCopy](https://learn.microsoft.com/pt-br/azure/storage/common/storage-use-azcopy-v10?toc=%2Fazure%2Fstorage%2Ffiles%2Ftoc.json&tabs=dnf)
- [Migre cargas de trabalho](https://azure.microsoft.com/pt-br/pricing/purchase-options/azure-account?icid=azure-migrate#tabs-pill-bar-ocea03_tab4)
- [O que são as Migrações para Azure?](https://learn.microsoft.com/pt-br/azure/migrate/migrate-services-overview?view=migrate-classic)
- [Sincronização de Arquivos do Azure e Azure Data Box](https://learn.microsoft.com/pt-br/azure/storage/files/storage-files-migration-server-hybrid-databox)
- [Gerenciador de Armazenamento](https://azure.microsoft.com/pt-br/products/storage/storage-explorer/?msockid=0a879c916bf366861df88afa6a98670a)
- [Calculadora de Preços Azure](https://azure.microsoft.com/pt-br/pricing/calculator/?ef_id=_k_EAIaIQobChMI14z7o_fWjwMVc0FIAB3PYQApEAAYASACEgLE-fD_BwE_k_&OCID=AIDcmmzmnb0182_SEM__k_EAIaIQobChMI14z7o_fWjwMVc0FIAB3PYQApEAAYASACEgLE-fD_BwE_k_&gad_source=1&gad_campaignid=1635078708&gbraid=0AAAAADcJh_s0nlhmSLvv4COb6oAkGNm0s&gclid=EAIaIQobChMI14z7o_fWjwMVc0FIAB3PYQApEAAYASACEgLE-fD_BwE)
- [Assinatura do Azure](https://learn.microsoft.com/pt-br/azure/azure-resource-manager/management/azure-subscription-service-limits)
  
📎 Link do curso: [Microsoft Azure AZ-900 - DIO.me](https://web.dio.me/lab/computacao-da-nuvem-laboratorio/learning/6d6083cf-0291-428d-a5f2-c93166e6874d)
