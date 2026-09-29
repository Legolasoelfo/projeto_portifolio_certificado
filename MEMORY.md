# Memória do projeto

Documento de contexto para retomar o trabalho (por pessoas ou por assistentes de IA). Atualize a cada decisão relevante.

## Propósito

Hub pessoal de certificados de 2026 que passa a sensação de acompanhar a evolução de uma pessoa em tecnologia. Não é um currículo tradicional: é uma experiência.

## Decisões de design

- **Paleta (tema escuro):** fundo `#0a0f1a`; ciano `#22d3ee` = automação; verde `#34d399` = segurança de sistemas; violeta `#a78bfa` = front-end; azul `#60a5fa` = back-end.
- **Inspiração:** minimalismo premium (espaço em branco, tipografia limpa, animações suaves), sem copiar identidade visual de terceiros.
- **Abertura:** torres translúcidas flutuantes em canvas 2D, em homenagem ao estilo de consoles clássicos, **sem logo, nome nem áudio originais**. O som é sintetizado com Web Audio (original).
- **Tela de entrada com botões** porque navegadores só liberam áudio após um gesto do usuário.
- **Dados fora da lógica:** certificados, timeline, estatísticas, sobre, repositórios e pilares ficam em constantes no topo do script.

## Histórico de versões

1. Hero com personagem 3D (Three.js) e teclado animado pelo scroll.
2. Foto de referência com câmera entrando no monitor e IDE animada.
3. Loading de 4 segundos com barra.
4. Abertura estilo console clássico com animação.
5. Som de abertura sintetizado e tela de entrada.
6. Paleta tech por área, seção do GitHub e melhorias de UX/acessibilidade.

## Restrições e cuidados

- Sem dependências externas: manter o site em HTML/CSS/JS puros, a menos que o roadmap avance para React.
- Caminhos de arquivos relativos (compatível com GitHub Pages em subpasta).
- Respeitar `prefers-reduced-motion` e manter alvos de toque de pelo menos 44 px.
- Certificados marcados como "Exemplo" são apenas ilustrativos.

## Pendências

Ver [ROADMAP.md](ROADMAP.md).

## Como retomar com uma IA

Envie o `index.html` e este arquivo e diga o que quer mudar. Peça para preservar os dados no topo do script e as decisões acima.
