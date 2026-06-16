# Massafy — Inspire-se

Plataforma de inspiração visual estilo Pinterest, construída com HTML5, CSS3, JavaScript puro e Supabase como backend.

## Características

- 🎨 Interface minimalista com gradientes e glassmorphism
- 🔐 Autenticação com Google e Email via Supabase
- 💾 Sistema de salvos e favoritos sincronizados
- 🔍 Busca e filtros em tempo real
- ⚡ Sem framework JavaScript — apenas vanilla JS
- 🌙 Dark theme completo

## Setup Local

1. Clone o repositório:
```bash
git clone <seu-repo> massafy
cd massafy
```

2. Abra o arquivo `index.html` em um servidor local (não abra direto no navegador):
```bash
# Usando Python 3
python3 -m http.server 3000

# Ou com Node.js (npm install -g http-server)
http-server -p 3000
```

3. Acesse `http://localhost:3000`

## Deploy no Vercel

1. Faça o push do código para GitHub:
```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/seu-usuario/massafy.git
git push -u origin main
```

2. No [Vercel](https://vercel.com):
   - Clique em "New Project"
   - Selecione o repositório `massafy`
   - Clique em "Deploy" (não precisa de configurações adicionais)

## Configuração do Supabase

1. Crie uma conta em [Supabase](https://supabase.com)
2. No arquivo `index.html`, localize a seção `const initSupabase()` e adicione suas credenciais:

```javascript
const SUPABASE_URL = "sua-url-aqui";
const SUPABASE_KEY = "sua-chave-aqui";
```

## Estrutura do Projeto

```
massafy/
├── index.html          # Arquivo único com HTML + CSS + JS
├── vercel.json         # Configuração do Vercel
├── package.json        # Metadados do projeto
├── .gitignore          # Arquivos ignorados no git
└── README.md           # Este arquivo
```

## Tecnologias

- **Frontend**: HTML5, CSS3, JavaScript (Vanilla)
- **Styling**: Tailwind CSS (CDN), CSS Grid/Flexbox
- **Backend**: Supabase (PostgreSQL + Auth)
- **Hospedagem**: Vercel
- **Fonts**: Google Fonts (Syne, DM Sans)

## Licença

MIT
