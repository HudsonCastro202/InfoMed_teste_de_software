# Documentação da API — Login

## Endpoint

POST /login

---

# Descrição

Responsável pela autenticação do usuário no sistema.

---

# Requisição

## Headers

Content-Type: application/json

---

# Body

```json
{
  "email": "teste@exdex.com",
  "senha": "123456"
}
```

---

# Respostas

## 200 — Sucesso

```json
{
  "status": "sucesso",
  "mensagem": "Login realizado"
}
```

---

## 401 — Erro

```json
{
  "status": "erro",
  "mensagem": "E-mail ou senha inválidos"
}
```