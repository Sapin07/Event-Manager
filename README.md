# Event Manager API

API REST em TypeScript/Fastify para inscrições em eventos com validação tipada e documentação automática.

## Proposta

Projeto demonstrativo focado em boas práticas de desenvolvimento backend com TypeScript:
- Configuração do Fastify com TypeScript
- Validação de dados com Zod
- Type safety end-to-end
- Documentação automática com Swagger

**Nota:** Este projeto **não persiste dados**. Os dados recebidos são validados e retornados, mas não são salvos (se desligar o server tudo volta para a estaca zero). Para um projeto real, seria necessário adicionar uma camada de persistência (banco de dados) para armazenar as inscrições, algumas alterações simples e a magia acontece.

## 🛠️ Stack

- TypeScript + Fastify
- Zod (validação)
- Swagger/OpenAPI (documentação)

## 🚀 Como usar

```bash
npm install
npm run dev
```

Servidor: `http://localhost:3333`  
Documentação: `http://localhost:3333/docs`

## API

### POST `/subscriptions`
Inscreve alguém em um evento

**Body:**
```json
{
  "name": "João Silva",
  "email": "joao@example.com"
}
```

**Response (201):**
```json
{
  "name": "João Silva",
  "email": "joao@example.com"
}
```

## ⚙️ Configuração

Opcional - crie `.env`:
```env
PORT=3333
```

---

Projeto educacional focado em TypeScript e validação tipada.
