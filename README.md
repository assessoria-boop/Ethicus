# Ethicus · Hospital Veterinário 24h (Landing Page)

Landing page estática (HTML único, sem dependências externas) para o Ethicus Hospital Veterinário 24h · São Caetano do Sul/SP.

## Imagens que você precisa adicionar nesta pasta

Todas em **.webp** (nomes exatos, tudo minúsculo):

| Arquivo | O que é | Recomendação |
|---|---|---|
| `logo.webp` | Logo do cliente (usada no cabeçalho, no hero e como favicon) | quadrada, 512x512, fundo creme ou transparente |
| `1.webp` … `5.webp` | Prints reais das avaliações do Google (carrossel de depoimentos) | largura ~800px, altura livre |
| `clinica1.webp` … `clinica4.webp` | Fotos da clínica (galeria com fade automático) | proporção 4:3, ~1200x900px |
| `bg-desktop.webp` | Faixa de imagem do hero no desktop (base curvada) | 2400x629, assunto no centro |
| `bg-mobile.webp` | Faixa de imagem do hero no mobile | 1000x667, assunto no centro |

Quer mais ou menos prints de avaliação? Basta duplicar/remover um bloco `.carrossel-slide`
e o `.carrossel-dot` correspondente em `index.html`. O mesmo vale para as fotos da clínica:
adicione ou remova `<img>` dentro de `.clinica-galeria` (a primeira precisa ter `class="ativo"`).

## Como converter para webp

- Online: squoosh.app (qualidade 75–80 já fica ótimo)
- Windows + ImageMagick: `magick foto.jpg -quality 80 clinica1.webp`

## Configurações já aplicadas

- WhatsApp: `+55 11 97445-5545` (número nunca aparece na tela, só nos botões)
- Mensagem automática: `Olá encontrei vocês pelo Google, gostaria de atendimento.`
- Google Tag Manager: `GTM-W6VC3VMZ` (carregamento adiado até a 1ª interação ou 3,5s)
- Mapa: Street View da Estrada das Lágrimas, 1843 · Bairro Mauá
- Fontes: 100% do sistema (zero requisição de fonte externa)
- Cores da logo: verde `#1F4433`, laranja `#EF6C31`, creme `#FBF1E8`
- Botões de WhatsApp sempre no verde oficial `#25D366`
- Zoom e arraste lateral bloqueados no mobile

## Publicar

É um site estático: sirva a pasta em qualquer host (Netlify, Vercel, Hostinger, GitHub Pages)
ou abra `index.html` direto no navegador para conferir.
