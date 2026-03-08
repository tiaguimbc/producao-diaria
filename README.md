# 📊 Sistema de Gestão de Produção Diária (PCP)

Este projeto é uma ferramenta de suporte à decisão e controle operacional desenvolvida para otimizar o fluxo de trabalho em ambientes de produção e logística. A aplicação centraliza o rastreamento de equipamentos e a gestão de tickets em uma interface única e intuitiva.

---

### 📋 Visão Geral do Sistema
O sistema foi projetado para resolver a fragmentação de dados de produção, permitindo que as informações de hardware e chamados sejam processadas e sincronizadas de forma estruturada.

* **Gestão de Equipe Dinâmica**: Organização de fluxos de trabalho divididos por colaboradores (Tiago, Alana e William), facilitando o acompanhamento de metas individuais.
* **Rastreamento de Hardware**: Campos específicos para controle de Seriais de Rastreadores, ICCIDs, Periféricos e Câmeras.
* **Persistência Local (Offline-First)**: Utilização de `localStorage` para garantir que nenhum dado seja perdido durante a operação, mesmo sem conexão constante.

---

### 🛠️ Diferenciais Técnicos
* **Ingestão Versátil de Dados**: Suporte para importação via arquivos Excel (.xlsx), CSV ou colagem direta de texto, utilizando a biblioteca **SheetJS**.
* **Integração com Ecossistema JIRA**: Identificação automática de chaves de chamados via Expressões Regulares (Regex) e geração de links diretos para a plataforma.
* **Sincronização com Cloud**: Arquitetura que utiliza **Google Apps Script** para persistir dados concluídos em uma planilha mestra do Google Sheets.
* **Fila de Submissão Segura**: Implementação de lógica de fila (`submissionQueue`) para garantir a integridade dos dados durante envios em massa.

---

### 🚀 Impacto Operacional
* **Automação de Etiquetas**: Funcionalidade integrada para exportação de dados formatados prontos para geração de etiquetas de expedição.
* **Monitoramento em Tempo Real**: Painel de estatísticas que exibe o total de chamados pendentes e concluídos na sessão atual.

---

### 💻 Stack Tecnológica
* **Frontend**: HTML5, Tailwind CSS, Lucide Icons.
* **Processamento**: JavaScript (ES6+), SheetJS.
* **Backend/Cloud**: Google Apps Script, LocalStorage API.
