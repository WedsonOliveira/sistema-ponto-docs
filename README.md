# sistema-ponto-docs
Documentação do Projeto
# 🕒 Sistema de Gerenciamento de Ponto  

Um sistema para cadastro de funcionários, autenticação e registro de ponto, desenvolvido com **Node.js**, **Express**, **PostgreSQL** e **HTML/CSS/JavaScript** no frontend.

---

## 🚀 Funcionalidades  

### 🔹 **Cadastro de Funcionários** 📝  
- Armazena **nome, idade, cargo e senha** no banco de dados.  
- **Senhas criptografadas** com `bcrypt` para maior segurança.  
- Verificação para evitar **senhas duplicadas**.  

### 🔹 **Autenticação de Funcionários** 🔐  
- Login via **senha cadastrada**.  
- Se a senha for válida, exibe **nome e cargo** do funcionário.  
- Caso contrário, impede o acesso ao **registro de ponto**.  

### 🔹 **Registro de Ponto** ⏳  
- Funcionário autenticado pode registrar ponto com **data e hora**.  
- Registro armazenado no **PostgreSQL**.  

### 🔹 **Interface Web Responsiva** 🖥️  
- **Página inicial** com botão para funcionários.  
- Formulários **intuitivos e responsivos**.  
- **Feedback visual** de erro ou sucesso nas ações.  

---

## 🛠️ Tecnologias Utilizadas  

### **Backend**  
- **Node.js** + **Express.js**  
- **PostgreSQL** (Banco de Dados)  
- **bcrypt** (Criptografia de senha)  
- **dotenv** (Gerenciamento de variáveis de ambiente)  
- **CORS** (Permissões de comunicação entre frontend e backend)  

### **Frontend**  
- **HTML5** (Estruturação da página)  
- **CSS3** (Estilização e responsividade)  
- **JavaScript (ES6+)** (Lógica e interatividade)  

---

## 📂 Estrutura do Projeto  

```yaml
sistema-ponto/
│-- public/                # Arquivos frontend (HTML, CSS, JS)
│   │-- index.html         # Página de login e registro de ponto
│   │-- funcionarios.html   # Cadastro de funcionários
│   │-- inicio.html         # Página inicial do sistema
│   │-- styles.css         # Estilos da aplicação
│   │-- scripts.js         # Lógica do frontend
│
│-- server.js              # Servidor Node.js
│-- .env                   # Variáveis de ambiente (dados do banco)
│-- package.json           # Dependências do projeto
│-- README.md              # Documentação
│
└── database/              # Scripts do banco de dados
    ├── schema.sql         # Criação das tabelas
    ├── seed.sql           # Dados iniciais (opcional)

