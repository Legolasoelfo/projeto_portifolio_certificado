# Hub Pessoal de Certificados — 2026

Site pessoal que apresenta minha evolução em tecnologia através de cursos e certificados, com abertura animada, filtros por categoria, timeline e integração com meu GitHub.

> **Minha evolução através do aprendizado.**

**Demo:** _adicione aqui o link do GitHub Pages_ · **Autor:** [Victor Silva Granja](https://github.com/Legolasoelfo)

## Funcionalidades

- Abertura animada (torres flutuantes em canvas) com som sintetizado via Web Audio e opção "Entrar sem som"
- Hero, frase de transição e seções com animação de entrada (scroll reveal)
- Certificados em cards, com filtro por categoria (com contagem), estado vazio e modal de visualização
- Timeline da evolução (horizontal no desktop, vertical no celular)
- Estatísticas com contador animado, pilares de estudo e seção do GitHub
- Tema escuro com cores por área: ciano = automação, verde = segurança, violeta = front-end, azul = back-end

## Tecnologias

HTML, CSS e JavaScript puros, em um único `index.html`. Sem build, sem dependências e sem arquivos de áudio ou fontes externas.

## Como rodar

Abra o `index.html` no navegador. Para servir localmente: `python3 -m http.server 8000` e acesse `http://localhost:8000`.

## Como adicionar um certificado

1. Coloque a imagem e/ou o PDF na pasta `certificates/`.
2. No topo do `<script>` do `index.html`, adicione um objeto em `CERTIFICADOS`:

```js
{
  title: "Nome do curso",
  institution: "Instituição",
  category: "Cibersegurança", // Programação, Cibersegurança, Dados, Inteligência Artificial, Automação, Tecnologia, Outros
  hours: 120,
  date: "2026-10-04",
  desc: "Breve descrição do que aprendi.",
  image: "certificates/certificado-01.png",
  pdf: "certificates/certificado-01.pdf"
}
```

Use caminhos **relativos** (sem `/` no início) para funcionar no GitHub Pages. Sem `image`, o card mostra uma prévia gerada. Os itens marcados como "Exemplo" devem ser substituídos pelos certificados reais.

## Outros conteúdos editáveis (topo do script)

`TIMELINE`, `STATS`, `SOBRE`, `REPOS` (repositórios do GitHub) e `PILARES`.

## Estrutura

```
projeto_portifolio_certificado/
├── index.html       # site completo
├── certificates/    # imagens e PDFs dos certificados
├── README.md
├── ROADMAP.md       # próximos passos
└── MEMORY.md        # decisões e contexto do projeto
```

## Publicar no GitHub Pages

Repositório → **Settings → Pages** → *Deploy from a branch* → `main` / `(root)`. O site fica em `https://legolasoelfo.github.io/projeto_portifolio_certificado/`.

## UX e acessibilidade

Link "pular para o conteúdo", foco visível, navegação por teclado, alvos de toque de 44 px, modal com foco preso e fechamento por Esc, barra de progresso, seção ativa no menu, `prefers-reduced-motion` respeitado e contraste adequado no tema escuro.

## Documentação

[ROADMAP.md](ROADMAP.md) · [MEMORY.md](MEMORY.md)
