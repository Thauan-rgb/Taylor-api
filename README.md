# Taylor API 

API REST desenvolvida em Node.js e Express para gerenciamento de músicas da Taylor Swift.

## Requisitos

- Node.js
- npm

## Instalação

Clone o repositório:

```bash
git clone <LINK_DO_REPOSITORIO>
cd taylor-api
```

Instale as dependências:

```bash
npm install
```

## Executando o servidor

Inicie a API:

```bash
node server.js
```

O servidor será iniciado em:

```text
http://localhost:3000
```

## Rotas Disponíveis

### Listar músicas

```http
GET /musicas
```

### Buscar música por ID

```http
GET /musicas/:id
```

### Salvar música

```http
POST /musicas
```

Exemplo de corpo da requisição:

```json
{
  "name": "Love Story",
  "album": "Fearless",
  "lyrics": "Trecho da música"
}
```

### Atualizar avaliação e comentário

```http
PUT /musicas/:id
```

Exemplo:

```json
{
  "nota": 5,
  "comentario": "Excelente música"
}
```

### Excluir música

```http
DELETE /musicas/:id
```

## Tecnologias Utilizadas

- Node.js
- Express
- UUID
- CORS

## Estrutura do Projeto

```text
src/
├── controllers/
├── models/
└── routes/
```
