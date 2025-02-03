# **Teste para Desenvolvedor Backend Laravel**

## 📌 **Aplicação SOLID**

### 🎯 **Objetivo**
O objetivo deste teste é desenvolver uma **API REST** utilizando **Laravel**, garantindo a aplicação de **boas práticas de desenvolvimento, arquitetura limpa e princípios SOLID**.

A API deve ser um **CRUD (criação, edição, visualização e exclusão)** de **Domínios e Blocos**, onde um **Domínio pode ter vários Blocos (one-to-many)**.

O candidato deve implementar os seguintes conceitos e padrões:
- ✅ **Princípios SOLID**
- ✅ **Migrations**
- ✅ **Repositories com Interface**
- ✅ **Services para regras de negócio**
- ✅ **DTOs (Data Transfer Object) para entrada e saída**
- ✅ **Enrichers para enriquecer respostas da API**
- ✅ **Formaters para padronizar as saídas de dados**
- ✅ **Validações de entrada**
- ✅ **Estrutura desacoplada seguindo boas práticas**

---

## 📌 **Requisitos**

### 📂 **Backend (Laravel)**

#### **1️⃣ Configuração**
- Configure um **projeto Laravel do zero** utilizando **MySQL como banco de dados**.
- Utilize **Eloquent ORM e migrations** para gerenciamento das tabelas.

#### **2️⃣ Estrutura de Dados**

A estrutura do banco de dados deve conter as seguintes tabelas:

##### **🔹 Tabela `domains` (Domínios)**
- `id` (INT) → Identificador único do domínio
- `name` (STRING) → Nome do domínio

##### **🔹 Tabela `blocks` (Blocos)**
- `id` (INT) → Identificador único do bloco
- `name` (STRING) → Nome do bloco
- `domain_id` (INT) → Relacionamento com um `domain`

#### **3️⃣ Relacionamentos**
- Um **Domínio** pode ter **vários Blocos** (**One-to-Many**).
- A deleção de um **Domínio** deve remover automaticamente os **Blocos** associados (**cascade delete**).

#### **4️⃣ Rotas da API**

##### **🔹 Domínios (`domains`)**
- **`GET /api/domains`** → Lista todos os domínios.
- **`POST /api/domains`** → Cria um novo domínio.
- **`PUT /api/domains/{id}`** → Atualiza um domínio existente.
- **`DELETE /api/domains/{id}`** → Exclui um domínio.

##### **🔹 Blocos (`blocks`)**
- **`GET /api/blocks`** → Lista todos os blocos.
- **`POST /api/blocks`** → Cria um novo bloco.
- **`PUT /api/blocks/{id}`** → Atualiza um bloco existente.
- **`DELETE /api/blocks/{id}`** → Exclui um bloco.

---

## 📌 **Instruções para subir no GitHub**

1️⃣ **Criar um repositório público** no **GitHub**.

2️⃣ **Criar um arquivo README.md** no repositório contendo **instruções detalhadas** sobre como clonar o repositório, instalar dependências e rodar o projeto.

3️⃣ O **README.md** deve conter:
- Como clonar o repositório.
- Instruções para rodar o backend, incluindo instalação de dependências, configuração do ambiente e execução do projeto.

4️⃣ **Banco de Dados**
- Utilizar **MySQL** como banco de dados.
- Configurar o projeto para rodar corretamente com as **migrations do Laravel**.

5️⃣ **Garantia de execução**
- Verificar se todas as instruções no **README.md** são suficientes para que qualquer pessoa consiga rodar o projeto sem dificuldades.

---

## 📌 **Instruções para a Documentação da API**

1️⃣ Criar uma **coleção no Postman** contendo todas as **rotas da API devidamente configuradas**.

2️⃣ Incluir dentro da coleção as requisições para todas as operações do CRUD, garantindo que cada rota seja testável de forma simples.

3️⃣ Configurar cada requisição com um **body formatado corretamente** para criação e atualização de dados.

4️⃣ Exportar a coleção do **Postman** em um arquivo **JSON** e incluí-lo dentro do repositório, para que qualquer pessoa possa importar e testar as rotas rapidamente.

---

## 📌 **Critérios de Avaliação**

1️⃣ **Funcionalidade**
- O sistema deve **funcionar corretamente** com todas as operações de CRUD para **Domínios e Blocos**.

2️⃣ **Boas Práticas de Código**
- **Backend (Laravel)**: Uso adequado de **controllers, services, repositories, rotas, validações e migrations**.

3️⃣ **Organização do Código**
- O código deve ser **claro, modular e bem estruturado**.

4️⃣ **Documentação no GitHub**
- O repositório deve estar **organizado**.
- O **README.md** deve conter **todas as instruções necessárias** para rodar o projeto corretamente.

---

### **📌 Observação Importante**
⚠️ O teste **será considerado inválido** se as instruções no **README.md** **não forem suficientes** para rodar o projeto corretamente.  
✅ Antes de enviar, **teste o projeto** em um ambiente limpo seguindo as instruções do **README.md** para garantir que tudo esteja funcionando!  

🚀 **Boa sorte e bom desenvolvimento!** 🚀  
