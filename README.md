# Letícia Corres — Landing Page

Landing page da terapeuta **Letícia Corres** — estética integrativa e terapias naturais, com atendimento em **Vila Velha** e **Serra (ES)** e teleconsultas para todo o Brasil.

Site **estático** (HTML, CSS e JavaScript puros), leve, responsivo e otimizado para SEO. Pronto para hospedar no **GitHub** + **Netlify**.

---

## 📁 Estrutura

```
leticia-corres/
├── index.html          Página principal (com todo o SEO embutido)
├── css/
│   └── style.css       Estilos (paleta verde-sálvia & creme)
├── js/
│   └── main.js         Menu, animações, WhatsApp e fallback de imagens
├── images/
│   ├── favicon.svg     Ícone do site
│   └── og-cover.jpg    Imagem de capa para redes sociais (WhatsApp/Facebook)
├── netlify.toml        Configuração de deploy e cabeçalhos
├── robots.txt          Instruções para buscadores
├── sitemap.xml         Mapa do site para o Google
└── README.md           Este arquivo
```

---

## 🎨 Identidade visual

- **Cores:** verde-sálvia, creme e off-white (paleta natural, botânica).
- **Fontes:** Cormorant Garamond (títulos) + Jost (texto), carregadas do Google Fonts.
- **Imagens:** as fotos são carregadas do Unsplash. Se alguma não carregar, aparece automaticamente um **fundo botânico da marca** no lugar — o site nunca mostra imagem quebrada.

### Trocar pelas fotos reais da Letícia (recomendado)
1. Coloque as fotos dela na pasta `images/` (ex.: `hero.jpg`, `leticia.jpg`).
2. No `index.html`, troque o endereço `https://images.unsplash.com/...` de cada `<img>` pelo caminho local, ex.: `src="images/hero.jpg"`.
3. Substitua também `images/og-cover.jpg` por uma foto/arte dela para as redes sociais.

---

## 🔎 SEO e Google (serviços "recomendados de forma orgânica")

Tudo o que ajuda o Google a entender e recomendar os serviços já está no código:

- **Meta tags** de título, descrição e palavras-chave (limpeza de pele, revitalização, teleconsulta, vegano, dry needling, acupuntura, ventosaterapia…).
- **Geolocalização** (`geo.region`, `geo.position`, `ICBM`) apontando para **Vila Velha e Serra, ES**.
- **Dados estruturados JSON-LD** do tipo *HealthAndBeautyBusiness* + *FAQPage*: nome, telefone, área de atendimento, lista de serviços, horários e link do Instagram. É isso que gera os resultados ricos e o reconhecimento local no Google.
- **sitemap.xml** e **robots.txt** para indexação.
- **Open Graph / Twitter Cards** para uma pré-visualização bonita ao compartilhar o link.

> **Observação honesta:** os serviços estão descritos no HTML de forma **legível e semântica** (não como texto escondido/oculto atrás do fundo). Isso é proposital: o Google **penaliza** texto camuflado ("cloaking"), e o caminho seguro para ranquear de forma orgânica é exatamente o que foi feito aqui — dados estruturados + conteúdo real rico em palavras-chave. Assim a Letícia sobe nas buscas sem risco de punição.

### Depois de publicar
1. Cadastre o site no **Google Search Console** (`search.google.com/search-console`).
2. Envie o `sitemap.xml`.
3. Crie/valide o **Perfil da Empresa no Google** (Google Meu Negócio) para Vila Velha e Serra — é o que mais impulsiona a busca local.

---

## 🚀 Como publicar

### Opção A — Netlify por "arrastar e soltar" (mais rápido)
1. Acesse **app.netlify.com/drop**.
2. Arraste a **pasta inteira** `leticia-corres` para a área indicada.
3. Pronto: o Netlify gera um endereço (ex.: `nome-aleatorio.netlify.app`). Em *Site settings → Domain* você pode trocar o nome ou ligar um domínio próprio.

### Opção B — GitHub + Netlify (recomendado, com atualizações automáticas)

**1. Subir no GitHub**
```bash
cd leticia-corres
git init
git add .
git commit -m "Landing page Letícia Corres"
git branch -M main
git remote add origin https://github.com/SEU_USUARIO/leticia-corres.git
git push -u origin main
```

**2. Conectar ao Netlify**
1. Em **app.netlify.com** → *Add new site* → *Import an existing project*.
2. Escolha **GitHub** e selecione o repositório `leticia-corres`.
3. Deixe *Publish directory* como `.` (já definido no `netlify.toml`) e clique em **Deploy**.
4. A cada `git push`, o Netlify republica o site automaticamente.

### Domínio próprio (opcional)
Em *Domain settings* no Netlify, adicione seu domínio (ex.: `leticiacorres.com.br`) e siga as instruções de DNS. Depois, atualize os endereços `https://leticiacorres.com.br/` no `index.html`, `sitemap.xml` e `robots.txt`.

---

## 📞 Contato configurado

- **WhatsApp:** +351 960 281 342 — botão flutuante e todos os CTAs já apontam para `https://wa.me/351960281342`.
- **Instagram:** [@leticia.corres](https://www.instagram.com/leticia.corres/)

Para trocar o número, faça um "localizar e substituir" de `351960281342` no `index.html`.

---

Feito com cuidado 🌿
