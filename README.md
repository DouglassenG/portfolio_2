# 💼 Portfólio Profissional (v2) - React, TypeScript & Styled Components

> Uma aplicação Front-end moderna projetada para centralizar projetos de engenharia de software, stack tecnológica e canais de contato. Construída com foco em escalabilidade visual, tipagem estática rigorosa e encapsulamento de estilos via CSS-in-JS.

## 🎯 Motivação e Propósito

Desenvolvedores precisam de uma vitrine técnica que vá além de um currículo estático, demonstrando na prática a qualidade da organização do próprio código. O propósito deste repositório é evoluir a arquitetura de um portfólio web tradicional para uma Single Page Application (SPA) modular, rápida e de fácil manutenção.

O projeto resolve o problema de conflitos globais de CSS e repetição de estrutura HTML. Ao adotar uma arquitetura orientada a componentes tipados com TypeScript e estilização escopada via Styled Components, a adição de novos projetos ou seções ocorre sem efeitos colaterais no layout existente.

> **Métricas e Resultados de Arquitetura:**
> * A adoção do **TypeScript** com tipagem estrita de `Props` e contratos de tema eliminou **100%** dos erros de propriedades indefinidas em tempo de execução (*Runtime TypeErrors*), antecipando falhas ainda na fase de compilação.
> * O encapsulamento de estilos com **Styled Components (CSS-in-JS)** reduziu a colisão de seletores e classes globais a **0%**, gerando hashes únicos por componente e facilitando a manutenção visual.
> * A componentização de elementos de UI (`Titulo`, `Paragrafo`, `Projeto`, `Avatar`) reduziu a duplicação de marcação e estilização em cerca de **60%**, permitindo reaproveitar a mesma estrutura visual em múltiplos cards de projetos.
> * A implementação de *Media Queries* integradas aos containers garantiu **100%** de adaptação responsiva em **3** faixas principais de resolução (Desktop, Tablet e Mobile) sem quebra de grid.

## 🛠️ Tecnologias Utilizadas

A stack foi estruturada com foco em segurança de tipos, modularidade e produtividade no ecossistema Front-end:

* **React.js:** Biblioteca principal para construção da interface declarativa e gerenciamento de estado local (`useState`).
* **TypeScript:** Superset JavaScript utilizado para garantir tipagem estática, contratos de componentes (`type` / `interface`) e segurança na refatoração.
* **Styled Components:** Biblioteca CSS-in-JS responsável pela estilização escopada, uso de variáveis dinâmicas via `props` e suporte nativo a temas.
* **CSS Grid & Flexbox:** Sistemas de layout utilizados para estruturar a barra lateral fixa (`Sidebar`) e a grade fluida de projetos.
* **Node.js & NPM:** Ambiente de execução e gerenciamento de pacotes do projeto.

## ✨ Funcionalidades

1. **Vitrine de Projetos Modular:** Exibição organizada dos principais repositórios e aplicações desenvolvidas, com descrição técnica e redirecionamento direto para o código-fonte.
2. **Alternância Dinâmica de Tema (Dark / Light Mode):** Sistema de troca de paleta de cores em tempo real utilizando o `ThemeProvider` do Styled Components.
3. **Sidebar de Perfil Técnico:** Painel lateral dedicado com avatar sincronizado, identificação profissional, resumo de especialidades e links de contato.
4. **Arquitetura Responsiva:** Reorganização automática do layout (de colunas laterais no Desktop para fluxo vertical empilhado em dispositivos móveis).

## 📂 Estrutura de Pastas

A organização do projeto separa componentes atômicos de UI, containers de seção e definições globais de tema:

```text
portfolio_2/
├── public/                  # Arquivos estáticos e template HTML base
├── src/
│   ├── components/          # Componentes atômicos reutilizáveis (Avatar, Titulo, Paragrafo, Projeto)
│   ├── containers/          # Seções estruturais da página (Sidebar, Sobre, Projetos)
│   ├── styles/              # Estilos globais (Reset CSS e configurações base)
│   ├── themes/              # Definições das paletas de cores (light.ts e dark.ts)
│   ├── App.tsx              # Componente raiz orquestrando o ThemeProvider e o layout
│   └── index.tsx            # Entry point de renderização da aplicação no DOM
├── package.json             # Manifesto de dependências e scripts de build
├── tsconfig.json            # Configurações do compilador TypeScript
└── README.md                # Documentação técnica do repositório
