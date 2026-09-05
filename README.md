# Aula Prática 1 de Arquitetura Web

# Aula Prática 1 - Comparativo Prático: HTML Semântico vs. HTML Não Semântico

Este projeto foi desenvolvido como uma atividade prática com o objetivo de evidenciar as diferenças conceituais, estruturais e de acessibilidade entre o uso de **HTML Semântico** e a estruturação genérica baseada apenas em tags neutras (**HTML Não Semântico / Div Soup**).

Ambas as versões compartilham o mesmo layout visual e propósito de conteúdo, permitindo uma análise direta de como a escolha das tags impacta a qualidade do código, a indexação (SEO) e a experiência de tecnologias assistivas.

---

## 🔗 Demonstração e Links do Projeto

Você pode acessar e inspecionar o código de cada uma das versões nos links abaixo:

- 🌐 **Versão Semântica:** [Acesse aqui](https://alefealvesc.github.io/Alefe_2023010253_Aula_Pratica_DCC704/versao-otimizada/)
- 📦 **Versão Não Semântica (Divs):** [Acesse aqui](https://alefealvesc.github.io/Alefe_2023010253_Aula_Pratica_DCC704/versao-nao-otimizada/)

---

## 🎯 Objetivo da Atividade

- Analisar na prática o impacto da perda de significado semântico quando todo o documento é estruturado unicamente por `<div>` e `<span>`.
- Demonstrar a clareza, manutenibilidade e hierarquia proporcionadas pelas tags semânticas da especificação HTML5.
- Compreender a relevância das landmarks semânticas para acessibilidade digital (leitores de tela como NVDA, TalkBack, VoiceOver).

---

## ⚖️ Quadro Comparativo

| Elemento / Seção | Versão Semântica | Versão Não Semântica |
| :--- | :--- | :--- |
| **Cabeçalho da Página** | `<header>` | `<div class="header">` |
| **Menu de Navegação** | `<nav>` + `<ul><li>` | `<div class="menu">` + `<div>` |
| **Conteúdo Principal** | `<main>` | `<div id="content">` ou `<div class="main">` |
| **Artigos / Posts Independentes** | `<article>` | `<div class="post">` ou `<div class="card">` |
| **Seções Temáticas** | `<section>` | `<div class="section">` |
| **Conteúdo Relacionado / Lateral** | `<aside>` | `<div class="sidebar">` |
| **Rodapé** | `<footer>` | `<div class="footer">` |
| **Botões de Ação** | `<button>` | `<div onclick="...">` |
| **Títulos Hierárquicos** | `<h1>` até `<h6>` | `<div class="title-lg">` |

---

## 🔍 Principais Diferenças Observadas

### 1. Acessibilidade (A11y)
- **HTML Semântico:** Leitores de tela conseguem mapear landmarks de navegação (`header`, `main`, `footer`), permitindo ao usuário cego pular diretamente para o conteúdo principal ou navegar pelos tópicos usando atalhos de teclado.
- **HTML Não Semântico:** O leitor de tela interpreta a página como um bloco homogêneo de divisões genéricas, sem oferecer pontos de referência nativos para navegação rápida.

### 2. SEO (Search Engine Optimization) e Web Scraping
- Os motores de busca (como o Google) atribuem peso e contexto ao conteúdo baseado na semântica. Elementos como `<main>` e `<article>` indicam com precisão onde está o conteúdo de valor, facilitando indexação e rich snippets.

### 3. Manutenibilidade e Legibilidade do Código
- Na versão semântica, qualquer desenvolvedor que inspeciona o HTML identifica imediatamente a função de cada componente. Na versão com apenas `<div>`, a compreensão depende inteiramente de nomes de classes arbitrários (`div soup`).

---

## 📂 Estrutura de Arquivos

```text
├── versao-otimizada/
│   ├── index.html       # Implementação utilizando tags HTML5 semânticas
│   ├── styles.css       # Folha de estilo
│   └── scripts.js       # Arquivo JavaScript
├── versao-nao-otimizada/
│   ├── index.html       # Implementação estruturada exclusivamente com divs
│   ├── styles.css       # Folha de estilo espelhada para manter o mesmo design
│   └── scripts.js       # Arquivo JavaScript
└── README.md            # Documentação do projeto
```

---

## 🛠️ Tecnologias Utilizadas

- **HTML5** (Semântico e Estrutural)
- **CSS3** (Estilização e Normalização)
- **JavaScript** (Interatividade e Manipulação DOM)
---

## 👨‍💻 Autor

Desenvolvido por **Álefe Alves da Costa**.