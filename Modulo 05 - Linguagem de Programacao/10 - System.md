# System

---

## O namespace `System`

`System` é um dos **principais namespaces** do .NET. Ele contém tipos fundamentais usados em praticamente todos os programas.

Ao escrever:

```csharp
using System;
```

Você ganha acesso direto a classes como:

- `Console`
- `String`
- `DateTime`
- `Math`

---

## Exemplo de uso

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.WriteLine("Hoje é: " + DateTime.Now.ToShortDateString());
        Console.WriteLine("PI aproximado: " + Math.PI);
    }
}
```

---

## Por que é importante?

- Quase todo exemplo básico de C# começa com `using System;`.
- Muitos tipos centrais do .NET estão dentro deste namespace.

Saber disso ajuda a entender de onde vêm as classes que você usa o tempo todo.