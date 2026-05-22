# Missão Transformação — Site Institucional

Site estático de uma página (`missao-transformacao.html`) para a comunidade/missão evangélica Missão Transformação, sediada em Curitiba, PR, Brasil.

## Estrutura do projeto

```
transformacao/
├── missao-transformacao.html   # Arquivo principal (todo HTML/CSS/JS inline)
├── img/                        # Todas as imagens locais
│   ├── Asset_16.png            # Logo (nav)
│   ├── Screenshot_2.png        # Imagem da seção Sobre
│   ├── Screenshot_3-10.png     # Logos dos ministérios
│   ├── Slide_001-004.jpg       # Slides do hero
│   ├── w-001 a w-010.jpg       # Fotos da galeria
│   ├── e-001 a e-004.jpg       # Produtos (bonés)
│   └── s-001 a s-004.jpg       # Produtos (camisetas)
└── CLAUDE.md
```

## Tecnologia

- HTML5 single-file (sem build, sem framework, sem dependências JS externas)
- CSS inline com variáveis CSS (`--gold`, `--cream`, `--charcoal`, etc.)
- JavaScript vanilla inline no final do `<body>`
- Fontes: Plus Jakarta Sans (headings), Inter (body), DM Sans (UI)

## Seções

| Seção | ID | Descrição |
|---|---|---|
| Hero | `#hero` | Slideshow com 4 slides + CTA Instagram |
| Sobre | `#sobre` | História da missão + stats + imagem |
| Ministérios | `#ministerios` | 8 ministérios em grid |
| Galeria | `#galeria` | 12 fotos em grid |
| Loja | `#loja` | 8 produtos (bonés + camisetas) |
| Contato | `#contato` | Info de contato + formulário |
| Footer | — | Links e copyright |

## Paleta de cores

```css
--cream:    #faf7f2   /* fundo principal */
--gold:     #b8962e   /* cor primária / destaque */
--gold-lt:  #d4ad4f   /* dourado claro */
--charcoal: #2c2924   /* texto principal */
--dark:     #19160f   /* fundo escuro (contato) */
--muted:    #63605a   /* texto secundário */
--stone:    #8c8070   /* texto terciário */
```

## Contato real

- Email: adm@transformacao.org.br
- Instagram: @missaotransformacao
- Localização: Curitiba, PR, Brasil
- Fundação: 2019

## Convenções importantes

- **CSS**: variáveis em `:root`, mobile-first media queries em `@media(max-width:768px)` e `@media(max-width:1024px)`
- **Animações**: `.reveal` + IntersectionObserver para scroll reveal; stagger animado em cards de ministérios, produtos e galeria
- **Nav**: pill flutuante com backdrop-filter, encolhe ao rolar (`class="s"`)
- **Sem backend**: formulário de contato é fake (exibe mensagem de sucesso após 1.2s)
- **SEO**: meta description, Open Graph, Twitter Card e Schema.org Organization incluídos no `<head>`
- **Acessibilidade**: `rel="noopener noreferrer"` em todos os links `target="_blank"`; `loading="lazy"` em imagens abaixo do fold

## Ministérios cadastrados

1. **Forja** — homens com caráter e propósito
2. **Adrenalina** — jovens conectados a Cristo
3. **Missão Casais** — fortalecimento do matrimônio
4. **Legendários** — legado e identidade de homens
5. **Legado** — formação de líderes intergeracionais
6. **REM** — Reto de Empoderamiento Matrimonial (casais)
7. **Conexão Mulheres** — encontro e identidade feminina
8. **Mulheres em Oração** — intercessão e fé
