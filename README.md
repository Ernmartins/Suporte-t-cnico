SmartHelp – Sistema Inteligente de Tickets de Suporte Técnico

Projeto Final – Curso de Técnico de Helpdesk
Plataforma web moderna para abertura, gestão e monitorização de tickets com:
✔ Firebase Firestore
✔ Firebase Authentication
✔ Firebase Storage
✔ Dashboard com gráficos
✔ Login técnico
✔ Consulta de estado do ticket

🚀 Funcionalidades Principais
👤 1. Portal do Cliente

Enviar tickets de suporte técnico

ID automático no formato TCK-0001

Campos: nome, email, telefone, categoria, prioridade, descrição

Maior área para descrição detalhada

Interface moderna (tema dark)

Suporte a anexos (imagens, PDFs)

🔐 2. Login Técnico (Firebase Auth)

Página exclusiva de login (login.html)

Acesso seguro com email + password

Sessão persistente

Após login → redireciona para painel do técnico

Logout disponível a qualquer momento

🧑‍🔧 3. Painel do Técnico (Admin)

Listagem de todos os tickets

Cores diferentes conforme estado: Aberto, Em andamento, Resolvido

Filtros por categoria e prioridade

Atualizar estado do ticket (dropdown)

Registar ações internas (notas técnicas)

Ver anexos enviados pelo cliente

Botão de Logout

📊 4. Dashboard com Gráficos (Chart.js)

Página dashboard.html inclui:

Gráfico de tickets por estado

Gráfico de tickets por categoria

Gráfico de tickets por prioridade

Atualização em tempo real (Firestore Listener)

🔍 5. Página de Consulta de Ticket por ID

(consultar-ticket.html)

Cliente insere ID (ex.: TCK-0032)

Sistema retorna:

Estado

Prioridade

Categoria

Técnico responsável (opcional)

Data

Descrição resumida

Indicador visual das fases (barra de progresso)

📁 6. Upload de Ficheiros (Firebase Storage)

Agora o cliente pode anexar:

Imagens

PDFs

Prints de erros

No painel técnico o administrador pode:

Visualizar

Fazer download

Apagar anexos

🛠 Tecnologias Utilizadas

HTML5 + CSS3 (tema dark profissional)

JavaScript ES Modules

Firebase 11

Authentication

Firestore Database

Storage

Chart.js para gráficos

GitHub Pages para publicação

📂 Estrutura do Projeto
suporte-tecnico/
│
├── index.html                (Portal Cliente – abrir ticket)
├── login.html                (Login técnico)
├── admin.html                (Painel técnico)
├── atualizar-ticket.html     (Alterar estado do ticket)
├── consultar-ticket.html     (Cliente consulta ticket)
├── dashboard.html            (Gráficos)
│
├── firebase.js               (Configuração Firebase)
├── auth.js                   (Lógica de login/logout)
├── admin.js                  (Gestão de tickets)
├── consulta.js               (Consultar ticket)
├── dashboard.js              (Gráficos)
│
├── style.css                 (Tema dark global)
│
├── /uploads                  (Pasta local opcional)
└── README.md                 (Documentação completa)

🔧 Como Instalar
1️⃣ Clonar o repositório
git clone https://github.com/teu-usuario/suporte-tecnico.git
cd suporte-tecnico

2️⃣ Configurar Firebase

Ir a:
👉 https://console.firebase.google.com

Criar:
✔ Projeto
✔ Firestore
✔ Authentication (Email/Password)
✔ Storage

Copiar o firebaseConfig e colar em firebase.js.

3️⃣ Ativar Regras Temporárias

Para testes iniciais:

allow read, write: if true;


⚠️ Depois do projeto, mudar para regras seguras.

🔑 Login Técnico – Como funciona

Criar um utilizador manualmente no Firebase Auth

Entrar via página login.html

Se o login falhar → mensagem de erro

Se tiver sucesso → entra no painel (admin.html)

Logout através do botão no header

Redirecionamento automático caso o técnico não esteja autenticado

🧪 Testes Realizados

Envio de ticket no portal cliente

Escrita e leitura Firestore

Upload de ficheiros para Storage

Atualização do estado

Autenticação técnico

Consulta de ticket por ID

Dashboard atualizado em tempo real

Responsividade mobile

🧠 Apreciação Crítica

O sistema entrega:
✔ Organização profissional
✔ Experiência real de Helpdesk
✔ Inteligência de estrutura
✔ Base de dados sempre sincronizada
✔ Interface moderna e intuitiva

Pontos de melhoria:

Sistema de notificações por email

Comentários técnico-cliente

Exportação de relatórios PDF

⭐ Autoavaliação
Aspeto	Nota
Organização	⭐⭐⭐⭐⭐
Criatividade	⭐⭐⭐⭐⭐
Código	⭐⭐⭐⭐
Aprendizagem	⭐⭐⭐⭐⭐
Documentação	⭐⭐⭐⭐⭐
📄 Licença

Uso académico.
Não utilizar comercialmente sem autorização.
