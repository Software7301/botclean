# 🤖 Bot de Whitelist Discord

Bot automatizado para gerenciar whitelist em servidores Discord com sistema de perguntas e aprovação.

## ✨ Funcionalidades

- ✅ Sistema de whitelist automatizado
- ✅ Chat limpo e profissional
- ✅ Perguntas personalizáveis
- ✅ Sistema de aprovação/reprovação
- ✅ Interface intuitiva com botões
- ✅ Suporte a DMs (mensagens privadas)

## 🚀 Instalação

### Opção 1: Desenvolvimento Local

1. **Clone o repositório:**
```bash
git clone https://github.com/Software7301/bot.git
cd bot
```

2. **Instale as dependências:**
```bash
pip install -r requirements.txt
```

3. **Configure o bot:**
```bash
cp config_example.json config.json
```
Edite o `config.json` com suas informações:
- Token do Discord
- ID do servidor
- IDs dos canais
- ID do cargo da equipe

4. **Execute o bot:**
```bash
python main.py
```

### Opção 2: Hospedagem Online (Recomendado)

#### Heroku
1. **Crie uma conta no [Heroku](https://heroku.com)**
2. **Instale o Heroku CLI**
3. **Configure as variáveis de ambiente:**
```bash
heroku config:set DISCORD_TOKEN=seu_token_aqui
heroku config:set GUILD_ID=id_do_servidor
heroku config:set WHITELIST_CHANNEL_ID=id_do_canal_anuncios
heroku config:set WHITELIST_TEAM_CHANNEL_ID=id_do_canal_equipe
heroku config:set WHITELIST_ROLE_ID=id_do_cargo_equipe
```

4. **Deploy:**
```bash
git add .
git commit -m "Deploy bot"
git push heroku main
```

#### Railway
1. **Crie uma conta no [Railway](https://railway.app)**
2. **Conecte seu repositório GitHub**
3. **Configure as variáveis de ambiente no painel do Railway**
4. **Deploy automático!**

#### Outras Plataformas
- **Render:** Similar ao Heroku
- **DigitalOcean App Platform:** Interface web
- **AWS/GCP:** Para usuários avançados

## 🔧 Configuração

### Variáveis de Ambiente (Hospedagem)
```env
DISCORD_TOKEN=seu_token_aqui
GUILD_ID=id_do_servidor
WHITELIST_CHANNEL_ID=id_do_canal_anuncios
WHITELIST_TEAM_CHANNEL_ID=id_do_canal_equipe
WHITELIST_ROLE_ID=id_do_cargo_equipe
```

### Configuração Local (config.json)
```json
{
    "token": "seu_token_aqui",
    "guild_id": "id_do_servidor",
    "whitelist_channel_id": "id_do_canal_anuncios",
    "whitelist_team_channel_id": "id_do_canal_equipe",
    "whitelist_role_id": "id_do_cargo_equipe",
    "questions": [
        "Qual é o seu nome completo?",
        "Qual é a sua idade?",
        "..."
    ]
}
```

## 📋 Comandos Disponíveis

- `!setup` - Configura o sistema de whitelist
- `!whitelist` - Reenvia o embed de whitelist
- `!verificar` - Verifica as configurações
- `!canais` - Lista todos os canais
- `!limpar_sessoes` - Limpa sessões ativas

## 🔐 Segurança

- ✅ Tokens nunca expostos no código
- ✅ Variáveis de ambiente para produção
- ✅ .gitignore configurado
- ✅ Configuração local para desenvolvimento

## 📝 Como Usar

1. **Configure o bot** com suas informações
2. **Execute o comando** `!setup` no canal desejado
3. **Usuários clicam** no botão "Iniciar Whitelist"
4. **Respondem as perguntas** via DM
5. **Equipe revisa** e aprova/reprova

## 🤝 Contribuição

1. Fork o projeto
2. Crie uma branch para sua feature
3. Commit suas mudanças
4. Push para a branch
5. Abra um Pull Request

## 📄 Licença

Este projeto está sob a licença MIT. Veja o arquivo LICENSE para mais detalhes.

## 🆘 Suporte

Se você encontrar algum problema:
1. Verifique as configurações
2. Confirme se o bot tem as permissões necessárias
3. Abra uma issue no GitHub

---

**Desenvolvido com ❤️ para a comunidade Discord**
