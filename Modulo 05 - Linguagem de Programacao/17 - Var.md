# var

---

## O que é `var`?

`var` permite que o **compilador deduza o tipo** da variável com base no valor atribuído.

```csharp
var idade = 30;          // tipo inferido: int
var nome = "Maria";     // tipo inferido: string
var ativo = true;        // tipo inferido: bool
```

`var` não é um tipo dinâmico; o tipo é fixado em tempo de compilação.

---

## Quando usar `var`?

- Quando o tipo é **óbvio** pela atribuição.
- Quando o tipo é muito longo ou genérico (ex.: tipos de LINQ).

```csharp
var lista = new List<string>();
```

---

## Quando evitar

- Quando o uso de `var` deixa o código confuso, escondendo o tipo real.

Boas práticas recomendam equilíbrio: use `var` para melhorar a legibilidade, não para escondê-la.