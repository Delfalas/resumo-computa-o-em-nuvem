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
