# V3 · territórios materiais — proveniência e evidência (resumo público)

Cinco conceitos materialmente distintos de templates antes/depois (demo, placeholders sintéticos
não humanos, zero rede, zero dados privados). V1 (raiz) e V2 (`/v2/`) permanecem intactas.

## Modelos (solicitado → servido)
- **Criador de design:** `cx/gpt-6.1-sol` (9router, stream) → **servido `gpt-6.1-sol`** — especificação
  completa dos 5 conceitos (43.436 caracteres, 288,6 s), incluindo parâmetros exatos dos fundos.
- **Implementador/QA:** orquestração Hermes (zaipkg/glm-5.3-flash) — materialização determinística
  da especificação, sem decisões criativas além das resoluções de conflito documentadas.
- **Verificador adversarial (gauntlet):** `alitp-intl/deepseek-v4-pro` (9router, stream) — independente
  dos dois anteriores; veredito em `gauntlet/` no workspace local do projeto.

## Geração de imagens por IA — NÃO utilizada
Todas as rotas nomeadas foram sondadas com chamadas reais e estavam indisponíveis:
Nano Banana via tokenrouter (provedor sem suporte a imagens; crédito esgotado no upstream 403),
wan/alitp (provedor sem suporte), GPT Image (ausente do catálogo ao vivo), Google Flow
(muro de login — nenhuma sessão autorizada; nenhuma credencial foi digitada).
**Os fundos são 100% procedimentais** (CSS + SVG inline com sementes fixas — feTurbulence,
feDisplacementMap, feDiffuseLighting, grão de filme). Nada foi apresentado como se fosse gerado por IA.
A especificação documenta os prompts futuros (seção 7), rotulados "não utilizado nesta rodada".

## Marca
- Wordmark oficial mesoestetic (#1D1D1B) embutido inline, nunca recolorido; cartão branco também no
  template escuro (não existe versão branca autorizada).
- Fonte: **Hanken Grotesk (SIL OFL 1.1)** — substituta declarada da Graphik (oficial, licença comercial
  não disponível). Declaração visível no rodapé de cada peça; arquivo OFL acompanha o projeto local.
- Paleta estritamente monocromática (#1D1D1B/#111111/#4A4A4A/#7D7D7D/#D1D1D1/#E2E2E2/#F2F2F2/#F8F8F8/#FFFFFF).

## QA executado (r1)
- Render real (Chrome via Playwright): desktop 1200×1200, intermediário 800 (escala), mobile 390×844 —
  5 templates + galeria; sem sobreposições, rodapé integral, fonte carregada, zero erros de console.
- Contraste medido: 8,86:1 a 16,88:1 (mínimo exigido 4,5:1) em todos os pares de texto.
- Recorte: `data-crop="none"`, `data-image-fit="contain"` em todos os viewports (nenhum crop;
  nenhuma imagem real — nada a consentir nesta rodada).
- Distinção material: teste de miniaturas 300px (títulos removidos) — cinco silhuetas + cinco materiais
  inconfundíveis; matriz quantitativa por RMS/histograma na evidência local.
- Integridade: rodapé de 4 avisos em todas as peças; único metadado temporal "tempo não informado";
  campos opcionais ausentes; nenhum claim clínico/terapêutico; placeholders idênticos em antes/depois
  (nada sugere melhora).
- Correções r0→r1 (todas achadas por render real, não por revisão estática): lentes sobrepostas no
  Conceito 2; conteúdo mobile pintado sob os fundos (z-index morto em estáticos); offsets desktop
  persistindo no mobile; recorte de miniaturas no index. Detalhes no relatório de correções local.

## Verificação de arquivos
`MANIFESTO-SHA256.txt` lista os hashes de todos os artefatos desta pasta.
