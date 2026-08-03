# Sentinela — Autenticação JWT

Aplicação full stack de autenticação com React, Node.js e Express. Demonstra cadastro, login, hash de senhas, emissão de JWT e proteção de rotas.

## Recursos

- Cadastro e login
- Senhas protegidas com bcrypt
- JWT assinado com expiração de uma hora
- Validação de emissor e audiência
- Middleware para rotas protegidas
- Restauração e encerramento de sessão
- Área autenticada responsiva
- Respostas de erro consistentes

## Executando

```bash
cp .env.example .env
npm install
npm run dev
```

Web: `http://localhost:5173`  
API: `http://localhost:3333`

## Acesso demonstrativo

```text
E-mail: demo@sentinela.dev
Senha: Sentinela123!
```

## Endpoints

```text
POST /api/auth/register
POST /api/auth/login
GET  /api/auth/me
GET  /api/health
```

## Segurança

Defina um `JWT_SECRET` longo e aleatório em produção. Os usuários deste projeto ficam em memória para fins demonstrativos; utilize banco de dados e HTTPS em uma implantação real.

## Referências

- [Express](https://expressjs.com/en/guide/using-middleware/)
- [jsonwebtoken](https://github.com/auth0/node-jsonwebtoken)
- [bcrypt.js](https://github.com/dcodeIO/bcrypt.js)
