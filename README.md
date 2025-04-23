# 🤖 ERP Assistente no WhatsApp com n8n, Google Sheets e MegaAPI

Este projeto transforma o WhatsApp em um *assistente virtual ERP inteligente*, integrando automações construídas com *n8n*, *Google Sheets* e *MegaAPI* para atendimento personalizado de *clientes e vendedores*.

---

## 🚀 Funcionalidades principais

### 👤 Jornada do Cliente

**1️⃣ Consulta de Pedidos**

O cliente digita *1* no WhatsApp, e o assistente:

- Busca seus pedidos no Google Sheets (aba *pedidos*)
- Formata os dados com número do pedido, valor, status e data
- Envia o resultado de forma clara e amigável

*Exemplo:*

*📦 Seus últimos pedidos:*

*• Pedido #1001 – R$ 1500,00 – Faturado (01/04/2024)*  
*• Pedido #1002 – R$ 2200,00 – Em separação (05/04/2024)*

**2️⃣ Segunda via de Boleto**

- Ao digitar *2*, o cliente recebe os links atualizados dos boletos, baseados na aba *boletos* do Sheets
- Links são enviados no formato clicável via WhatsApp

---

### 🧑‍💼 Jornada do Vendedor

**1️⃣ Consulta de Orçamentos**

O vendedor digita *1* e recebe seus últimos orçamentos registrados, com resumo de cliente, produto, quantidade e valor total

*Exemplo:*

*📑 Seus últimos orçamentos registrados:*  
*• 10/04/2024 – Empresa Alfa – Piso Vinílico x100 = R$ 4.550,00*

**2️⃣ Registro de Novo Orçamento**

- Ao digitar *3*, o assistente solicita um texto no padrão:  
  *Empresa Beta, Piso Laminado, 300, 39.90*
- O sistema valida, formata e grava o orçamento automaticamente na aba *orcamentos*
- Uma mensagem de confirmação é enviada

*Exemplo:*  
*Oi João, seu orçamento foi salvo com sucesso!*  
*Cliente: Empresa Beta*  
*Produto: Piso Laminado*  
*Total: R$ 11.970,00*

---

## 🛠️ Tecnologias Utilizadas

- *n8n* – Automação no-code
- *Google Sheets* – Banco de dados leve e acessível
- *MegaAPI* – Envio e recebimento de mensagens WhatsApp
- Webhook e controle de etapa para continuidade do diálogo

---

## 📁 Estrutura das planilhas

- *usuarios* – Contém dados de login, tipo de usuário e controle de etapa
- *pedidos*, *boletos*, *orcamentos*, *comissoes*, *ocorrencias* – Planilhas vinculadas às funcionalidades

---

## 📌 Casos de uso ideais

- Pequenas e médias empresas que desejam atendimento automatizado no WhatsApp
- Times de vendas, suporte e atendimento
- Apresentação como MVP de automação com IA + cloud
