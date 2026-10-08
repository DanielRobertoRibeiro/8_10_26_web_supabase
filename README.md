Gerenciador de Produtos com React e Supabase

Aplicação web desenvolvida em React integrada ao Supabase para gerenciamento e cadastro de produtos em tempo real.

🚀 Tecnologias Utilizadas

React (com Hooks: useState, useEffect)

Supabase (Banco de dados PostgreSQL e cliente JavaScript)

JavaScript (ES6+)

HTML5 / CSS

📋 Pré-requisitos

Antes de iniciar, certifique-se de ter instalado em sua máquina:

Node.js (versão 16 ou superior recomendada)

Um gerenciador de pacotes como npm ou yarn

⚙️ Configuração do Supabase

Crie uma conta e um projeto no Supabase.

No painel do Supabase, crie uma tabela chamada produtos com a seguinte estrutura sugerida:

id (UUID ou Integer, Chave Primária)

created_at (Timestamp)

name (Text)

description (Text)

Configure o seu arquivo de conexão (supabaseClient.js) com as suas credenciais (SUPABASE_URL e SUPABASE_ANON_KEY).

📦 Instalação e Execução

Clone o repositório:

git clone https://github.com/DanielRobertoRibeiro/8_10_26_web_supabase.git
cd 8_10_26_web_supabase


Instale as dependências:

npm install


Inicie o servidor de desenvolvimento:

npm run dev


(ou o comando equivalente configurado no seu package.json para iniciar a aplicação React).

🛠️ Funcionalidades

Listagem Dinâmica: Busca e exibe todos os produtos cadastrados no banco de dados Supabase ao carregar a aplicação.

Cadastro de Produtos: Formulário preparado para adicionar novos itens com nome e descrição.

Tratamento de Erros: Gestão de estados de carregamento (loading) e captura de exceções durante as requisições assíncronas.
