# 🐾 PetNet - Frontend

## 📋 Sobre o Projeto
O **PetNet** é uma plataforma voltada para pet shops, criada para facilitar a **prospecção e gestão de serviços**.  
Nesta primeira sprint, o foco foi no **frontend** do sistema, com base em um novo fluxo de agendamento, onde o cliente seleciona o serviço e é redirecionado para o **WhatsApp**, enquanto o **gerente** finaliza o agendamento manualmente.

## 👥 Equipe
- Beatriz Barbosa Moscardini  
- Guilherme Fagundes Framil  
- Mariana Guerra Ferraz  
- Rafaela Campos Corrêa Santos  
- Wagner Campos Pacheco Bernardes dos Santos  

---

## 🎯 Objetivo da Sprint
- Atualizar requisitos do sistema  
- Definir páginas e componentes do front-end  
- Estruturar o projeto em React  
- Estabelecer paleta de cores, fontes e stack mínima  

---

## 🖥️ Telas Prototipadas
O front-end foi modelado com base nas seguintes telas e fluxos principais:

| Página / Componente | Descrição |
|----------------------|------------|
| **Landing Page** | Apresentação dos serviços e acesso aos cadastros |
| **Cadastro de Usuário** | Formulário para cadastro do cliente |
| **Cadastro de Pet** | Tela para adicionar informações do pet |
| **Agendamento** | Exibição dos serviços e botão de contato via WhatsApp |
| **Admin / Painel do Gerente** | Controle de pets, usuários e agendamentos |
| **Cards (Pet, Usuário, Serviço)** | Componentes reutilizáveis para listagens |

> 💡 *Cada uma dessas telas foi representada nos protótipos da Sprint 01.*

---

## 🗂️ Estrutura de Pastas
```
PETNET-FRONTEND/
│── public/              # Arquivos públicos (favicon, index.html, imagens globais)
│
└── src/
    ├── assets/          # Imagens, ícones, fontes
    ├── components/      # Componentes reutilizáveis
    │   ├── common/      # Botões, inputs, modais
    │   ├── layout/      # Navbar, footer, sidebar
    │   └── cards/       # CardPet, CardUser, CardService
    │
    ├── pages/           # Páginas principais
    │   ├── landing/
    │   ├── cadastroUser/
    │   ├── cadastroPet/
    │   ├── agendamento/
    │   └── admin/
    │       ├── pets/
    │       ├── users/
    │       └── agendamentos/
    │
    ├── services/        # Comunicação com o backend (API)
    │   ├── api.js
    │   ├── pets.js
    │   ├── users.js
    │   └── agendamentos.js
    │
    ├── hooks/           # Hooks personalizados
    ├── context/         # Context API para estados globais
    ├── styles/          # Estilos globais e variáveis
    ├── router/          # Definição de rotas
    ├── utils/           # Funções auxiliares (formatadores, validações)
    ├── App.jsx
    └── main.jsx
```

---

## ⚙️ Stack Utilizada
| Categoria | Tecnologias |
|------------|--------------|
| **Base do Projeto** | React + Vite |
| **Roteamento** | React Router |
| **Requisições** | Axios / React Query |
| **Formulários e Validação** | React Hook Form + Zod |
| **Estilização** | TailwindCSS + Material UI Icons |
| **Datas** | Day.js |
| **Qualidade de Código** | ESLint + Prettier + Husky |

---

## 🎨 Design System

**Paleta de cores:**
| Cor | Código |
|------|---------|
| Azul principal | `#3370EB` |
| Amarelo destaque | `#F9EE7C` |
| Branco | `#FFFFFF` |
| Preto | `#000000` |

**Fontes utilizadas:**
| Fonte | Uso |
|--------|-----|
| Montserrat | Títulos |
| Roboto | Textos corridos |
| Open Sans | Subtítulos / labels |
| Source Code Pro | Números / tabelas |

---

## 🧠 Regras de Negócio (Resumo)
- O agendamento é realizado apenas pelo gerente (via WhatsApp).  
- Colaboradores só podem mudar o status para “Em andamento” ou “Finalizado”.  
- Clientes não realizam agendamentos de forma autônoma.  
- O sistema deve exibir status e validar e-mails obrigatoriamente.  

---

## 🚀 Como Executar o Projeto

```bash
# Clonar o repositório
git clone https://github.com/seu-usuario/petnet-frontend.git

# Acessar a pasta
cd petnet-frontend

# Instalar dependências
npm install

# Rodar o projeto
npm run dev
```

---

## 📸 Protótipos
(https://www.figma.com/design/ZWN7I2H0pkGLh5n4YCt7iJ/PETNET?node-id=0-1&t=Q9pl4mEeGBX3fPmF-1)

---

## 🧩 Próximos Passos
- Integração com backend (API PetNet)  
- Implementação das páginas dinâmicas  
- Controle de autenticação e proteção de rotas  

---
