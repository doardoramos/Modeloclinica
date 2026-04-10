# iStore Premium — Deploy no Vercel

## 🚀 Como fazer o deploy

### Opção 1 — Via Vercel CLI (recomendado)

```bash
# 1. Instale a CLI do Vercel (apenas uma vez)
npm install -g vercel

# 2. Dentro desta pasta, rode:
vercel

# 3. Siga o assistente interativo:
#    - Log in (ou crie conta)
#    - Confirme o nome do projeto
#    - Confirme as configurações padrão (pressione Enter)
```

O site estará online em segundos com uma URL tipo `https://istore-premium.vercel.app`.

---

### Opção 2 — Via GitHub (deploy contínuo)

1. Suba esta pasta para um repositório GitHub
2. Acesse [vercel.com](https://vercel.com) e clique em **"Add New Project"**
3. Importe o repositório
4. Clique em **Deploy** — sem configuração extra necessária

Cada `git push` fará um novo deploy automático.

---

### Opção 3 — Drag & Drop

1. Acesse [vercel.com/new](https://vercel.com/new)
2. Arraste a pasta `istore-vercel` diretamente para o site
3. Pronto ✅

---

## 📁 Estrutura do projeto

```
istore-vercel/
├── public/
│   └── index.html      ← site completo (HTML + CSS + JS)
├── vercel.json         ← configuração do Vercel
└── README.md
```

## ✏️ Personalizações antes do deploy

No arquivo `public/index.html`, localize e edite:

| O que mudar | Onde encontrar |
|---|---|
| Número do WhatsApp | `📱 (21) 99999-0000` |
| Nome/logo da loja | `iStore Premium` |
| Preços dos produtos | `data-price` nos cards do catálogo |
| Imagens dos iPhones | `data-img` nos cards |
| Cor de destaque | `--accent: #4f8ef7` nos tokens CSS |
