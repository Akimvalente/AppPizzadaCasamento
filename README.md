# 🍕 Sistema de Gestão de Recibos e Entregas - Pizzada

[Acessar aqui] (https://script.google.com/macros/s/AKfycbz1c3yDQCMHQ4fdDhVzf7gW280IG2ce9HnBM_u8dBlpatk94CwRIoDNj7hU_AZ-DBhrtg/exec)

Uma aplicação web leve e responsiva desenvolvida em **Google Apps Script** (HTML/JS/CSS) integrada diretamente com o **Google Planilhas**. O sistema consolida pedidos agrupados por comprador/telefone, gera recibos térmicos para impressão e realiza o controle do fluxo de entregas em tempo real.

---

## 🚀 Funcionalidades

- **Agrupamento Inteligente:** Consolida automaticamente múltiplos itens/pizzas comprados pela mesma pessoa em um único registro.
- **Busca Global Instantânea:** Pesquisa em tempo real por **Nome do Comprador**, **Código do Pedido** ou **Telefone**.
- **Indicadores Visuais por Status:**
  - ⬜ **Pendente:** Cartão neutro/branco.
  - 🟦 **Impresso:** Cartão destacado em azul suave.
  - 🟩 **Entregue:** Cartão destacado em verde suave.
- **Filtros e Abas de Navegação:**
  - **Aba "Em Aberto / Impressos":** Exibe a fila de produção ativa com filtros rápidos por status (Todos, Pendentes, Impressos).
  - **Aba "Concluídos (Entregues)":** Mantém a fila principal limpa movendo pedidos entregues para uma aba de histórico.
- **Impressão de Recibos Térmicos:** Layout formatado para impressoras térmicas (58mm / 80mm) com a lista consolidada das pizzas e opção de edição de texto pré-impressão.
- **Sincronização Direta:** Atualização do status diretamente na coluna correspondente da planilha do Google.

---

## 🛠️ Tecnologias Utilizadas

- **Backend:** [Google Apps Script](https://developers.google.com/apps-scrip) (JavaScript)
- **Database:** Google Sheets API (via Google Apps Script)
- **Frontend:** HTML5, CSS3, JavaScript Vanilla
- **Design System:** Responsive CSS / Mobile First

---

## 📂 Estrutura do Projeto

```text
├── Código.gs          # Lógica do servidor (leitura/escrita na planilha e agrupamento)
├── Index.html         # Interface gráfica, estilos CSS e manipuladores DOM
└── README.md          # Documentação do projeto
