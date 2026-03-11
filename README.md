# Weven — Landing Page

Landing page estática e responsiva para apresentar o app de gestão de inventário com IA da Weven. Construída com HTML, Tailwind CSS (prefixo `tw-`), GSAP (animações) e Swiper (carrossel).

## Recursos

- Layout 100% responsivo com Tailwind CSS.
- Animações de entrada e scroll com GSAP + ScrollTrigger.
- Seções de Hero, Prova Social, Benefícios, Dicas e CTA.
- Ícones via Bootstrap Icons e Google Material Icons (CDN).
- Metadados e Open Graph configurados em português.

## Estrutura

```
landWEVEN/
├─ assets/            # imagens e ícones
├─ css/
│  ├─ tailwind.css    # fonte do Tailwind
│  ├─ tailwind-build.css
│  └─ index.css       # estilos adicionais
├─ index.html         # página principal
├─ index.js           # scripts (animações, menu, etc.)
└─ tailwind.config.js # configurações do Tailwind
```

## Como rodar localmente

1. cd landWEVEN
2. npm install
3. npm run start:tailwind
4. Abra `landWEVEN/index.html` no navegador (de preferência com Live Server).

## Build de produção

- npm run build:tailwind
- O HTML referencia `css/tailwind-build.css`.

## Publicação no GitHub Pages

Opção 1 — docs/ (recomendada):
1. Crie uma pasta `docs/` na raiz do repositório.
2. Copie todo o conteúdo de `landWEVEN/` para `docs/`.
3. Settings → Pages → Build and deployment → Deploy from a branch → `main` + `/docs`.

Opção 2 — raiz do repositório:
1. Mova o conteúdo de `landWEVEN/` para a raiz.
2. Settings → Pages → Deploy from a branch → `main` + `/ (root)`.

## SEO e Metadados

- Título e descrição em pt‑BR no `<head>`.
- Open Graph (og:title, og:description, og:url, og:image) em `landWEVEN/index.html`.
- Favicon em `landWEVEN/assets/logo.png`.

## Scripts

- Desenvolvimento: `npm run start:tailwind`
- Produção: `npm run build:tailwind`

