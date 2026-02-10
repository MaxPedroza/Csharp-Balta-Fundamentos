# Convert

---

## A classe `Convert`

A classe estática `System.Convert` fornece métodos para conversão entre tipos.

Exemplo:

```csharp
string texto = "30";
int idade = Convert.ToInt32(texto);

double valor = Convert.ToDouble("10,5");
bool ativo = Convert.ToBoolean("true");
```

---

## Diferença para `Parse`

- `Parse` normalmente é específico de um tipo (`int.Parse`, `double.Parse`).
- `Convert` funciona de forma genérica para vários tipos.

Alguns métodos de `Convert` tratam `null` de forma especial (por exemplo, retornando `0` para `ToInt32(null)`).

---

## Quando usar

- Quando precisa de conversão rápida entre vários tipos diferentes.
- Quando quer um comportamento um pouco mais flexível com valores `null`.