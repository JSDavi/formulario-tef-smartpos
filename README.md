# Formulário de Aquisição TEF / SMARTPOS - Infobrasil Sistemas

Este é o formulário de aquisição front-end oficial, projetado com uma interface limpa, acessível e responsiva.

## 🚀 Arquitetura e Tecnologias

Este projeto é 100% estático (Serverless) e utiliza serviços de terceiros para garantir segurança e entrega:

* **Hospedagem:** GitHub Pages (Sem limites de build, sempre online)
* **Design:** HTML5, CSS3, e Vanilla JavaScript (Identidade visual da Infobrasil Sistemas)
* **Envio Principal de Dados:** FormSubmit (E-mail ofuscado por string de segurança)
* **Auto-Resposta ao Cliente:** EmailJS (Template em português)
* **Segurança Anti-Bot:** Google reCAPTCHA v3 (Totalmente invisível, validado via EmailJS) + Trava de clique duplo no JS.

## 🔐 Segurança Implementada (Zero Trust)

Seguindo as regras estritas do projeto:
1. **Nenhum e-mail exposto no código-fonte.**
2. **Defesa DDoS / Spam:** O botão sofre disable (loading state) instantaneamente ao ser clicado. A requisição só é liberada se passar no desafio invisível do Google reCAPTCHA v3.
3. **Bloqueio de Domínio ativado.**

## 🌍 Como Publicar (GitHub Pages)

O deploy é feito automaticamente pelo GitHub, de forma gratuita:
1. Vá na aba **Settings** do repositório no GitHub.
2. Acesse **Pages** no menu esquerdo.
3. Em "Branch", selecione `main` e clique em **Save**.
