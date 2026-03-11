# Weven — Landing Page (AI Sales)

Landing page estática com animações e layout responsivo para divulgar um app de gestão de inventário com IA. O projeto utiliza HTML, Tailwind CSS (com prefixo de classes), animações com GSAP e carrossel com Swiper.

## Visão Geral

- Conteúdo focado em apresentar benefícios do produto, com seções de destaque, prova social e CTA.
- Estilos com Tailwind CSS usando prefixo `tw-` para evitar conflitos.
- Animações de entrada e ao rolar usando GSAP e ScrollTrigger.
- Ícones via Bootstrap Icons e Google Material Icons CDN.

## Estrutura de Pastas

- Raiz do repositório: metadados do projeto.
- Código-fonte da landing: pasta `landWEVEN/`
  - HTML/CSS/JS e assets ficam dentro de `landWEVEN`.
  - Arquivos principais:
    - `landWEVEN/index.html`
    - `landWEVEN/css/` (inclui `tailwind.css`, `tailwind-build.css` e `index.css`)
    - `landWEVEN/index.js`
    - `landWEVEN/assets/` (imagens e ícones)

## Como Rodar Localmente

1) Requisitos
- Node.js LTS e npm instalados.

2) Instalar dependências (na pasta da landing)
- Abra o terminal na raiz do repositório e execute:
  - `cd landWEVEN`
  - `npm install`

3) Desenvolvimento (Tailwind em modo watch)
- Ainda em `landWEVEN`, rode:
  - `npm run start:tailwind`
- Abra o arquivo `index.html` no navegador (idealmente com uma extensão tipo Live Server).

4) Build de produção (CSS minificado)
- Em `landWEVEN`, rode:
  - `npm run build:tailwind`
- O HTML utiliza o arquivo gerado `css/tailwind-build.css`.

Scripts disponíveis em [package.json](file:///c:/Users/willi/OneDrive/Documentos/landing-page/landWEVEN/package.json#L6-L9).

## SEO e Metadados

- Ajuste o título e a descrição na head do HTML.
- Atualize as tags Open Graph para compartilhamento:
  - Arquivo: [index.html](file:///c:/Users/willi/OneDrive/Documentos/landing-page/landWEVEN/index.html#L14-L21)
  - Campos: `og:title`, `og:description`, `og:type`, `og:url` e `og:image`.
- Favicon: `./assets/logo.png` dentro da pasta `landWEVEN/assets/`.

## Personalização de Tema

- As cores principais estão definidas no Tailwind:
  - [tailwind.config.js](file:///c:/Users/willi/OneDrive/Documentos/landing-page/landWEVEN/tailwind.config.js#L12-L15)
  - `primary: #BFFE66`, `secondary: #BDB8FF`
- Todas as classes Tailwind usam o prefixo `tw-` (ex.: `tw-flex`, `tw-text-4xl`).

## Acessibilidade e Boas Práticas

- Use textos alternativos nas imagens (`alt`).
- Garanta contraste adequado entre texto e fundo.
- Mantenha os CTAs com rótulos claros e atributos `aria-label` quando necessário.

## Deploy no GitHub Pages

Você tem duas opções:

- Opção A (recomendada): publicar os arquivos da pasta `landWEVEN` na raiz do repositório antes do deploy.
  - Copie o conteúdo de `landWEVEN/` para a raiz (ou ajuste a raiz do site para essa pasta).
  - Faça o build (`npm run build:tailwind`) e confirme que `css/tailwind-build.css` está referenciado no HTML.
  - Faça push para o GitHub e ative o Pages na aba “Settings” → “Pages”.

- Opção B: manter o código dentro de `landWEVEN` e publicar essa pasta.
  - Configure o Pages para publicar a partir de uma pasta específica (por exemplo, via GitHub Actions).
  - Alternativamente, crie uma pasta `docs/` na raiz e copie o conteúdo de `landWEVEN` para `docs/` (o Pages aceita publicar `/docs`).

## Tecnologias

- HTML5, CSS3 (Tailwind CSS 3.x)
- JavaScript (ES6+)
- GSAP + ScrollTrigger (via CDN)
- Swiper (via CDN)
- Bootstrap Icons, Google Material Icons (via CDN)

## Licença

- Licença: MIT (conforme `package.json`).
- Animações com GSAP — verifique as condições de uso da biblioteca.
