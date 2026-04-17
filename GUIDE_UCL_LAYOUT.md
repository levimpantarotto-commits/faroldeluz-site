# Guia do Desenvolvedor: Layout Padrão UCL

Este guia explica como utilizar o sistema de design criado para o portal Farol de Luz, baseado no padrão visual da página UCL.

## Estrutura de Arquivos

- `assets/ucl-template.css`: Contém toda a identidade visual (cores, fontes, cards).
- `ucl/template.html`: Um modelo pronto ("boilerplate") para criar novas páginas rapidamente.

## Como criar uma nova página

1. Copie o arquivo `ucl/template.html`.
2. Mantenha o link para o CSS: `<link rel="stylesheet" href="../assets/ucl-template.css">`.
3. Altere o conteúdo dentro da `div.container`.

## Classes Principais

| Classe | Descrição |
| :--- | :--- |
| `.universe-bg` | Container do fundo espacial (deve conter `.stars` e `.nebula`). |
| `.white-card` | O padrão de card de oferta (fundo branco, texto escuro). |
| `.price` | Estilo para o valor do produto (grande e em negrito). |
| `.action-btn` | Botão padrão de compra dentro do card. |
| `.hero-title` | Estilo do título principal da página. |

## Cores (Variáveis CSS)

As cores estão centralizadas no `:root` do arquivo CSS:
- `--primary-bg`: Fundo azul escuro espacial.
- `--accent-gold`: Dourado padrão Farol de Luz.
- `--ucl-dark`: Azul marinho profundo usado nos textos do card branco.

## Captura de Leads (Formulário)

O formulário de captura (`index.html`) está integrado com um Google Apps Script. Para replicar em novas páginas:
1. Copie a estrutura do `<form id="lead-form">`.
2. Mantenha o script de `fetch` apontando para a URL do Web App configurada.

---
*Configurado para o portal Farol de Luz.*
