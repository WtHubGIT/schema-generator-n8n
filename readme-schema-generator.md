# 🚀 Gerador de Schema N8N + Evolution API

Um gerador visual de schemas para facilitar a configuração de projetos com N8N, Evolution API, Redis e PostgreSQL no EasyPanel.

## 📋 Funcionalidades

- Interface web intuitiva para gerar schemas
- Integração com webhook do N8N
- Geração automática de URLs para os serviços
- Cópia rápida do schema gerado
- Link para gerador de chaves de segurança

## 🛠️ Tecnologias

- HTML5
- CSS3 (com gradientes e animações)
- JavaScript Vanilla
- Integração com N8N via webhook

## 📦 Como usar

### 1. Configure o Webhook do N8N

Antes de usar o gerador, você precisa configurar o webhook no N8N:

1. Abra seu N8N
2. Crie um novo workflow
3. Adicione um node "Webhook"
4. Configure o webhook para aceitar POST requests
5. Copie a URL do webhook

### 2. Configure o HTML

Abra o arquivo `html_form_generator.html` e substitua a URL do webhook na linha 318:

```javascript
const WEBHOOK_URL = 'http://SEU_IP:5678/webhook/gerar-schema';
```

### 3. Abra o arquivo HTML

Você pode abrir o arquivo diretamente no navegador ou hospedá-lo em um servidor web.

### 4. Preencha o formulário

- **Nome do Projeto**: O prefixo para seus domínios (ex: arcane)
- **Default Domain**: Seu domínio do EasyPanel (sem https://)
- **API Evolution Key**: Chave da API Evolution
- **N8N Encryption Key**: Chave de criptografia do N8N
- **Redis Key**: Senha do Redis
- **PostgreSQL Key**: Senha do PostgreSQL

### 5. Gere e copie o schema

Clique em "Gerar Schema" e copie o resultado para usar no EasyPanel.

## 🔑 Geração de Chaves

Para gerar chaves seguras, use o link disponível na interface:
[https://acte.ltd/utils/randomkeygen](https://acte.ltd/utils/randomkeygen)

## 📝 Estrutura do Projeto

```
schema-generator/
├── html_form_generator.html    # Interface do gerador
├── README.md                   # Este arquivo
└── .gitignore                 # Arquivos ignorados pelo Git
```

## 🤝 Contribuições

Contribuições são bem-vindas! Sinta-se à vontade para:

- Reportar bugs
- Sugerir novas funcionalidades
- Enviar pull requests

## 📄 Licença

Este projeto está sob a licença MIT.

## 👤 Autor

[Seu Nome]

---

⭐ Se este projeto te ajudou, considere dar uma estrela no GitHub!