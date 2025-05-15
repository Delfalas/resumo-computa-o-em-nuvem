# Resumo Computação em Nuvem
Este repositório contém o resumo das lições aprendidas durante o desenvolvimento do lab na DIO

# ☁️ Conceitos de Computação em Nuvem e Modelo de Custos

## 🔹 Tipos de Nuvem

### 🌐 Nuvem Pública
- Infraestrutura oferecida por provedores externos (ex: AWS, Azure, Google Cloud).
- Compartilhada entre múltiplos usuários (multi-tenant).
- Escalável sob demanda, sem necessidade de investir em hardware.
- Pagamento conforme o uso (pay-as-you-go).

> **Exemplo:** Hospedar um site em servidores da Amazon Web Services.

---

### 🏢 Nuvem Privada
- Infraestrutura dedicada, gerenciada internamente ou por terceiros.
- Recursos exclusivos para uma única organização (single-tenant).
- Maior controle, segurança e customização.
- Mais adequada para setores com requisitos regulatórios rigorosos.

> **Exemplo:** Servidores locais de uma empresa com políticas de segurança estritas.

---

### 🔀 Nuvem Híbrida
- Combinação de nuvem pública e privada.
- Permite mover cargas de trabalho entre ambientes conforme necessidade.
- Flexibilidade, escalabilidade e controle equilibrados.

> **Exemplo:** Processar dados sensíveis internamente e usar a nuvem pública para análises de grandes volumes.

---

## 💰 Modelos de Custo

### 💸 Opex (Operational Expenditure)
- Despesas operacionais recorrentes.
- Pagamento contínuo por serviços e infraestrutura sob demanda.
- Mais comum em ambientes de **nuvem pública** ou **híbrida**.

> **Exemplo:** Pagar mensalmente por servidores na nuvem.

---

### 🏗️ Capex (Capital Expenditure)
- Despesas de capital com aquisição de ativos físicos.
- Investimento inicial alto, com depreciação ao longo do tempo.
- Mais comum em ambientes de **nuvem privada** ou infraestrutura local.

> **Exemplo:** Comprar e manter servidores físicos próprios.

---

## ✅ Comparativo Rápido

| Característica        | Nuvem Pública | Nuvem Privada | Nuvem Híbrida |
|-----------------------|---------------|---------------|----------------|
| **Custo inicial**     | Baixo         | Alto          | Médio          |
| **Escalabilidade**    | Alta          | Limitada      | Alta           |
| **Controle e segurança** | Menor     | Maior         | Médio          |
| **Modelo de custo**   | Opex          | Capex         | Opex/Capex     |

---

## ✅ Benefícios da Computação em Nuvem

A computação em nuvem oferece diversas vantagens estratégicas e operacionais para empresas e desenvolvedores:

- **Alta Disponibilidade**: Recursos e serviços disponíveis 24/7 com redundância geográfica.
- **Escalabilidade**: Capacidade de aumentar ou reduzir recursos conforme a demanda.
- **Elasticidade**: Adaptação automática da infraestrutura ao uso, otimizando custos.
- **Confiabilidade**: Backup, recuperação de desastres e tolerância a falhas.
- **Previsibilidade**: Custos e desempenho previsíveis com base em métricas de uso.
- **Segurança**: Criptografia, controle de acesso, firewalls e atualizações automáticas.
- **Governança**: Políticas, auditorias e conformidade com normas e regulamentações.
- **Gerenciabilidade**: Ferramentas integradas para monitoramento, automação e gerenciamento centralizado.

---

## 💻 Como Criar uma Máquina Virtual na Azure

Siga os passos abaixo para criar uma VM no portal da Microsoft Azure:

1. Acesse o [Portal Azure](https://portal.azure.com).
2. No menu lateral, clique em **"Máquinas Virtuais"**.
3. Clique em **"+ Criar"** e selecione **"Máquina Virtual"**.
4. Preencha os campos obrigatórios:
   - Assinatura e Grupo de Recursos
   - Nome da VM
   - Região (ex: Brazil South)
   - Imagem (ex: Ubuntu 20.04 LTS ou Windows Server)
   - Tamanho da máquina (CPU/RAM)
   - Autenticação (senha ou chave SSH)
5. Configure a porta de entrada (por exemplo, SSH para Linux ou RDP para Windows).
6. Revise e clique em **"Criar"**.
7. Aguarde a implantação e acesse a VM através do IP público fornecido.

---

# 🌩️ Tipos de Serviço em Nuvem

![image-hierarquia-iaas-paas-saas](https://github.com/user-attachments/assets/f169258a-bc96-45c0-a6f0-40a1968b1318)




## ☁️ IaaS (Infrastructure as a Service)
- **O que é:** Fornece infraestrutura de TI básica sob demanda (servidores, redes, armazenamento).
- **Responsabilidade do usuário:** Sistema operacional, aplicativos, dados.
- **Exemplo:** Microsoft Azure VMs, Amazon EC2.

## ☁️ PaaS (Platform as a Service)
- **O que é:** Oferece uma plataforma completa para desenvolvimento, execução e gerenciamento de aplicações sem se preocupar com infraestrutura.
- **Responsabilidade do usuário:** Aplicações e dados.
- **Exemplo:** Azure App Service, Google App Engine.

## ☁️ SaaS (Software as a Service)
- **O que é:** Software pronto para uso, acessado via internet, sem necessidade de instalação ou manutenção.
- **Responsabilidade do usuário:** Uso do software.
- **Exemplo:** Microsoft 365, Google Workspace.


---

# 🛠️ Como Criar uma Instância Gerenciada de SQL no Azure

## 📌 Passos

1. **Acesse o Portal Azure**
   - [https://portal.azure.com](https://portal.azure.com)

2. **Crie um novo recurso**
   - Vá em **"Criar um recurso"** > **"Banco de dados"** > **"Instância Gerenciada de SQL"**

3. **Configuração básica**
   - Nome da instância
   - Região (localização do datacenter)
   - Resource Group
   - Nome DNS personalizado

4. **Configuração de computação e armazenamento**
   - Escolha a camada de serviço (por exemplo: General Purpose ou Business Critical)
   - Selecione número de vCores e tamanho do armazenamento

5. **Segurança e rede**
   - Configure a rede virtual (VNet)
   - Configure regras de firewall e autenticação

6. **Configurações adicionais (opcional)**
   - Backup automático
   - Alta disponibilidade
   - Tags de recurso

7. **Revisar e criar**
   - Verifique todas as configurações
   - Clique em **"Criar"**

8. **Aguardar a implantação**
   - O Azure provisionará a instância (isso pode levar alguns minutos)

## 🔗 Conectando-se à Instância
- Use ferramentas como **Azure Data Studio** ou **SQL Server Management Studio (SSMS)**
- Forneça o **endpoint DNS**, usuário e senha definidos na criação

---

# 🏗️ Componentes de Arquitetura da Azure

## 🌍 Região
- **Definição**: Conjunto de data centers implantados em uma área geográfica específica.
- **Função**: Hospedar recursos e serviços da Azure próximos ao usuário final para menor latência.
- **Exemplos**: `Brazil South`, `East US`, `West Europe`.

## 🌐 Pares de Região
- **Definição**: Duas regiões da mesma área geográfica emparelhadas para fornecer **alta disponibilidade** e **recuperação de desastres**.
- **Características**:
  - Atualizações planejadas são feitas uma de cada vez entre pares.
  - Replicação de dados e failover garantidos entre as regiões.
  - Separação física (em caso de desastres naturais).

## 📦 Grupo de Recursos
- **Definição**: Contêiner lógico que armazena recursos da Azure relacionados (como VMs, bancos de dados, redes).
- **Função**: Gerenciar recursos como uma unidade (implantação, atualização e exclusão em conjunto).
- **Boas práticas**: Agrupar recursos com o mesmo ciclo de vida.

## 🧾 Assinatura da Azure
- **Definição**: Unidade de faturamento e controle de acesso aos serviços da Azure.
- **Função**: 
  - Agrupar recursos com base em limites de cobrança.
  - Atribuir permissões específicas com base em funções (RBAC).
- **Vinculada a um Diretório Azure AD**.

## 🗂️ Grupo de Gerenciamento
- **Definição**: Contêiner hierárquico acima das assinaturas, usado para aplicar políticas, governança e controle de acesso em escala.
- **Função**:
  - Organizar múltiplas assinaturas.
  - Aplicar políticas do Azure Policy ou RBAC de forma centralizada.

---

## 💻 Máquinas Virtuais (VMs)
Máquinas Virtuais são emulações de computadores físicos que rodam sistemas operacionais e aplicativos como se fossem máquinas físicas. No Azure, elas permitem a execução de cargas de trabalho personalizadas com controle total sobre o sistema operacional, armazenamento e redes virtuais.

**Vantagens:**
- Alta flexibilidade e controle
- Suporte a diferentes sistemas operacionais
- Escalabilidade sob demanda

---

## 🖥️ Área de Trabalho Virtual
Área de Trabalho Virtual é um serviço que fornece desktops e aplicativos remotos acessíveis pela internet. Ele permite que múltiplos usuários acessem um ambiente Windows centralizado de forma segura.

**Vantagens:**
- Acesso remoto seguro
- Gerenciamento centralizado
- Redução de custos com infraestrutura física

---

## 🧱 Contêineres
Contêineres são unidades leves e portáteis que empacotam uma aplicação com todas as suas dependências, garantindo que ela funcione de forma consistente em qualquer ambiente. O Azure oferece serviços como o Azure Kubernetes Service (AKS) para orquestração de contêineres.

**Vantagens:**
- Inicialização rápida
- Portabilidade entre ambientes
- Eficiência no uso de recursos

---

## 🧩 Serviços de Aplicativos do Azure
Azure App Services é uma plataforma de hospedagem de aplicativos web, APIs REST e backends móveis. Ele permite que os desenvolvedores implantem rapidamente aplicações sem se preocupar com a infraestrutura.

**Recursos:**
- Suporte a várias linguagens (C#, Java, Python, Node.js, etc.)
- Integração com CI/CD
- Escalabilidade automática

---

# 🌐 Serviços de Rede do Azure

Os **Serviços de Rede do Azure** são componentes fundamentais para conectar, proteger e otimizar a comunicação entre recursos na nuvem e em ambientes locais. Eles fornecem infraestrutura para redes virtuais, roteamento, balanceamento de carga e conectividade híbrida.

---

## 1. Azure Virtual Network (VNet)

É o serviço básico de rede no Azure, permitindo que você crie redes privadas isoladas dentro da nuvem.

**Recursos:**
- Segmentação de redes em sub-redes
- Controle de tráfego com grupos de segurança de rede (NSG)
- Integração com outros serviços (VMs, bancos de dados, gateways)

---

## 2. Azure VPN Gateway

Permite a criação de túneis criptografados entre sua rede local e a rede virtual do Azure, usando protocolos como IPsec e IKE.

**Tipos:**
- **Site-to-Site (S2S):** Conecta redes locais inteiras ao Azure.
- **Point-to-Site (P2S):** Conecta dispositivos individuais ao Azure.
- **VNet-to-VNet:** Conecta diferentes VNets entre si.

**Vantagens:**
- Comunicação segura
- Custo mais acessível que conexões físicas
- Flexível para empresas com redes distribuídas

---

## 3. Azure ExpressRoute

Permite criar conexões privadas e de alta performance entre o Azure e data centers locais, sem passar pela internet pública.

**Características:**
- Alta largura de banda (até 100 Gbps)
- Baixa latência e maior confiabilidade
- Mais seguro que conexões baseadas em internet

**Casos de uso:**
- Aplicações críticas que exigem desempenho elevado
- Conformidade com requisitos regulatórios de dados
- Backup e replicação de grandes volumes

---

## 4. Azure DNS

Serviço de hospedagem de DNS que permite gerenciar nomes de domínio usando a infraestrutura do Azure.

**Benefícios:**
- Alta disponibilidade e desempenho global
- Integração com outros serviços do Azure
- Suporte a registros DNS padrão (A, AAAA, CNAME, MX, etc.)

**Usos comuns:**
- Resolver nomes de domínio para aplicativos hospedados no Azure
- Gerenciar zonas DNS públicas e privadas

---
