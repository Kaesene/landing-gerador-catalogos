# 🚀 Landing Page - Gerador de Catálogos

Landing page profissional otimizada para conversão, pronta para vender seu software!

## ✅ O Que Está Incluído

- **Design moderno e responsivo** (funciona em celular, tablet e desktop)
- **Hero section** com preço de/por e desconto de 80%
- **Seção de vídeo** para sua demonstração
- **9 features destacadas** com ícones
- **5 benefícios** detalhados
- **3 depoimentos** (editáveis)
- **8 perguntas frequentes** com accordion interativo
- **2 CTAs** estrategicamente posicionados
- **Garantia de 7 dias** em destaque
- **Animações suaves** e efeitos de hover
- **100% em HTML/CSS/JS puro** (fácil de hospedar)

## 📝 Como Personalizar

### 1. **Adicionar Seu Vídeo**

Localize a seção `<!-- Video Section -->` (linha ~229) e substitua o placeholder por:

**Opção A - Vídeo Local:**
```html
<video controls>
    <source src="demo-video.mp4" type="video/mp4">
</video>
```

**Opção B - YouTube:**
```html
<iframe width="100%" height="500"
    src="https://www.youtube.com/embed/SEU_VIDEO_ID"
    frameborder="0" allowfullscreen>
</iframe>
```

**Opção C - Vimeo:**
```html
<iframe src="https://player.vimeo.com/video/SEU_VIDEO_ID"
    width="100%" height="500" frameborder="0" allowfullscreen>
</iframe>
```

### 2. **Configurar Link de Checkout**

Localize `SEU_LINK_DE_CHECKOUT_AQUI` (linha ~546) e substitua pelo link da sua plataforma de pagamento:

```html
<a href="https://pay.kiwify.com/seu-link" class="cta-button">
```

**Plataformas sugeridas:**
- **Kiwify**: https://kiwify.com.br
- **Hotmart**: https://hotmart.com
- **Stripe**: https://stripe.com
- **Mercado Pago**: https://mercadopago.com.br

### 3. **Editar Depoimentos**

Localize a seção `<!-- Testimonials Section -->` (linha ~399) e personalize:

```html
<div class="testimonial-card">
    <div class="stars">⭐⭐⭐⭐⭐</div>
    <p class="text">"Seu depoimento aqui..."</p>
    <p class="author">Nome do Cliente</p>
    <p class="role">Cargo/Empresa - Cidade</p>
</div>
```

### 4. **Atualizar Informações de Contato**

No footer (linha ~562):

```html
<a href="mailto:seuemail@exemplo.com">Contato</a>
```

### 5. **Adicionar Favicon**

Coloque um arquivo `favicon.png` na mesma pasta do `index.html`.

## 🌐 Como Publicar (Grátis!)

### Opção 1: Vercel (Recomendado)

1. Crie conta em https://vercel.com
2. Conecte com GitHub
3. Crie repositório com a landing page
4. Faça deploy (1 clique)
5. Domínio grátis: `seu-projeto.vercel.app`

### Opção 2: Netlify

1. Crie conta em https://netlify.com
2. Arraste a pasta no site (drag & drop)
3. Pronto! Domínio grátis: `seu-projeto.netlify.app`

### Opção 3: GitHub Pages

1. Crie repositório no GitHub
2. Faça upload dos arquivos
3. Ative GitHub Pages nas configurações
4. Domínio grátis: `seu-usuario.github.io/nome-repo`

## 🎨 Personalização Avançada

### Mudar Cores Principais

No `<style>` (linha ~13), localize:

```css
/* Gradiente roxo */
background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);

/* Altere para suas cores */
background: linear-gradient(135deg, #SUA_COR_1 0%, #SUA_COR_2 100%);
```

**Cores sugeridas:**
- Azul: `#4A90E2 → #357ABD`
- Verde: `#56AB2F → #A8E063`
- Laranja: `#F2994A → #F2C94C`

### Adicionar Google Analytics

Antes do `</head>`, adicione:

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

### Adicionar Facebook Pixel

Antes do `</head>`, adicione:

```html
<!-- Facebook Pixel -->
<script>
  !function(f,b,e,v,n,t,s)
  {if(f.fbq)return;n=f.fbq=function(){n.callMethod?
  n.callMethod.apply(n,arguments):n.queue.push(arguments)};
  if(!f._fbq)f._fbq=n;n.push=n;n.loaded=!0;n.version='2.0';
  n.queue=[];t=b.createElement(e);t.async=!0;
  t.src=v;s=b.getElementsByTagName(e)[0];
  s.parentNode.insertBefore(t,s)}(window, document,'script',
  'https://connect.facebook.net/en_US/fbevents.js');
  fbq('init', 'SEU_PIXEL_ID');
  fbq('track', 'PageView');
</script>
```

## 📊 Testes A/B Sugeridos

1. **Preço**: Teste R$ 50 vs R$ 47 vs R$ 49,90
2. **Headline**: Teste diferentes frases no H1
3. **Cor do CTA**: Teste amarelo vs verde vs laranja
4. **Garantia**: Teste 7 dias vs 14 dias vs 30 dias
5. **Urgência**: Teste "100 primeiros" vs "48 horas" vs "Estoque limitado"

## 🎯 Checklist de Lançamento

- [ ] Substituir placeholder do vídeo pelo vídeo real
- [ ] Configurar link de checkout
- [ ] Editar depoimentos (usar depoimentos reais se possível)
- [ ] Adicionar favicon
- [ ] Atualizar email de contato
- [ ] Configurar Google Analytics
- [ ] Configurar Facebook Pixel (opcional)
- [ ] Testar todos os botões
- [ ] Testar em celular
- [ ] Verificar velocidade de carregamento
- [ ] Fazer deploy

## 💡 Dicas de Conversão

1. **Vídeo é CRUCIAL**: Grave um vídeo mostrando o software funcionando (2-3 min)
2. **Depoimentos reais**: Peça feedback de primeiros usuários
3. **Screenshots**: Adicione capturas de tela do app funcionando
4. **Senso de urgência**: "Apenas X vagas" funciona bem
5. **Garantia forte**: 7-14 dias de garantia aumenta conversão
6. **Prova social**: Contador de vendas, selos de segurança, etc.

## 🚨 Próximos Passos

1. Grave o vídeo de demonstração
2. Configure seu checkout (Kiwify é o mais fácil)
3. Faça deploy da página
4. Compartilhe nas redes sociais
5. Crie anúncios no Google/Facebook (opcional)

## 📞 Suporte

Qualquer dúvida sobre a landing page, é só avisar!

---

**Boa sorte nas vendas! 🚀💰**
