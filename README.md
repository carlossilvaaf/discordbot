# 🤖 Discord Bot - Base com Slash Commands

Este é um bot de Discord básico em Node.js utilizando `discord.js` v14+ com suporte a **Slash Commands**. Ele inclui um único comando `/ping` como exemplo.

---

## 🚀 Funcionalidade
- `/ping`: Responde com `Pong!`
---

## 📁 Estrutura
├── commands/
│ └── ping.js # Comando slash /ping
├── deploy-commands.js # Script para registrar comandos
├── index.js # Arquivo principal do bot
├── config.json # Configurações do bot
└── README.md # Documentação

---

## ⚙️ Requisitos

- Node.js v16.9 ou superior
- Token do bot do Discord
- ID do cliente (clientId)
- ID de uma guild (guildId) para testes rápidos com comandos locais

---

## 📦 Instalação
npm install

🛠️ Registro dos comandos
Antes de iniciar o bot, registre os comandos com:
node deploy-commands.js

▶️ Inicializando o bot
node index.js

💡 Observações
Este projeto registra comandos apenas na guilda especificada (guildId) para desenvolvimento rápido.

Para comandos globais (disponíveis em todos os servidores), substitua:
Routes.applicationGuildCommands(clientId, guildId)
por:
Routes.applicationCommands(clientId)

📚 Créditos
Feito por Haridade 💙 usando discord.js
