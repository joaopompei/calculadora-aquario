# 🚀 Guia de Deploy na Vercel

Este guia irá te ajudar a publicar a Calculadora de Consumo de Aquário na Vercel usando Git.

## 📋 Pré-requisitos

- ✅ Conta no GitHub
- ✅ Git instalado no seu computador
- ✅ Conta na Vercel (pode fazer login com GitHub)

## 🔧 Passo a Passo

### 1️⃣ Criar Repositório no GitHub

1. Acesse [GitHub](https://github.com)
2. Clique no botão **"+"** no canto superior direito
3. Selecione **"New repository"**
4. Preencha:
   - **Repository name:** `calculadora-aquario` (ou outro nome)
   - **Description:** "Calculadora de consumo de energia para aquário"
   - Deixe como **Public**
   - ✅ Marque **"Add a README file"** (ou use o README.md que criei)
5. Clique em **"Create repository"**

### 2️⃣ Preparar os Arquivos Localmente

Abra o terminal/prompt de comando e execute:

```bash
# Criar pasta do projeto
mkdir calculadora-aquario
cd calculadora-aquario

# Inicializar Git
git init

# Configurar seu Git (se ainda não configurou)
git config user.name "Seu Nome"
git config user.email "seu.email@exemplo.com"
```

### 3️⃣ Adicionar os Arquivos

Copie os arquivos que criei para dentro da pasta `calculadora-aquario`:
- `calculadora-aquario.html` (renomeie para `index.html`)
- `README.md`

**IMPORTANTE:** Renomeie o arquivo HTML para `index.html` para que a Vercel reconheça como página principal.

No terminal, execute:

```bash
# Renomear o arquivo
mv calculadora-aquario.html index.html

# Verificar os arquivos
ls
# Deve aparecer: index.html  README.md
```

### 4️⃣ Fazer o Primeiro Commit

```bash
# Adicionar todos os arquivos
git add .

# Fazer commit
git commit -m "Versão inicial da calculadora de aquário"

# Adicionar repositório remoto (substitua SEU_USUARIO e NOME_REPO)
git remote add origin https://github.com/SEU_USUARIO/calculadora-aquario.git

# Enviar para o GitHub
git branch -M main
git push -u origin main
```

💡 **Dica:** Se pedir autenticação, use um Personal Access Token do GitHub ao invés de senha.

### 5️⃣ Deploy na Vercel

#### Opção A: Via Dashboard da Vercel (Mais Fácil)

1. Acesse [Vercel](https://vercel.com)
2. Faça login com sua conta do GitHub
3. Clique em **"Add New..."** → **"Project"**
4. Encontre o repositório `calculadora-aquario`
5. Clique em **"Import"**
6. Mantenha as configurações padrão
7. Clique em **"Deploy"**
8. Aguarde 30-60 segundos
9. **Pronto!** 🎉 Seu site está no ar!

A Vercel vai gerar um link tipo: `calculadora-aquario.vercel.app`

#### Opção B: Via CLI da Vercel

Se preferir usar a linha de comando:

```bash
# Instalar Vercel CLI (apenas uma vez)
npm install -g vercel

# Fazer login
vercel login

# Deploy
vercel

# Seguir as instruções interativas
# Pressione Enter para aceitar as sugestões padrão
```

### 6️⃣ Personalizar Domínio (Opcional)

Na dashboard da Vercel:
1. Acesse seu projeto
2. Vá em **"Settings"** → **"Domains"**
3. Adicione um domínio customizado (se tiver) ou use o subdomínio da Vercel

## 🔄 Atualizações Futuras

Quando você modificar o código:

```bash
# Adicionar mudanças
git add .

# Fazer commit
git commit -m "Descrição da mudança"

# Enviar para o GitHub
git push

# A Vercel vai fazer deploy automaticamente! 🚀
```

## ⚙️ Configurações Opcionais da Vercel

### Criar arquivo `vercel.json` (opcional)

Para configurações avançadas, crie um arquivo `vercel.json`:

```json
{
  "buildCommand": null,
  "outputDirectory": ".",
  "framework": null
}
```

## 🐛 Problemas Comuns

### Erro: "Permission denied"
- Solução: Verifique se você tem permissão de escrita no repositório

### Erro: "Failed to deploy"
- Solução: Certifique-se que o arquivo se chama `index.html`

### Site não carrega corretamente
- Solução: Verifique se todos os arquivos foram enviados corretamente
- Verifique o console do navegador (F12) para erros

## 📊 Monitoramento

Na dashboard da Vercel você pode:
- Ver estatísticas de acesso
- Verificar logs de deploy
- Configurar analytics
- Ver métricas de performance

## 🎯 Próximos Passos

Após o deploy:
- ✅ Teste o site em diferentes dispositivos
- ✅ Compartilhe o link com amigos aquaristas
- ✅ Peça feedback e faça melhorias
- ✅ Adicione Google Analytics (se quiser)

## 📱 Links Úteis

- [Documentação Vercel](https://vercel.com/docs)
- [Documentação Git](https://git-scm.com/doc)
- [GitHub Guides](https://guides.github.com)

---

**Dúvidas?** Consulte a documentação oficial ou abra uma issue no repositório!

**Boa sorte com seu deploy! 🚀**
