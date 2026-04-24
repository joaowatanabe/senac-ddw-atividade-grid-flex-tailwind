# Fruta & Fruto

Site single page desenvolvido como atividade prática da Unidade Curricular de **Desenvolvimento Web para Dispositivos Móveis** do **SENAC-RS**.

---

## Sobre o Projeto

O **Fruta & Fruto** é um site fictício de receitas com foco no reaproveitamento de alimentos. O objetivo da atividade é aplicar na prática os conceitos de HTML semântico, estilização com Tailwind CSS e design responsivo para múltiplos dispositivos.

---

## Tecnologias Utilizadas

| Tecnologia          | Descrição                                  |
| ------------------- | ------------------------------------------ |
| **HTML5**           | Estrutura semântica da página              |
| **Tailwind CSS v4** | Estilização via classes utilitárias inline |
| **Google Fonts**    | Fontes Pacifico (títulos) e Roboto (corpo) |

---

## Técnicas Abordadas

### HTML Semântico

Uso correto das tags estruturais do HTML5, garantindo acessibilidade e organização do conteúdo:

- `<header>`, `<main>`, `<footer>` para estrutura macro da página
- `<section>` para separar blocos de conteúdo
- `<nav>` e `<ul>` para a navegação
- `<article>` implícito nos cards de receitas
- Hierarquia correta de títulos: `<h1>` → `<h2>` → `<h4>` → `<h5>`

### Responsividade / Mobile First

O layout foi construído com abordagem **mobile first**, expandindo progressivamente para telas maiores:

- Grid de cards: `grid-cols-1` → `sm:grid-cols-2` → `lg:grid-cols-3`
- Tamanhos de fonte fluidos: `text-5xl md:text-6xl lg:text-7xl`
- Altura do hero adaptada: `min-h-120 md:min-h-140`
- Controle de quebra de linha no desktop: `md:whitespace-nowrap`

### Tailwind CSS — Classes Utilitárias

Toda a estilização é aplicada diretamente no HTML via classes Tailwind, sem CSS externo customizado:

- **Layout:** `flex`, `grid`, `gap`, `max-w-*`, `mx-auto`, `px-*`, `py-*`
- **Posicionamento:** `fixed`, `absolute`, `relative`, `inset-0`, `z-50`
- **Tipografia:** `font-[Pacifico]`, `font-[Roboto]`, `font-light`, `font-bold`, `text-*`, `leading-*`
- **Cores arbitrárias:** `text-[#8B1A1A]`, `bg-[#f0f0f0]`, `hover:bg-[#5C0F0F]`
- **Efeitos:** `shadow-md`, `rounded-lg`, `overflow-hidden`, `object-cover`, `drop-shadow-lg`
- **Scroll suave:** `scroll-mt-16` para compensar o header fixo ao navegar por âncoras

### Navegação por Âncoras

Menu fixo (`fixed`) com links internos que rolam suavemente até cada seção usando IDs (`#inicio`, `#receitas`, `#quem-somos`, `#contato`) e a classe `scroll-mt-16` para não sobrepor o conteúdo.

### Overlay em Imagem de Fundo

Técnica de sobreposição no hero com imagem de fundo posicionada com `absolute inset-0` e uma camada `bg-black/40` para escurecer e garantir legibilidade do texto branco.

### Tipografia com Google Fonts

Uso de duas famílias tipográficas com papéis distintos:

- **Pacifico** — fonte cursiva decorativa, usada exclusivamente em títulos (`h1`, `h2`, `h4`)
- **Roboto** — fonte sem serifa legível, usada em todo o corpo de texto

---

## 📁 Estrutura de Arquivos

```
fruta-e-fruto/
├── index.html
├── css/
│   └── output.css          # CSS gerado pelo Tailwind CLI
└── assets/
    ├── img/
    │   ├── logo.jpg
    │   ├── banner.jpg
    │   ├── receitas/
    │   │   ├── tigela-de-abacate.jpg
    │   │   ├── salada-de-kiwi.jpg
    │   │   ├── prato-oriental.jpg
    │   │   ├── pimentoes-a-juliana.jpg
    │   │   ├── mix-de-vegetais.jpg
    │   │   └── beterrabas-assadas.jpg
    │   └── pessoas/
    │       ├── roberta.jpg
    │       ├── marcela.jpg
    │       └── andreia.jpg
```

---

## Informações Acadêmicas

- **Instituição:** SENAC-RS
- **Unidade Curricular:** Desenvolvimento Web para Dispositivos Móveis
- **Tipo:** Atividade prática individual
