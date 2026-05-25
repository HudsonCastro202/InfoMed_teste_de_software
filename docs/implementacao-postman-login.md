# Implementação do Teste no Postman

## Endpoint

POST http://localhost/login

---

# Body

```json
{
  "email": "teste@exdex.com",
  "senha": "123456"
}
```

---

# Script de Teste

```javascript
pm.test("Status code is 200", function () {
    pm.response.to.have.status(200);
});
```