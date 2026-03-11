# Weven — Landing Page

Landing page estática e responsiva para divulgar o app de gestão de inventário com IA da Weven. O projeto usa HTML, Tailwind CSS com prefixo `tw-`, GSAP (animações) e Swiper (carrossel).

## Recursos

- Layout responsivo com Tailwind CSS (prefixo `tw-`).
- Animações de entrada e ao rolar com GSAP + ScrollTrigger.
- Seções de Hero, Prova Social, Benefícios, Dicas e CTA.
- Ícones via Bootstrap Icons e Google Material Icons (CDN).

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

## Requisitos

- Node.js LTS e npm.

## Instalação

1. Entre na pasta do projeto:
   - `cd landWEVEN`
2. Instale as dependências:
   - `npm install`

## Desenvolvimento

- Inicie o Tailwind em modo watch:
  - `npm run start:tailwind`
- Abra `landWEVEN/index.html` no navegador (recomendado usar uma extensão tipo Live Server).

## Build de Produção

- Gere o CSS minificado:
  - `npm run build:tailwind`
- O HTML referencia `css/tailwind-build.css`.

## SEO e Metadados

- Título/descrição ajustados para português.
- Open Graph configurado (title/description/url/image) em `landWEVEN/index.html`.
- Favicon: `landWEVEN/assets/logo.png`.

## Publicação no GitHub Pages

Opção 1 — Publicar a pasta `docs/`:
1. Crie `docs/` na raiz do repositório.
2. Copie o conteúdo de `landWEVEN/` para `docs/`.
3. Em Settings → Pages → Build and deployment:
   - Deploy from a branch
   - Branch: `main` | Folder: `/docs`

Opção 2 — Publicar na raiz:
1. Mova o conteúdo de `landWEVEN/` para a raiz do repositório.
2. Em Settings → Pages → Build and deployment:
   - Deploy from a branch
   - Branch: `main` | Folder: `/ (root)`

## Personalização de Tema

- Cores principais em `tailwind.config.js`:
  - `primary: #BFFE66`
  - `secondary: #BDB8FF`
- Todas as classes Tailwind usam prefixo `tw-` (ex.: `tw-flex`, `tw-text-4xl`).

## Boas Práticas de Acessibilidade

- Forneça `alt` descritivo nas imagens.
- Garanta contraste adequado de cores.
- Use `aria-label` nos botões/links quando necessário.

## Scripts

- `npm run start:tailwind` — watch do Tailwind (dev)
- `npm run build:tailwind` — build minificado (prod)

## Licença

MIT. Ver `package.json`.
