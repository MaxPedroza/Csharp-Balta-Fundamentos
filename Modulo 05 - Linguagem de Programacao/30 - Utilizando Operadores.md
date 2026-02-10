# Utilizando operadores

---

## Combinando operadores

Na prática, você combina operadores aritméticos, de atribuição e de comparação para construir expressões.

```csharp
int a = 10;
int b = 5;

bool resultado = (a + b) > 10; // true
```

---

## Precedência de operadores

Algumas regras de precedência (ordem de avaliação):

1. Parênteses `()`
2. Multiplicação e divisão `*` `/` `%`
3. Soma e subtração `+` `-`
4. Comparações `==`, `!=`, `>`, `<`, `>=`, `<=`
5. Lógicos `&&`, `||`

Use sempre **parênteses** para deixar claro o que você quer calcular.

---

## Exemplo completo

```csharp
int idade = 20;
int pontos = 50;

bool podeEntrar = (idade >= 18) && (pontos >= 40);
```

Aqui usamos operadores de comparação e lógicos juntos.