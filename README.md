# 🌊 Lauren Dashboard

> Painel de produtividade pessoal desenvolvido como projeto autoral durante o curso **Sprint IA no Trabalho** da [PrograMaria](https://www.programaria.org) — 2026.

---

## ✨ Sobre o Projeto

O **Lauren Dashboard** é um painel web personalizado que centraliza as ferramentas de produtividade do dia a dia em uma interface elegante e interativa. Com integração ao ecossistema Google via OAuth 2.0, o dashboard permite gerenciar tarefas e compromissos diretamente pela tela, sem precisar alternar entre vários apps.

---

## 🚀 Funcionalidades

| Feature | Descrição |
|---|---|
| 🔐 **Login com Google** | Autenticação segura via OAuth 2.0 |
| 📅 **Eventos do Google Calendar** | Visualize, adicione, edite e exclua compromissos da semana |
| ✅ **Tarefas do Google Tasks** | Liste e conclua tarefas diretamente no painel |
| ☁️ **Clima em Tempo Real** | Temperatura atual via Open-Meteo (sem API key!) |
| 🕐 **Data e Hora** | Relógio atualizado em tempo real |
| 🍅 **Pomodoro Timer** | Timer de foco com ciclos de 25 min + pausa |
| 📝 **Bloco de Notas** | Anotações salvas automaticamente no navegador (localStorage) |
| 📧 **Acesso Rápido** | Atalhos com 1 clique para Gmail, Agenda e Tarefas Google |

---

## 🛠️ Tecnologias Utilizadas

- **HTML5** + **CSS3** (Vanilla — sem frameworks)
- **JavaScript** (ES6+ — sem bibliotecas externas)
- **Google Identity Services (GIS)** — OAuth 2.0
- **Google Calendar API** — leitura e escrita de eventos
- **Google Tasks API** — leitura e conclusão de tarefas
- **Open-Meteo API** — clima em tempo real (gratuita, sem chave)
- **Google Fonts** — Outfit + Space Mono

---

## ⚙️ Como Rodar Localmente

### Pré-requisitos
- Navegador moderno (Chrome, Firefox, Edge)
- [Node.js](https://nodejs.org/) instalado (para o live-server)

### Passo a passo

```bash
# 1. Clone o repositório
git clone https://github.com/seu-usuario/lauren-dashboard.git

# 2. Entre na pasta
cd lauren-dashboard

# 3. Inicie o servidor local
npx -y live-server --host=localhost --port=8080
```

Acesse em: **[http://localhost:8080](http://localhost:8080)**

> ⚠️ É necessário acessar via `http://localhost:8080` (não via `file://`) para que o login com Google funcione corretamente.

---

## 🔐 Configuração do Google Cloud (para desenvolvedores)

Para usar sua própria conta Google, você precisará:

1. Criar um projeto no [Google Cloud Console](https://console.cloud.google.com)
2. Ativar as APIs: **Google Calendar API**, **Google Tasks API**, **Gmail API**
3. Criar credenciais OAuth 2.0 (tipo: Aplicativo Web)
4. Adicionar `http://localhost:8080` em **Origens JavaScript autorizadas**
5. Substituir o `CLIENT_ID` no `index.html` pelo seu

> ℹ️ O **Client ID** é um identificador público do app (por design do OAuth 2.0) e não representa risco de segurança ao ser compartilhado.

---

## 🔒 Segurança

Este projeto utiliza **apenas o OAuth 2.0 Client ID**, que é público por design e seguro de versionar. Não há chaves secretas, tokens ou senhas no código.

Caso você adapte o projeto com outras APIs que exijam chaves secretas, utilize **variáveis de ambiente** e nunca as inclua no repositório.

---

## 📁 Estrutura do Projeto

```
lauren-dashboard/
├── index.html        # Aplicação completa (HTML + CSS + JS)
├── personagem.png    # Avatar do dashboard
├── .gitignore        # Arquivos ignorados pelo Git
└── README.md         # Este arquivo
```

---

## 💡 Contexto de Desenvolvimento

Este projeto foi criado com auxílio de **IA generativa (Vibecoding)** durante o curso **Sprint IA no Trabalho** da PrograMaria, como exercício prático de desenvolvimento web com inteligência artificial. Todo o processo de criação, iteração e refinamento fez parte do aprendizado.

---

## 👩‍💻 Autora

Feito com 💙 por **Lauren** — 2026  
Curso: [Sprint IA no Trabalho · PrograMaria](https://www.programaria.org)
