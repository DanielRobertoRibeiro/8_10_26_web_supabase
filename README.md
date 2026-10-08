# 📦 Gerenciamento de Produtos com React & Supabase

Aplicação web moderna desenvolvida em **React** e integrada ao **Supabase**, projetada para gerenciar um catálogo de produtos de forma simples, eficiente e responsiva.

---

## 🚀 Tecnologias Utilizadas

- **React** (Hooks: `useState`, `useEffect`)
- **Supabase** (Banco de dados PostgreSQL e cliente JavaScript)
- **JavaScript (ES6+)**
- **HTML5 & CSS / Tailwind CSS** (conforme estilização aplicada)

---

## 📋 Funcionalidades

- **Listagem em Tempo Real:** Busca todos os produtos cadastrados na tabela `produtos` do Supabase ao carregar a aplicação.
- **Tratamento de Estados:** Gerenciamento visual de estados de carregamento (*loading*) e captura de erros.
- **Cadastro de Novos Itens:** Formulário preparado para adicionar novos produtos contendo nome e descrição (`newItemName` e `newItemDescription`).

---

## ⚙️ Pré-requisitos

Antes de clonar e rodar o projeto, certifique-se de ter instalado em sua máquina:
- [Node.js](https://nodejs.org/) (versão 16 ou superior recomendada)
- Um gerenciador de pacotes como **npm** ou **yarn**
- Uma conta e um projeto configurado no [Supabase](https://supabase.com/)

---

## 🛠️ Instalação e Execução

1. **Clone o repositório:**
   ```bash
   git clone https://github.com/DanielRobertoRibeiro/8_10_26_web_supabase.git
   cd 8_10_26_web_supabase
   ```

2. **Instale as dependências:**
   ```bash
   npm install
   ```

3. **Configure o Supabase:**
   Certifique-se de que o arquivo `supabaseClient.js` está configurado corretamente com suas credenciais do projeto Supabase:
   ```javascript
   import { createClient } from '@supabase/supabase-js'

   const supabaseUrl = 'SUA_URL_DO_SUPABASE'
   const supabaseKey = 'SUA_CHAVE_ANON_DO_SUPABASE'

   export const supabase = createClient(supabaseUrl, supabaseKey)
   ```

4. **Execute o projeto em modo de desenvolvimento:**
   ```bash
   npm run dev
   # ou
   npm start
   ```

---

## 🗄️ Estrutura do Banco de Dados (Supabase)

Para que a aplicação funcione perfeitamente, certifique-se de criar uma tabela chamada `produtos` no seu banco de dados Supabase com, no mínimo, as seguintes colunas:
- `id` (Chave primária / UUID ou Serial)
- `created_at` (Timestamp com fuso horário)
- `name` (Texto - Nome do produto)
- `description` (Texto - Descrição do produto)

---

## 📝 Contribuição

Contribuições, sugestões de melhorias e *pull requests* são sempre bem-vindos! Sinta-se à vontade para abrir uma issue ou enviar melhorias.

---

## 📄 Licença

Este projeto está sob a licença MIT. Sinta-se livre para utilizá-lo em seus estudos e projetos pessoais.
