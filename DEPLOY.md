# 🚀 Guia de Deploy no GitHub Pages

## Pré-requisitos

- Conta no GitHub
- Git instalado no computador

## Passo a Passo

### 1. Criar Repositório no GitHub

1. Acesse [github.com](https://github.com)
2. Clique em **"New repository"** (ou no botão **+** no canto superior direito)
3. Preencha:
   - **Repository name:** `convite-miguel` (ou o nome que preferir)
   - **Description:** "Convite digital para aniversário - Tema Carros"
   - Marque como **Public**
   - **NÃO** marque "Add a README file" (já temos um)
4. Clique em **"Create repository"**

### 2. Inicializar o Repositório Local

Abra o terminal/prompt na pasta do projeto e execute:

```bash
git init
git add .
git commit -m "Initial commit: Convite aniversário Miguel"
```

### 3. Conectar com o GitHub

Substitua `SEU-USUARIO` pelo seu nome de usuário do GitHub:

```bash
git remote add origin https://github.com/SEU-USUARIO/convite-miguel.git
git branch -M main
git push -u origin main
```

### 4. Ativar GitHub Pages

1. No repositório do GitHub, vá em **Settings** (Configurações)
2. No menu lateral esquerdo, clique em **Pages**
3. Em **Source**, selecione:
   - **Branch:** `main`
   - **Folder:** `/ (root)`
4. Clique em **Save**
5. Aguarde alguns minutos (geralmente 1-3 minutos)

### 5. Acessar o Site

Seu convite estará disponível em:

```
https://SEU-USUARIO.github.io/convite-miguel/
```

## 📝 Fazendo Alterações

Para atualizar o convite após modificações:

```bash
git add .
git commit -m "Descrição da alteração"
git push
```

O GitHub Pages será atualizado automaticamente em alguns minutos.

## 🔧 Dicas Importantes

### Domínio Personalizado (Opcional)

Se você tiver um domínio próprio:

1. Vá em **Settings > Pages**
2. Em **Custom domain**, adicione seu domínio
3. Configure o DNS do seu domínio apontando para o GitHub Pages

### Verificar Build

Após o push, você pode verificar o status do deploy em:
- **Actions** tab no repositório do GitHub

### Performance

- Todos os arquivos estão otimizados
- Imagens já estão na raiz
- CSS está inline para carregamento mais rápido
- Fontes são carregadas do Google Fonts (CDN rápido)

### SEO Básico

O HTML já inclui:
- Meta viewport para responsividade
- Title descritivo
- Lang="pt-BR" para português brasileiro

## 🐛 Solução de Problemas

### Site não carrega

1. Verifique se o GitHub Pages está ativado em Settings > Pages
2. Aguarde alguns minutos após o push
3. Limpe o cache do navegador (Ctrl+Shift+Delete)
4. Tente em modo anônimo/privado

### Imagens não aparecem

- Todos os caminhos de arquivos estão relativos (sem `/` no início)
- Certifique-se de que todos os arquivos foram commitados:
  ```bash
  git status
  ```

### Fontes não carregam

- A fonte Magneto (MAGNETOB.TTF) está na raiz do projeto
- Fontes do Google são carregadas via CDN

## 📱 Compartilhar o Convite

Depois de publicado, você pode:

1. **Encurtar a URL** usando [bit.ly](https://bitly.com) ou [tinyurl.com](https://tinyurl.com)
2. **Criar QR Code** usando [qr-code-generator.com](https://www.qr-code-generator.com)
3. **Compartilhar diretamente** no WhatsApp, email ou redes sociais

## 🎯 Próximos Passos

- [ ] Fazer primeiro deploy
- [ ] Testar em diferentes dispositivos
- [ ] Compartilhar com amigos e família
- [ ] Monitorar confirmações via WhatsApp

---

**Qualquer dúvida, consulte a [documentação oficial do GitHub Pages](https://docs.github.com/pt/pages)**
