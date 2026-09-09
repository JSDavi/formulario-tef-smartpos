# Formulário de Aquisição TEF / SMARTPOS

## Como publicar no Netlify (gratuito)

### Passo 1 — Criar conta
Acesse https://netlify.com e crie uma conta gratuita (pode usar o Google ou GitHub).

### Passo 2 — Fazer o deploy
1. No painel do Netlify, clique em **"Add new site"**
2. Escolha **"Deploy manually"**
3. Arraste a pasta `FORMULARIOS` inteira para a área indicada
4. Aguarde alguns segundos — o Netlify gera o link automaticamente

### Passo 3 — Personalizar o link (opcional)
1. Vá em **Site configuration > Change site name**
2. Digite um nome amigável, ex: `formulario-tef-smartpos`
3. Seu link ficará: `https://formulario-tef-smartpos.netlify.app`

### Passo 4 — Ver as respostas
1. No painel do Netlify, vá em **Forms**
2. Clique no formulário `aquisicao-tef-smartpos`
3. Todas as respostas ficam salvas ali, com data e hora

---

## Estrutura do formulário

```
index.html       ? Arquivo principal do formulário
README.md        ? Este arquivo
```

## Funcionalidades

- Seleção condicional: TEF ou SMARTPOS
- Campos específicos exibidos conforme o produto escolhido
- Máscara automática de CNPJ e telefone
- Aviso amarelo quando o responsável pela loja é o mesmo do site do TEF
- Aviso laranja com instruções de instalação do AppSuperTEF
- Integração automática com Netlify Forms (sem backend necessário)
- Responsivo para celular e computador
