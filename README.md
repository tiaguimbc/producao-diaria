# 📊 Produção Diária - PCP

Uma solução de Planeamento e Controlo de Produção (PCP) desenvolvida para digitalizar o fluxo de trabalho industrial e logístico. O sistema permite o rastreio de equipamentos, gestão de tickets e sincronização automática com bases de dados na nuvem.

## 🚀 Funcionalidades Principais
* **Ingestão Versátil de Dados:** Suporte para importação via ficheiros Excel (.xlsx), CSV e entrada direta por texto formatado.
* **Rastreabilidade de Ativos:** Campos otimizados para captura de Seriais de Rastreadores, ICCIDs e controlo de periféricos (Teclados, Câmeras, Smart Speakers).
* **Gestão Individualizada:** Divisão de fluxo de trabalho por abas de colaboradores, permitindo uma gestão clara da produtividade por equipa.
* **Automação de Etiquetas:** Geração de ficheiros formatados prontos para a criação de etiquetas de identificação.
* **Persistência Robusta:** Utilização de `LocalStorage` para funcionamento "Offline-First", garantindo a segurança dos dados locais.

## 🛠️ Tecnologias Utilizadas
* **Frontend:** HTML5 & Tailwind CSS (Interface moderna e responsiva).
* **Core:** JavaScript (ES6+) para manipulação de lógica de negócio.
* **Integração:** SheetJS (XLSX.js) para processamento de planilhas.
* **Backend:** Google Apps Script (Web App) para persistência de dados em nuvem via Google Sheets.

## 🧩 Diferenciais Técnicos
* **Links Inteligentes para JIRA:** O sistema utiliza expressões regulares (Regex) para identificar chaves de chamados e gerar links de acesso rápido automaticamente.
* **Fila de Submissão Segura:** Implementação de lógica de fila (`submissionQueue`) para assegurar que múltiplos envios sejam processados sequencialmente sem perda de pacotes.
* **Visualização de Status:** Dashboard integrado com contagem em tempo real de itens totais e concluídos por sessão.

## 📋 Como utilizar
1. Clone o repositório.
2. Certifique-se de que a imagem de fundo `unnamed.jpg` está na raiz do projeto.
3. Abra o `index.html` e utilize o botão "Config" para importar a sua base de dados inicial.
