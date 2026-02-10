# Using

---

## O que é `using`?

O `using` em C# tem **dois usos principais**:

1. **Importar namespaces** para facilitar o uso de tipos.
2. Criar um **bloco de uso** de recursos que precisam ser descartados corretamente.

---

## 1. Importar namespaces

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.WriteLine("Olá, mundo!");
    }
}
```

Sem o `using System;`, você teria que escrever `System.Console.WriteLine` toda vez.

---

## 2. Using para descarte de recursos

Usado com tipos que implementam `IDisposable` (arquivos, conexões, streams):

```csharp
using (var arquivo = new StreamWriter("log.txt"))
{
    arquivo.WriteLine("Mensagem de log");
}
// Aqui o arquivo é fechado automaticamente
```

Nesse caso, ao sair do bloco `using`, o recurso é liberado automaticamente.

---

## Boas práticas

- Importe apenas os namespaces que realmente precisa.
- Use o `using` de descarte para lidar com recursos externos (arquivo, rede, banco de dados).