# Operadores de comparação

---

## Principais operadores

| Operador | Descrição              | Exemplo   |
|----------|------------------------|-----------|
| `==`     | igual a                | `a == b`  |
| `!=`     | diferente de           | `a != b`  |
| `>`      | maior que              | `a > b`   |
| `<`      | menor que              | `a < b`   |
| `>=`     | maior ou igual         | `a >= b`  |
| `<=`     | menor ou igual         | `a <= b`  |

---

## Retorno booleano

Todas as comparações retornam um `bool` (`true` ou `false`):

```csharp
int a = 10;
int b = 20;

bool resultado = a < b; // true
```

Esses resultados são usados em `if`, `while`, etc.