# 🚀 Como Fazer Deploy da Landing Page

## Opção 1: GitHub + Vercel (RECOMENDADO - Mais Fácil)

### Passo 1: Criar Repositório no GitHub

1. Acesse: https://github.com/new
2. Nome do repositório: `landing-gerador-catalogos`
3. Descrição: `Landing page para venda do Gerador de Catálogos`
4. Visibilidade: **Public**
5. **NÃO** marque "Add README" (já temos)
6. Clique em **"Create repository"**

### Passo 2: Enviar Código para o GitHub

No terminal, dentro da pasta `landing-gerador-catalogos`, execute:

```bash
git remote add origin https://github.com/Kaesene/landing-gerador-catalogos.git
git branch -M main
git push -u origin main
```

### Passo 3: Deploy na Vercel

1. Acesse: https://vercel.com
2. Clique em **"Add New" → "Project"**
3. Importe o repositório `landing-gerador-catalogos`
4. Clique em **"Deploy"**
5. Aguarde ~30 segundos
6. **PRONTO!** Seu site está no ar! 🎉

Você receberá uma URL tipo: `landing-gerador-catalogos.vercel.app`

---

## Opção 2: Netlify (Arrastar e Soltar)

1. Acesse: https://app.netlify.com/drop
2. **Arraste a pasta** `landing-gerador-catalogos` para o site
3. Aguarde o upload
4. **PRONTO!** URL gerada automaticamente

---

## Opção 3: GitHub Pages (Grátis)

### Depois de fazer push para o GitHub:

1. Vá para o repositório no GitHub
2. Clique em **"Settings"**
3. No menu lateral, clique em **"Pages"**
4. Em "Source", selecione: **main** branch
5. Clique em **"Save"**
6. Aguarde 1-2 minutos
7. Sua página estará em: `https://kaesene.github.io/landing-gerador-catalogos/`

---

## 🎯 Depois do Deploy

### 1. Configure o Link de Checkout

No `index.html`, linha 546, substitua:
```html
href="SEU_LINK_DE_CHECKOUT_AQUI"
```

Por seu link da Kiwify/Hotmart/etc:
```html
href="https://pay.kiwify.com/seu-link-aqui"
```

Depois faça commit e push:
```bash
git add .
git commit -m "Adiciona link de checkout"
git push origin main
```

A Vercel/Netlify atualiza automaticamente! 🚀

### 2. Adicione Seu Vídeo

Quando gravar o vídeo:

**Se hospedar no YouTube:**
1. Faça upload no YouTube
2. Pegue o ID do vídeo (depois de `watch?v=`)
3. No `index.html`, substitua o placeholder por:
```html
<iframe width="100%" height="500"
    src="https://www.youtube.com/embed/SEU_VIDEO_ID"
    frameborder="0" allowfullscreen>
</iframe>
```

**Se usar vídeo local:**
1. Coloque o arquivo `demo-video.mp4` na mesma pasta
2. Substitua por:
```html
<video controls>
    <source src="demo-video.mp4" type="video/mp4">
</video>
```

Commit e push novamente!

---

## 🌐 Domínio Personalizado (Opcional)

### Se quiser usar um domínio próprio:

**Na Vercel:**
1. Vá em "Settings" → "Domains"
2. Adicione seu domínio (ex: `geradorcat.com.br`)
3. Configure os DNS conforme instruções

**Registros DNS necessários:**
```
Tipo: A
Nome: @
Valor: 76.76.21.21

Tipo: CNAME
Nome: www
Valor: cname.vercel-dns.com
```

---

## 📊 Adicionar Analytics (Opcional)

### Google Analytics

1. Crie conta em: https://analytics.google.com
2. Crie propriedade
3. Pegue o ID (formato: G-XXXXXXXXXX)
4. Adicione no `index.html` antes do `</head>`:

```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXXXXX"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'G-XXXXXXXXXX');
</script>
```

---

## 🔥 Próximos Passos

1. ✅ Fazer deploy
2. ✅ Adicionar link de checkout
3. ✅ Gravar e adicionar vídeo
4. ✅ Testar em celular
5. ✅ Compartilhar nas redes sociais
6. 💰 Começar a vender!

---

## 🆘 Precisa de Ajuda?

Se tiver qualquer problema, me avisa! 🚀
