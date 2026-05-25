# Modelagem de Teste de API — Login

## Técnica Utilizada
Particionamento de Equivalência

| Partição | Entrada | Resultado Esperado |
|---|---|---|
| P1 | Email inválido | Erro |
| P2 | Senha inválida | Erro |
| P3 | Dados válidos | Sucesso |

---

# Casos de Teste

## CT01

```json
{
  "email": "teste.com",
  "senha": "123456"
}
```

Resultado esperado:
Email inválido

---

## CT02

```json
{
  "email": "teste@exdex.com",
  "senha": "111111"
}
```

Resultado esperado:
Senha inválida

---

## CT03

```json
{
  "email": "teste@exdex.com",
  "senha": "123456"
}
```

Resultado esperado:
Login realizado