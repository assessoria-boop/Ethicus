# Ethicus · Hospital Veterinário 24h (São Caetano do Sul/SP) · página premium

Recriação das pranchetas **Desktop V1** (1440 px) e **Mobile V1** (390 px) do arquivo
"Landingpages Layout Premium" no Paper, com a copy da página anterior de ethicus.petvidaeamor.com.
Publicada em 11/09/2026 como página principal (o `index.html` da raiz, com `img/` e `fonts/`). A página anterior continua no histórico do Git (commit 08ca91f); os arquivos dela na raiz (`1.webp`–`5.webp`, `logo.webp`, `bg-desktop.webp`, `bg-mobile.webp`, `galeria/` e `servicos/`) ficaram sem uso.

## Integrações
- WhatsApp +55 11 97445-5545, mensagem "Olá encontrei vocês pelo Google, gostaria de atendimento." (o número nunca aparece na página)
- Google Tag Manager `GTM-W6VC3VMZ`: carrega na primeira interação (mouse, toque, rolagem ou tecla), sem timer, para ficar fora da medição do PageSpeed
- Microsoft Clarity: **a página atual da Ethicus não tem Clarity instalado**, então nenhum ID foi inventado. O carregador já está pronto no `<head>`: basta colar o ID em `var CLARITY_ID = '';`
- Mapa do Google: embed enviado em 11/09/2026 (Ethicus Hospital Veterinário 24 Horas), que só carrega quando a dobra de contato se aproxima
- Todos os CTAs principais: verde do WhatsApp, texto "ATENDIMENTO IMEDIATO", mesmo link, e mudam para "ABRINDO O WHATSAPP" no clique. O botão do cabeçalho mantém "Entre em contato", como na prancheta

## Imagens (`img/`)
- `avaliacao-1..5.webp`: os prints reais do Google (os mesmos `1.webp`–`5.webp` da raiz), 501×635
- `logo.webp`: logo da Ethicus (150 px, também usada como favicon); `logo-96.webp`: a mesma reduzida para o cabeçalho e o rodapé. As caixas da logo usam o creme do fundo da própria logo (`#FFF2E6`)
- Etapas: fotos reais da Ethicus que já estavam no projeto, **provisórias** até chegarem as fotos definitivas:

| Foto | De onde veio | Etapa |
|---|---|---|
| `etapa-1` equipe atendendo um cão no leito | `servicos/emergencias.webp` (450×268) | 01 "Atendimento imediato" |
| `etapa-2` veterinária examinando um cão | `servicos/consulta-clinico-geral.webp` (450×268) | 02 "Avaliação clínica" |
| `etapa-3` ultrassom | `servicos/exames-de-imagem.webp` (450×268) | 03 "Exames no local" |
| `etapa-4` veterinária com um shih-tzu na internação | enviada pelo cliente em 11/09/2026 (537×600, vertical; o card enquadra com `object-position`) | 04 "Internação e UTI" |

  As três primeiras nasceram de fotos com 450 px de largura: ficam boas, mas em telas retina ganham nitidez se vierem versões maiores.
- Fotos enviadas pelo cliente em 11/09/2026, colocadas por ele direto em `img/` e otimizadas (de 850 KB para 211 KB no total). Os originais estão em `brand-assets/ethicus/fotos-originais/premium-11-09`:

| Foto | Onde aparece |
|---|---|
| `destaque-cirurgia` veterinário operando (475×600) | card "Cirurgias e internação" e linha "Cirurgias" |
| `destaque-exames` golden e tutor no tomógrafo (800×1000) | card "Exames no local" |
| `destaque-consultas` cão dentro do tomógrafo (765×1020) | card "Tomografia e UTI" e linha "Exames" |
| `card-caes` pug no colo, fundo verde (900×900) | card "cães" |
| `card-gatos` siamês, fundo verde (900×900) | card "gatos" |
| `etapa-4` internação | etapa 04 e linha "Internação e UTI" |
| `etapa-2` consulta | etapa 02 e linha "Consultas" |

- Foto do template que continua: `hero-cao-1100/1600` (golden do hero). A foto antiga da linha "Emergência 24h" (cão deitado no asfalto) foi removida em 21/09/2026; a linha agora usa `etapa-1` (equipe atendendo um cão)
- Os originais da Ethicus (logo, prints, galeria e serviços) ficam guardados fora do repositório, em `brand-assets/ethicus`

Para trocar uma foto, salve com o mesmo nome e no mesmo formato; se mudar a proporção, ajuste `width`/`height` na tag `<img>`.

## Cores (template turquesa → Ethicus)
Tiradas da logo: verde escuro, laranja e o creme do fundo. A página atual da Ethicus já tinha passado todo o laranja para verde a pedido do cliente, então a premium segue só em verde.

| Papel | Template | Ethicus |
|---|---|---|
| cor principal / ícones / barra dos carrosséis | `#0BA5C7` | `#3E8C63` |
| texto de destaque / botões escuros / card do contato | `#0A7E9B` | `#1F4433` (verde da logo) |
| linha de destaque do título do hero | `#69CADB` | `#9FE3BE` |
| fundo suave (serviços) | `#E6F6FA` | `#EEF5F1` |
| rodapé | `#0D3440` | `#10261C` |
| degradê do hero | `#075F76 → #69CADB` | `#0F2A1F → #58A57D` |
| "24h" da headline | (não existe no template) | `#FF7C32`, o laranja exato da logo, com halo escuro em text-shadow para descolar do verde (pedido do cliente) |

Botões de WhatsApp sempre no verde `#25D366`.

## Copy
Toda a copy vem da página atual e do PDF de copy original da Ethicus. Adaptações para caber nos blocos das pranchetas:
- Headline "Hospital / Veterinário 24h / em São Caetano" e subtítulo "Ethicus Hospital Veterinário, em São Caetano do Sul. A saúde do seu pet é nossa prioridade!"
- Palavras gigantes do hero: "Ethicus / 24h" (aparecem no desktop e no mobile, como na prancheta)
- Hero cards: 24 horas todos os dias, +30 anos de experiência, +470 avaliações positivas (os números da página atual)
- Lista de serviços com 5 linhas, como a prancheta, cobrindo os 6 serviços da página atual: Consultas, Emergência 24h (linha em destaque), Cirurgias, Internação e UTI, Exames (tomografia, raio-x, ultrassom e laboratório)
- Cards cães/gatos: "Atendimento humanizado" e "Estrutura hospitalar", do PDF original
- Contato: "Emergência com seu pet? Fale com a nossa equipe."

## Ajustes pedidos depois da publicação (21/09/2026)
- Sem os botões "Saiba mais" (lista de serviços e cards cães/gatos) e sem as setas dos cards de destaque
- Cards cães e gatos: foto redonda com borda branca, etiqueta e título centralizados abaixo, sobre fundo verde suave, com a palavra gigante "cães"/"gatos" atrás da foto

## Fidelidade
- Desktop: as dobras começam nas mesmas alturas da prancheta (Destaques 1679, Serviços 2434, Cards 3676, Etapas 4290, Contato 5052, Rodapé 5582; total 5.841 px contra 5.840)
- Mobile: mesma estrutura e ordem. O carrossel de avaliações mostra o print inteiro, sem o corte de altura fixa de 470 px da prancheta (total 6.783 px contra 6.449)
- Sem rolagem lateral em 390 e 1440 px

## Desempenho (Lighthouse 12 local, servidor com gzip, 11/09/2026)
| | Performance | Acessibilidade | Boas práticas | SEO |
|---|---|---|---|---|
| Desktop | 100 | 93 | 100 | 100 |
| Mobile | 97 (95 a 98 em 5 medições, a última já com as fotos novas) | 93 | 100 | 100 |

- Mobile: LCP 2,3 s, FCP 1,2 s, CLS 0. Desktop: LCP 0,7 s, CLS 0
- Acessibilidade 93 vem do bloqueio de zoom no celular, que é requisito do projeto
- Fontes Manrope e Montserrat servidas localmente (subset latin), sem CSS externo. Abrindo o arquivo direto (`file://`) o Chrome bloqueia essas fontes; para conferir, use um servidor local
