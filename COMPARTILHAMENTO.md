# 📱 Configuração de Compartilhamento WhatsApp

## ✅ Meta Tags Adicionadas

Adicionei as meta tags Open Graph no HTML para que o link apareça bonito quando compartilhado no WhatsApp, Facebook, etc.

### Como vai aparecer:

**Título:**
🎉 Aniversário do Miguel - 4 Anos! 🏎️

**Descrição:**
Foi dada a largada! Convite especial para a festa de 4 anos do Miguel. Tema CARROS - Domingo, 30 de Novembro às 14h no Salão de Festas.

**Imagem:**
Logo do Carros (logo-cars.png)

---

## 🖼️ Melhorar a Imagem de Preview (OPCIONAL)

Para uma preview ainda melhor, você pode criar uma imagem personalizada de 1200x630px com:
- Logo Carros
- Nome "MIGUEL"
- Texto "4 ANOS"
- Data e local

### Passos para criar imagem personalizada:

1. **Use um editor online:**
   - [Canva.com](https://canva.com) (gratuito)
   - [Photopea.com](https://photopea.com) (gratuito, similar ao Photoshop)

2. **Tamanho da imagem:**
   - Largura: 1200px
   - Altura: 630px

3. **Conteúdo sugerido:**
   ```
   🎉 MIGUEL FAZ 4 ANOS! 🏎️
   Tema: CARROS
   30 de Novembro - 14h
   ```

4. **Salvar como:**
   - Nome: `share-preview.jpg`
   - Qualidade: Alta
   - Formato: JPG

5. **Adicionar ao projeto:**
   - Coloque o arquivo `share-preview.jpg` na raiz do projeto
   - Edite o index.html, linha 16:
   ```html
   <meta property="og:image" content="https://pedrotomecm.github.io/convite-miguel/share-preview.jpg">
   ```
   - Faça o mesmo na linha 24 (twitter:image)

---

## 🔄 Atualizar Preview no WhatsApp

Depois de fazer o deploy:

### Método 1: Cache do WhatsApp
1. Aguarde 24-48 horas
2. O WhatsApp atualiza automaticamente

### Método 2: Forçar atualização (RECOMENDADO)
1. Acesse: https://developers.facebook.com/tools/debug/
2. Cole a URL do seu convite
3. Clique em "Scrape Again"
4. Aguarde alguns minutos
5. Teste compartilhar no WhatsApp novamente

---

## 🧪 Testar Preview

### Antes de compartilhar:

1. **Facebook Debugger:**
   - URL: https://developers.facebook.com/tools/debug/
   - Cole seu link
   - Veja como vai aparecer

2. **LinkedIn Post Inspector:**
   - URL: https://www.linkedin.com/post-inspector/
   - Cole seu link

3. **Twitter Card Validator:**
   - URL: https://cards-dev.twitter.com/validator
   - Cole seu link

---

## 📋 URLs Configuradas

**IMPORTANTE:** Atualize estas URLs depois de publicar no GitHub Pages:

Atualmente configurado como:
```
https://pedrotomecm.github.io/convite-miguel/
```

Se seu repositório tiver nome diferente, atualize:
- Linha 13: `og:url`
- Linha 16: `og:image`
- Linha 24: `twitter:image`

---

## ✨ Resultado Final

Quando alguém compartilhar o link no WhatsApp, vai aparecer:

```
┌─────────────────────────────────┐
│  [IMAGEM: Logo Carros]          │
├─────────────────────────────────┤
│ 🎉 Aniversário do Miguel - 4   │
│ Anos! 🏎️                        │
│                                 │
│ Foi dada a largada! Convite    │
│ especial para a festa de 4     │
│ anos do Miguel. Tema CARROS... │
│                                 │
│ pedrotomecm.github.io           │
└─────────────────────────────────┘
```

---

## 🐛 Problemas Comuns

### Preview não aparece
- Aguarde 5-10 minutos após deploy
- Use o Facebook Debugger para forçar atualização
- Verifique se as URLs estão corretas

### Imagem não carrega
- Verifique se o arquivo existe na raiz
- Confirme que a URL está correta
- Certifique-se que o arquivo tem permissões públicas

### Texto aparece cortado
- WhatsApp limita descrição a ~150 caracteres
- Use texto mais curto se necessário

---

## 📝 Customizar Texto

Para mudar o que aparece, edite estas linhas no index.html:

**Título (linha 14):**
```html
<meta property="og:title" content="SEU TEXTO AQUI">
```

**Descrição (linha 15):**
```html
<meta property="og:description" content="SUA DESCRIÇÃO AQUI">
```

---

**Dica:** Sempre teste o compartilhamento em um grupo de teste antes de enviar para todos! 📲
