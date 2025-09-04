# Palhares Ferreira Advocacia — Site estático (HTML/CSS/JS)

## Como usar
1. Substitua `assets/logo.svg` pela sua logomarca.
2. Edite `script.js` na seção `CONFIG`:
   - `whatsappNumber`: número completo com DDI e DDD (ex.: +5511999999999)
   - `whatsappMsg`: mensagem automática inicial
   - `instagramUser`: usuário do Instagram (sem @)
   - `email`: e-mail de contato
   - address`: endereço do escrit`ório
   - `googleMapsEmbedUrl`: link de incorporação do Google Maps (iframe `src`)

> **Como obter o link do Google Maps (embed)**
> - Google Maps ➜ busque o endereço ➜ `Compartilhar` ➜ `Incorporar um mapa` ➜ copie o `src` do `<iframe>` e cole em `CONFIG.googleMapsEmbedUrl`.

3. Atualize o **blog** em `posts.json` (não precisa tocar no HTML):
```json
[
  {"title": "Título do post", "date": "2025-08-01", "excerpt": "Resumo...", "url": "https://link-externo-ou-pagina.html"}
]
```
4. Teste localmente com um servidor estático (para o `fetch` do `posts.json` funcionar):
   - Python: `python -m http.server 8080` (ou outro)
   - Node: `npx serve`
5. Publique os arquivos em qualquer hospedagem estática (Cloudflare Pages, Vercel, Netlify, GitHub Pages, etc.).

## SEO incluído
- Metatags básicas (`title`, `description`, `keywords`, OpenGraph).
- JSON-LD `LegalService` com campos para completar.
- HTML semântico, headings hierárquicos e alt em imagens.

## Acessibilidade e UX
- Link “Pular para o conteúdo”.
- Teccla de contraste claro/escuro om persistência.
- Animações leves (reveal on scroll).

## Sem formulário
A página de contato usa só botões/links (WhatsApp, Instagram e e-mail), conforme solicitado.

---
Feito com ♥ para Palhares Ferreira Advocacia.
