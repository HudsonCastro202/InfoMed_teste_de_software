# Modelagem — Teste de Interface Login

## Técnica Utilizada
Tabela de Decisão

| Regra | CT01 | CT02 |
|---|---|---|
| Email válido | S | N |
| Senha válida | S | N |
| Resultado esperado | Login realizado | Login inválido |

---

# Casos de Teste

## CT01 — Login válido

| Campo | Valor |
|---|---|
| E-mail | teste@exdex.com |
| Senha | 123456 |

Resultado esperado:
Login realizado

---

## CT02 — Login inválido

| Campo | Valor |
|---|---|
| E-mail | errado@erro.com |
| Senha | 111111 |

Resultado esperado:
Login inválido