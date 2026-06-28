# Pereira &amp; Sedrez — Sociedade de Advogados

Site institucional do escritório **Pereira &amp; Sedrez Sociedade de Advogados**
(Balneário Piçarras/SC). Site estático, sem etapa de build — pronto para hospedar
no **GitHub Pages**.

## Stack

- HTML5 + CSS3 (CSS custom properties, grid/flex) + JavaScript puro (sem frameworks)
- Sem dependências, sem build — apenas arquivos estáticos
- Tipografia: **Cinzel Decorative** (auto-hospedada, do manual de marca),
  **Cinzel** e **Cormorant Garamond** (títulos) e **Jost** (texto) via Google Fonts
- Paleta e logos extraídos do manual de marca oficial

## Estrutura

```
pereira-sedrez/
├── index.html              # página única (one-page)
├── assets/
│   ├── css/styles.css
│   ├── js/main.js          # header, menu mobile, animações, form → WhatsApp
│   ├── fonts/              # Cinzel Decorative (.ttf) + licença OFL
│   └── img/                # logos (transparentes), fotos, favicons
├── .nojekyll               # evita processamento Jekyll no GitHub Pages
└── README.md
```

## Seções

Início (hero) · Faixa de destaques · O Escritório · Áreas de Atuação
(Direito Imobiliário em destaque, Público, Empresarial e Trabalhista, Civil) ·
Direito Imobiliário (especialidade) · Equipe · Contato (com mapa e formulário) · Rodapé.

## Como publicar no GitHub Pages

1. Crie um repositório no GitHub (ex.: `pereira-sedrez`).
2. Envie **o conteúdo desta pasta** para a raiz do repositório:
   ```bash
   cd pereira-sedrez
   git init
   git add .
   git commit -m "Site institucional Pereira & Sedrez"
   git branch -M main
   git remote add origin https://github.com/<seu-usuario>/<repo>.git
   git push -u origin main
   ```
3. No GitHub: **Settings → Pages → Build and deployment → Source: Deploy from a branch**,
   selecione `main` / `/ (root)` e salve.
4. O site ficará disponível em `https://<seu-usuario>.github.io/<repo>/`.

### Domínio próprio (opcional)

Para usar um domínio (ex.: `pereiraesedrez.adv.br`), crie um arquivo `CNAME`
na raiz com o domínio e configure o DNS conforme a documentação do GitHub Pages.

## Personalização rápida

- **Cores:** variáveis no topo de `assets/css/styles.css` (`:root`).
- **Contato / WhatsApp:** número `5547984176438` em `index.html` e `assets/js/main.js`.
- **Textos das áreas / bios:** diretamente no `index.html`.
- **Fotos:** substitua os arquivos em `assets/img/` mantendo os nomes.

## Observação (OAB)

O conteúdo foi elaborado em tom sóbrio e informativo, em conformidade com o
Código de Ética e Disciplina da OAB e o Provimento n.º 205/2021.
