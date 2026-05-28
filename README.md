# TVF PRO RES — Página de Vendas

Página de vendas oficial do curso TVF PRO RES.

## 🚀 Deploy no Vercel — Passo a passo

### Método 1: Drag & Drop (mais fácil)

1. Acesse **https://vercel.com/new**
2. Faça login (GitHub, Google ou email)
3. Role até a seção **"Deploy a Template"** ou clique em **"Import"**
4. Procure a opção de upload de pasta — ou acesse diretamente:
   **https://vercel.com/new/clone** e use a área de drop
5. Arraste a pasta `tvf-deploy` inteira para a área de upload
6. Clique em **Deploy**
7. Em ~30 segundos sua URL estará no ar

### Método 2: Vercel CLI

```bash
# Instalar Vercel CLI (uma vez só)
npm install -g vercel

# Entrar na pasta do projeto
cd tvf-deploy

# Fazer deploy
vercel

# Para deploy de produção (URL definitiva)
vercel --prod
```

### Método 3: GitHub (recomendado para atualizações futuras)

1. Crie um repositório no GitHub
2. Faça upload dos arquivos `index.html` e `vercel.json`
3. Em https://vercel.com/new, conecte o repositório
4. Toda alteração no GitHub atualiza o site automaticamente

---

## 📂 Estrutura do projeto

```
tvf-deploy/
├── index.html      # Página de vendas (tudo embutido)
└── vercel.json     # Configurações de segurança e cache
```

## 🌐 Após o deploy

- A URL inicial será algo como: `tvf-pro-res-xxx.vercel.app`
- Para domínio personalizado: **Settings → Domains** no painel da Vercel
- Apontar o DNS do seu domínio para a Vercel (instruções aparecem na hora)

## 🔧 Para atualizar a página

Basta substituir o `index.html` e fazer novo deploy. Se usar GitHub, é automático.

## ⚙️ Configurações incluídas no vercel.json

- Headers de segurança (XSS, clickjacking, MIME-sniffing)
- Cache otimizado para performance
- URLs limpas (sem .html no final)
