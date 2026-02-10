# Valores padrão

---

## O que são valores padrão?

Cada tipo em C# possui um **valor padrão** (default), usado quando uma variável é criada sem inicialização explícita (em campos, arrays, etc.).

Alguns exemplos:

- `int` → `0`
- `double` → `0.0`
- `bool` → `false`
- `char` → `\0` (caractere nulo)
- `string` → `null`

---

## Operador `default`

Você pode obter o valor padrão com a palavra-chave `default`:

```csharp
int numero = default;          // 0
bool ativo = default;          // false
DateTime data = default;       // 01/01/0001
```

Ou explicitando o tipo:

```csharp
int numero = default(int);
```

---

## Por que isso importa?

- Ajuda a entender o estado inicial de variáveis e campos.
- Evita surpresas ao trabalhar com arrays e coleções recém-criadas.