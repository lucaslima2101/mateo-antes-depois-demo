# EVIDÊNCIA — V4 (refinamento, sem marca)

Rodada: 2026-11-05 · executor: Naia (representante), pipeline determinístico.

## O que mudou (feedback V3 do Lucas, aplicado inteiro)
- Opções 1, 3 e 5 usadas como referências; **nenhum** conceito tratado como integralmente aceito.
- Execução 3 (Hélice Aberta) e 4 (Elos em Suspensão) **retrabalhadas** (haviam sido chamadas de toscas).
- As cinco versões refinadas; marca/logomarca **removida** de todas as peças.
- Ausência de marca **não implica** uso adequado ou autorizado; nenhuma conformidade é alegada.
- Selo adicional "verificação clínica: pendente" em todas as peças + rodapé reforçado.
- Casos reais (Argibenone): **bloqueados** — origem e consentimento de imagem não verificados; nada real é exibido; sem upload a serviços externos; demonstração exclusivamente sintética.
- Sem protocolo, dose, tempo ou instrução clínica inventados; campos ausentes não aparecem; "tempo não informado" quando desconhecido.

## Verificação executada
- QA automatizado (Playwright/Chrome): 5 templates × desktop 1200 / intermediário 800 / mobile 390 —
  sem marca (`marca-card`/logo ausentes, string ausente no corpo), lockup correto, status presente,
  rodapé ≥4 linhas de segurança, fonte carregada, zero sobreposição, placeholders sintéticos nos
  visores, contraste WCAG ≥ mínimo, zero erro de console. (`evidencia/qa-render.json`)
- QA visual por visão: 5 renders desktop + 2 renders mobile revisados individualmente;
  rodapés completos sem truncamento; zero logomarca.
- Teste de miniatura 300px (contact sheet sem títulos): 5 silhuetas inconfundíveis
  (diagonal fluida / faixa horizontal pesada com círculos / eixo vertical da hélice / dark + arco / cápsulas bio-orgânicas).
- Galeria: 4 painéis de status + 5 cartões com prévias; prévias confirmadas renderizadas por viewport
  (nota: captura `full_page` headless pode omitir camadas escaladas fora da viewport — artefato de
  captura, não de navegação; evidência por cartão em `qa-render/card-0X-viewport.png`).
- Integridade: MANIFESTO-SHA256.txt com hashes de todos os artefatos; zero rede
  (nenhum fetch/XHR/img externo; canário de padrões no build).

## Rotas de imagem por IA (GPT Image / Nano Banana / Flow)
Re-sondadas com chamadas reais em 2026-11-05 — **bloqueadas** (evidência em `rotas-imagem-probe-v4.json`).
Nada foi simulado como gerado; fundos 100% procedimentais (CSS + SVG, sementes fixas). Sem gasto.

## Conteúdo desta pasta (100% sintético, sem dados reais)
index.html · seda-em-vies.html · materia-em-relevo.html · helice-aberta.html ·
elos-em-suspensao.html · campo-vesicular.html · MANIFESTO-SHA256.txt ·
rotas-imagem-probe-v4.json · CONTACT-SHEET.png
