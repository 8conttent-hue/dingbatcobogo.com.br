# CLAUDE.md — DINGBATCOBOGO

Site gerado pelo **SF (Site Factory)** em 15/04/2026.

## Contexto do Site

**Nome:** DINGBATCOBOGO
**Nicho:** Casa e Decoração
**Keywords:** Ola Nos somos a Dinbat uma equipe do bem com o objetivo
**Paleta de cores:** sunset | **Fonte:** montserrat

Olá! Nos somos a Dinbat, uma equipe do bem com o objetivo de ajudar as pessoas que buscam conhecimento e aprimoramento no nosso mercado de design gráfico, arquitetura e urbanismo. Trabalhamos na área há 10 anos e para nós é um prazer poder compartilhar conhecimento através da internet. Já estamos há 5 ano trabalhando bastante para o crescimento do nosso site e acredito muito que podemos ajudar você. Leitores dos níveis iniciantes ao avançado são muito bem vindos ao nosso espaço. Temos bastante conteúdo para todos. Aqui você vai encontrar diversos reviews e análises técnicas sobre diversos assunto dentro do mercado. Todas as análises são feitas por especialistas e dedicamos muito tempo nas na criação de nossos conteúdos antes de publicar. Sinta-se em casa! Roberto Elizer Co-fundador & Diretor de Criação Roberto é formado em arquitetura e urbanismo pela universidade federal do Rio de Janeiro. Trabalha com projetos de identidade visual e Branding há mais de quatro anos. Quando não está desenvolvendo projetos, está desenhando fontes ou fazendo um design gráfico. Junto de Stephany desde 2018, opera como Diretor de Criação, ao mesmo tempo comanda as criações do nosso site. Stephany Schmitt Co-fundadora & Diretora de Criação Por cinco anos, Stephany atuou como design gráfico. Há pouco mais de três anos atrás, uniu-se a Roberto para a criação da Dingbat, além de design e outros os projetos.



## Componentes visuais usados

| Seção | Variante |
|-------|----------|
| Header | Header-D |
| Hero | Hero-D |
| Features | Features-D |
| About Section | About-D |
| Posts | Posts-D |
| Footer | Footer-E |
| Página Sobre | Sobre-H |
| Página Contato | Contato-F |

## Estrutura do projeto

```
src/
  sections/        # Layout escolhido pelo SF — Header, Hero, Features, About, Posts, Footer, Sobre, Contato
  data/            # JSONs com todo o conteúdo editável
  content/blog/    # Posts em Markdown
  pages/           # Rotas Astro (index, sobre, contato, blog, privacidade, termos)
  layouts/         # BaseLayout com fonte e cores dinâmicas
  styles/          # global.css com variáveis CSS de cor
public/
  images/          # hero.jpg, about.jpg, blog/*.jpg — inseridos automaticamente via Pexels
```

## O que editar

### Textos e conteúdo
- **`src/data/home.json`** — hero (título, subtítulo, botão), features (título, items), about section (título, desc, stats), posts
- **`src/data/sobre.json`** — conteúdo completo da página Sobre (hero, texto, missão)
- **`src/data/contato.json`** — título, subtítulo, email, tempo de resposta
- **`src/data/siteConfig.json`** — nome, slug, email, redes sociais, menu

### Imagens
Imagens já estão em `public/images/` (via Pexels). Para substituir, mantenha os mesmos nomes de arquivo:
- `hero.jpg` — imagem de fundo do Hero
- `about.jpg` — imagem da seção About (home)
- `sobre.jpg` — imagem de fundo da página Sobre
- `blog/{slug}.jpg` — imagens dos posts

### Posts do blog
Arquivos em `src/content/blog/`. Ajuste o tom de voz, adicione dados específicos do nicho e personalize conforme a identidade do site.

### Cores
Variáveis em `src/styles/global.css`: `--color-primary`, `--color-accent`, `--color-dark`.

## Deploy

```bash
bun install
bun run build
# Faça upload da pasta dist/ para Netlify, Vercel ou hosting estático
```
