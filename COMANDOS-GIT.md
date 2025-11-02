# 📝 Comandos Git - Guia Rápido

## Primeiro Deploy

### 1. Inicializar o repositório
```bash
git init
```

### 2. Adicionar todos os arquivos
```bash
git add .
```

### 3. Fazer o primeiro commit
```bash
git commit -m "Initial commit: Convite aniversário Miguel - Tema Carros"
```

### 4. Adicionar o repositório remoto
Substitua `SEU-USUARIO` pelo seu nome de usuário do GitHub:
```bash
git remote add origin https://github.com/SEU-USUARIO/convite-miguel.git
```

### 5. Renomear branch para main
```bash
git branch -M main
```

### 6. Enviar para o GitHub
```bash
git push -u origin main
```

---

## Atualizações Futuras

Quando fizer alterações no convite:

### 1. Ver arquivos modificados
```bash
git status
```

### 2. Adicionar alterações
```bash
# Adicionar todos os arquivos modificados
git add .

# OU adicionar arquivo específico
git add index.html
```

### 3. Fazer commit
```bash
git commit -m "Descrição da alteração"
```

Exemplos de mensagens:
- `"Atualiza data do evento"`
- `"Corrige link do WhatsApp"`
- `"Melhora responsividade mobile"`
- `"Ajusta cores do tema"`

### 4. Enviar para o GitHub
```bash
git push
```

---

## Comandos Úteis

### Ver histórico de commits
```bash
git log
```

### Ver histórico resumido
```bash
git log --oneline
```

### Ver diferenças antes de commitar
```bash
git diff
```

### Desfazer alterações não commitadas
```bash
# Desfazer alterações em arquivo específico
git checkout -- index.html

# Desfazer todas as alterações
git checkout -- .
```

### Ver repositórios remotos
```bash
git remote -v
```

---

## Solução de Problemas

### Erro: "remote origin already exists"
```bash
git remote remove origin
git remote add origin https://github.com/SEU-USUARIO/convite-miguel.git
```

### Erro: "Updates were rejected"
```bash
git pull origin main --rebase
git push
```

### Esqueci de adicionar arquivo
```bash
git add arquivo-esquecido.txt
git commit --amend --no-edit
git push --force
```

### Quero mudar a mensagem do último commit
```bash
git commit --amend -m "Nova mensagem"
git push --force
```

---

## Estrutura de Branches (Opcional - Avançado)

Se quiser trabalhar com branches separadas:

### Criar branch para desenvolvimento
```bash
git checkout -b dev
```

### Alternar entre branches
```bash
git checkout main
git checkout dev
```

### Mesclar branch dev na main
```bash
git checkout main
git merge dev
git push
```

---

## Boas Práticas

✅ **FAZER:**
- Commits frequentes e pequenos
- Mensagens descritivas
- Testar antes de commitar
- Usar `.gitignore` para arquivos desnecessários

❌ **NÃO FAZER:**
- Commitar arquivos com senhas ou dados sensíveis
- Fazer commits muito grandes
- Usar mensagens genéricas ("update", "fix")
- Fazer `git push --force` sem necessidade

---

## Fluxo de Trabalho Recomendado

1. ✏️ Fazer alterações no código
2. 🧪 Testar localmente (abrir index.html no navegador)
3. 📝 `git status` (ver o que mudou)
4. ➕ `git add .` (adicionar alterações)
5. 💬 `git commit -m "mensagem"` (commitar)
6. 🚀 `git push` (enviar para GitHub)
7. ⏳ Aguardar 1-3 minutos
8. ✅ Verificar no GitHub Pages

---

## Links Úteis

- [Git Cheat Sheet](https://education.github.com/git-cheat-sheet-education.pdf)
- [GitHub Docs](https://docs.github.com/pt)
- [Git Book (PT-BR)](https://git-scm.com/book/pt-br/v2)

---

**Dica:** Salve este arquivo para consulta rápida! 📌
