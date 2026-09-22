# Formulário Oficial de Aquisição — TEF / SMARTPOS
### Infobrasil Sistemas

Aplicação web moderna, responsiva e automatizada para captação, conferência e processamento de solicitações de aquisição/instalação de soluções TEF (PinPad) e SMARTPOS.

🔗 **Acesso em Produção:** [https://jsdavi.github.io/formulario-tef-smartpos/](https://jsdavi.github.io/formulario-tef-smartpos/)

---

## 🚀 Principais Recursos

- **Fluxo Condicional Inteligente:** Alternância dinâmica de formulário de acordo com a solução escolhida (PinPad / TEF físico integrado ou SMARTPOS Android móvel).
- **Consulta Automática de CNPJ (BrasilAPI):** Preenchimento instantâneo de Razão Social, Nome Fantasia e Endereço completo ao digitar os 14 dígitos do CNPJ.
- **Gerenciador Dinâmico de Terminais:**
  - Suporte a múltiplos equipamentos/caixas com adição e replicação ágil de dados (Afiliação, Lógico e Modelos).
  - Botão de auto-preenchimento ("Copiar para todos") para agilizar implantações em redes ou múltiplos caixas.
- **Geração Client-Side de Checklist Oficial (.docx):**
  - O documento Word oficial da empresa é gerado diretamente no navegador do usuário utilizando `JSZip` e um template otimizado.
  - Tabela de equipamentos 100% dinâmica (ajusta-se automaticamente à quantidade exata de terminais cadastrados: 1, 5, 10 ou mais).
  - Nomenclatura padronizada: `CHECK LIST [CNPJ] - [NOME DA EMPRESA] [DATA].docx`.
  - Disponibiliza download local imediato na tela de confirmação.
- **Disparo de E-mail com Anexo (FormSubmit Multipart):**
  - Envio nativo em segundo plano via `iframe` oculto, garantindo entrega do anexo binário (.docx) e resumo completo na caixa da equipe técnica.
  - Sem recarregamento brusco da página e sem poluição visual no corpo do e-mail.
- **Segurança & Proteção contra Bots:**
  - Proteção invisível via **Google reCAPTCHA v3**.
  - Validação estrita de campos obrigatórios e máscaras de digitação em tempo real (`Cleave.js`).
- **Design & Acessibilidade:**
  - Totalmente responsivo (Mobile-first) com escala de espaçamentos fluida.
  - Navegação intuitiva pelo teclado (avanço no `Enter` e auto-focus dinâmico).
  - Ícones semânticos em SVG de alta fidelidade visual.

---

## 🛠️ Tecnologias Utilizadas

- **Frontend:** HTML5, CSS3 moderno (Flexbox, CSS Grid, variáveis nativas), JavaScript Vanilla (ES6+).
- **Processamento de Documentos:** `JSZip` (v3.10.1) com template compilado em Base64.
- **Máscaras de Entrada:** `Cleave.js` (v1.6.0).
- **Segurança:** Google reCAPTCHA v3.
- **API Externa:** `BrasilAPI` (v1).
- **Entrega de Formulários:** `FormSubmit`.
- **Hospedagem:** GitHub Pages.

---

## 📂 Estrutura de Arquivos

```text
├── index.html                           # Aplicação completa (Estrutura, Estilos e Scripts)
├── docx_template_b64.js                 # Template DOCX oficial compilado em Base64
├── template_checklist_tef.docx          # Modelo Word base com marcadores dinâmicos
├── Exemplo de relatorio preenchido...   # Documento de referência visual
├── SMARTPOS.jpg                         # Imagem do equipamento SmartPOS
├── TEF.jpg                              # Imagem do equipamento PinPad/TEF
└── README.md                            # Documentação do projeto
```

---

&copy; 2026 **Infobrasil Sistemas**. Todos os direitos reservados.
