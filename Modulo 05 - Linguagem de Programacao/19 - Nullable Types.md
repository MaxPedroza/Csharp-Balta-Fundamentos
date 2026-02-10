# Nullable types

---

## Problema

Tipos de valor (como `int`, `double`, `bool`) **não aceitam `null`** por padrão.

Mas e quando um valor realmente pode "não existir"? Ex.: idade de alguém não informada.

---

## Solução: tipos anuláveis

Use `?` após o tipo:

```csharp
int? idade = null;

if (idade.HasValue)
{
    Console.WriteLine(idade.Value);
}
```

- `HasValue` indica se há um valor.
- `Value` acessa o valor (cuidado, só use se tiver certeza de que não é nulo).

---

## Operador de coalescência nula

```csharp
int idadeReal = idade ?? 0; // se idade for null, usa 0
```

---

## Importância

Tipos anuláveis ajudam a **modelar melhor** a realidade e evitam o uso de "valores mágicos" como `-1` para representar "não informado".