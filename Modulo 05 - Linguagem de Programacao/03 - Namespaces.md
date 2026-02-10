# Namespaces

---

## O que é um namespace?

Um **namespace** é uma forma de **organizar** o código em C#, agrupando tipos relacionados (classes, interfaces, enums, etc.).

Ele ajuda a:

- Evitar conflitos de nomes.
- Organizar melhor projetos grandes.
- Indicar a "área" de responsabilidade de uma classe.

---

## Exemplo

```csharp
namespace MeuProjeto.SistemaDePedidos
{
    class Pedido
    {
        // ...
    }
}
```

Aqui:

- `MeuProjeto.SistemaDePedidos` é o namespace.
- `Pedido` é a classe dentro desse namespace.

---

## Usando namespaces no código

Para usar uma classe de outro namespace, você pode:

1. Escrever o nome completo (namespace + tipo):

```csharp
var data = System.DateTime.Now;
```

2. Ou importar o namespace com `using` (ver próxima aula):

```csharp
using System;

class Program
{
    static void Main()
    {
        Console.WriteLine(DateTime.Now);
    }
}
```

---

## Organização por namespaces

Boas práticas comuns:

- Usar o nome da **empresa** ou **projeto** como raiz (ex.: `MinhaEmpresa.Produto.Modulo`).
- Criar namespaces que representem **módulos** ou **camadas** (ex.: `MinhaApp.Data`, `MinhaApp.Services`).