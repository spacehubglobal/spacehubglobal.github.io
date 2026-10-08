# SpaceHub Global

Jekyll-powered multilingual technology publication.

## Site structure

- `/` — English homepage
- `/es/` — Spanish homepage
- `/pt-br/` — Brazilian Portuguese homepage
- `/blog/...` — English articles
- `/es/blog/...` — Spanish articles
- `/pt-br/blog/...` — Brazilian Portuguese articles

## Adding a new blog

Every post must include a language, category, description and a language-specific permalink.

### English

```yaml
---
layout: article
title: "Your article title"
description: "A concise search description."
date: 2026-10-08
lang: en
category: "SEO & Digital Marketing"
permalink: /blog/your-article-slug/
---
```

### Spanish

```yaml
---
layout: article
title: "Título del artículo"
description: "Descripción breve para buscadores."
date: 2026-10-08
lang: es
category: "SEO y Marketing Digital"
permalink: /es/blog/your-article-slug/
---
```

### Brazilian Portuguese

```yaml
---
layout: article
title: "Título do artigo"
description: "Descrição breve para mecanismos de busca."
date: 2026-10-08
lang: pt-BR
category: "SEO e Marketing Digital"
permalink: /pt-br/blog/your-article-slug/
---
```

The language homepage uses `site.posts` and filters by `lang`, so newly published posts appear automatically on the correct homepage. The six newest posts for that language are displayed.

## Important

Do not use the old JavaScript-only language switcher for page routing. Language selection now uses real URLs, which gives each language its own crawlable site structure and canonical URL.
