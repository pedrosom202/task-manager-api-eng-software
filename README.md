# 🧩 Task Manager API

## 📌 Sobre o projeto

Este projeto é uma API simples para gerenciamento de tarefas.

Ela permite:

* Criar tarefas
* Listar tarefas
* Atualizar tarefas
* Deletar tarefas

O principal objetivo não é a complexidade do sistema, mas sim demonstrar o uso correto do **Git** com boas práticas de versionamento e fluxo de trabalho profissional.

---

## 🎯 Problema que resolve

Antes, a equipe trabalhava sem controle de versão adequado:

* Arquivos ZIP com nomes confusos 😬
* Dificuldade para saber quem fez alterações
* Bugs reaparecendo frequentemente

Com este projeto, aplicamos:

* Controle de versão com Git
* Organização com branches
* Histórico claro de mudanças

---

## 🚀 Tecnologias utilizadas

* Node.js
* Express
* UUID (para gerar IDs)
* Git

---

## ▶️ Como rodar o projeto

### 1. Clonar o repositório

```bash
git clone <URL_DO_REPOSITORIO>
```

### 2. Entrar na pasta

```bash
cd task-manager-api
```

### 3. Instalar dependências

```bash
npm install
```

### 4. Rodar o projeto

```bash
npm run dev
```

O servidor estará disponível em:

```
http://localhost:3000
```

---

## 📡 Endpoints da API

### Criar tarefa

**POST** `/api/tasks`

Exemplo de body:

```json
{
  "title": "Estudar Git"
}
```

---

### Listar tarefas

**GET** `/api/tasks`

---

### Atualizar tarefa

**PUT** `/api/tasks/:id`

Exemplo:

```json
{
  "title": "Estudar Git avançado",
  "completed": true
}
```

---

### Deletar tarefa

**DELETE** `/api/tasks/:id`

---

## 🌿 Estratégia de branches

Utilizamos uma estrutura inspirada no Git Flow:

* `main` → versão em produção
* `develop` → integração das funcionalidades
* `feature/*` → desenvolvimento de novas funcionalidades
* `hotfix/*` → correções urgentes em produção

---

## 🔄 Fluxo de desenvolvimento

1. Criar uma branch a partir da `develop`

```
feature/nome-da-feature
```

2. Desenvolver a funcionalidade

3. Fazer commits organizados

4. Abrir um Pull Request

5. Fazer merge na `develop`

6. Quando pronto, fazer release para `main`

---

## 📝 Padrão de commits

Seguimos um padrão simples e organizado:

* `feat:` nova funcionalidade
* `fix:` correção de bug
* `docs:` documentação
* `refactor:` melhoria no código
* `test:` testes

### Exemplos:

```
feat: adiciona criação de tarefas
fix: corrige erro ao deletar tarefa
docs: atualiza README
```

---

## 🏷️ Versionamento

Utilizamos versionamento semântico:

* `v1.0.0` → primeira versão estável
* `v1.1.0` → novas funcionalidades
* `v1.1.1` → correções de bugs

As versões são marcadas com **tags no Git**.

---

## 🧯 Correções urgentes (Hotfix)

Quando um bug aparece em produção:

1. Criar branch a partir da `main`

```
hotfix/nome-do-bug
```

2. Corrigir o problema

3. Fazer merge em:

* `main`
* `develop`

---

## 📁 Estrutura do projeto

```
src/
  controllers/   → recebe as requisições
  services/      → regras de negócio
  routes/        → definição das rotas
  app.js         → inicialização do servidor
```

---

## 🧪 Como testar

Você pode usar:

* Postman
* Insomnia
* curl

Exemplo com curl:

```bash
curl -X POST http://localhost:3000/api/tasks \
-H "Content-Type: application/json" \
-d '{"title": "Teste"}'
```

---

## 🤝 Como contribuir

1. Fazer um fork do projeto
2. Criar uma branch:

```
feature/minha-feature
```

3. Fazer commits seguindo o padrão
4. Enviar para o repositório
5. Abrir um Pull Request

---

## 📌 Status do projeto

🚧 Em desenvolvimento

---

## 👨‍💻 Objetivo acadêmico

Este projeto foi desenvolvido com foco em:

* Aprender Git na prática
* Simular ambiente profissional
* Organizar fluxo de trabalho em equipe

---

## 📄 Licença

Este projeto é livre para uso educacional.
