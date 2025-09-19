# Express + TypeScript API

Este é um projeto API REST usando Express.js e TypeScript com endpoint de health check.

## 🚀 Quick Start

### 1. Instalar Dependências
```bash
npm install
```

### 2. Desenvolvimento
```bash
npm run dev
```

### 3. Build para Produção
```bash
npm run build
npm start
```

## 📚 Scripts Disponíveis

- `npm run dev` - Inicia servidor em modo desenvolvimento com hot reload
- `npm run build` - Compila TypeScript para JavaScript
- `npm start` - Inicia servidor de produção
- `npm run lint` - Executa ESLint
- `npm run lint:fix` - Corrige problemas de linting automaticamente

## 🔗 Endpoints

### Health Check
```
GET /health
```
**Resposta:**
```json
{
  "status": "OK",
  "timestamp": "2025-09-19T10:30:00.000Z",
  "uptime": 123.456,
  "environment": "development",
  "version": "1.0.0",
  "service": "my-project-api"
}
```

### Root
```
GET /
```
**Resposta:**
```json
{
  "message": "Welcome to Express + TypeScript API!",
  "version": "1.0.0",
  "endpoints": {
    "health": "/health",
    "root": "/"
  }
}
```

## 🛠️ Tecnologias

- **Express.js** - Framework web
- **TypeScript** - Superset tipado do JavaScript
- **ESLint** - Linter para qualidade de código
- **ts-node-dev** - Desenvolvimento com hot reload

## 📁 Estrutura do Projeto

```
├── src/
│   └── index.ts          # Servidor principal
├── dist/                 # Arquivos compilados (gerado automaticamente)
├── package.json          # Dependências e scripts
├── tsconfig.json         # Configuração TypeScript
├── .eslintrc.json        # Configuração ESLint
└── README.md             # Este arquivo
```

## 🌍 Variáveis de Ambiente

- `PORT` - Porta do servidor (padrão: 3000)
- `NODE_ENV` - Ambiente (development/production)

## 🚀 Deploy

O projeto está pronto para deploy. Após build, execute:

```bash
npm start
```

O servidor estará disponível na porta especificada pela variável `PORT` ou 3000 por padrão.