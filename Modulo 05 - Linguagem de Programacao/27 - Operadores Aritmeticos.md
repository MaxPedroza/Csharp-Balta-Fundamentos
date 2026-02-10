# Operadores aritméticos

---

## Principais operadores

| Operador | Descrição   | Exemplo      |
|----------|------------|--------------|
| `+`      | soma        | `a + b`      |
| `-`      | subtração   | `a - b`      |
| `*`      | multiplicação | `a * b`    |
| `/`      | divisão     | `a / b`      |
| `%`      | módulo (resto) | `a % b`   |

---

## Exemplo em código

```csharp
int a = 10;
int b = 3;

int soma = a + b;        // 13
int sub = a - b;         // 7
int mult = a * b;        // 30
int div = a / b;         // 3 (divisão inteira)
int resto = a % b;       // 1
```

---

## Atenção à divisão inteira

Se ambos os operandos forem inteiros, o resultado será inteiro. Para obter resultado real:

```csharp
double resultado = 10.0 / 3.0; // ~3,3333
```