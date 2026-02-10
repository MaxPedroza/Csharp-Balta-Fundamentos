# Estrutura condicional: switch

---

## Quando usar `switch`?

Use `switch` quando tiver muitas condições baseadas **no mesmo valor**.

---

## Exemplo

```csharp
string dia = "Segunda";

switch (dia)
{
    case "Segunda":
    case "Terca":
    case "Quarta":
    case "Quinta":
    case "Sexta":
        Console.WriteLine("Dia útil");
        break;

    case "Sabado":
    case "Domingo":
        Console.WriteLine("Fim de semana");
        break;

    default:
        Console.WriteLine("Dia inválido");
        break;
}
```

---

## Versões modernas

Em versões mais novas do C#, há recursos adicionais como **switch expression**, mas o `switch` tradicional ainda é muito utilizado e importante de entender.