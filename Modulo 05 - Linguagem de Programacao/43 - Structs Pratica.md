# Structs: prática

---

## Exemplo com método

```csharp
public struct Retangulo
{
    public double Largura;
    public double Altura;

    public double Area()
    {
        return Largura * Altura;
    }
}

static void Main()
{
    Retangulo r = new Retangulo { Largura = 3.0, Altura = 4.0 };
    Console.WriteLine(r.Area()); // 12
}
```

---

## Observações

- Embora structs possam ter métodos, propriedades e construtores, mantenha-os **simples**.
- Evite structs muito grandes, pois a cópia por valor pode se tornar custosa.