# Alias

---

## O que é um alias de tipo?

Em C#, alguns tipos possuem **apelidos (alias)** mais simples.

Exemplos:

- `int` é alias para `System.Int32`.
- `string` é alias para `System.String`.
- `bool` é alias para `System.Boolean`.

Ou seja, o código abaixo é equivalente:

```csharp
int x = 10;
System.Int32 y = 20;
```

---

## Alias com `using`

Você também pode criar aliases personalizados para tipos ou namespaces longos:

```csharp
using ColecaoDeStrings = System.Collections.Generic.List<string>;

ColecaoDeStrings nomes = new ColecaoDeStrings();
```

Isso pode melhorar a legibilidade em alguns cenários específicos.