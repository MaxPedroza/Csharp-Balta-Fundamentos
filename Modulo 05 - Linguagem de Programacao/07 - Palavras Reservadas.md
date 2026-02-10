# Palavras reservadas

---

## O que são palavras reservadas?

São palavras que têm **significado especial** para a linguagem C# e **não podem ser usadas como nomes de variáveis, métodos ou classes** (a menos que com escape específico).

Exemplos:

- `int`, `string`, `class`, `namespace`, `if`, `else`, `for`, `return`, `using`.

---

## Por que existem?

- Para definir a **sintaxe** da linguagem.
- Para indicar **comandos** e **estruturas** específicas.

---

## Evitando conflitos

Não tente usar palavras reservadas como nomes de variáveis:

```csharp
int class = 10; // ERRO
```

Se for absolutamente necessário (casos especiais, interoperabilidade), é possível usar `@` antes do nome:

```csharp
int @class = 10; // válido, mas não recomendado
```

---

## Dica

Conforme você programa, rapidamente memoriza as principais palavras reservadas. Não é preciso decorar listas enormes; o importante é reconhecer quando o compilador reclamar.