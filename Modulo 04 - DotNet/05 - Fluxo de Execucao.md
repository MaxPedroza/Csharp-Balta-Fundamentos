# Fluxo de execução de um app .NET

---

## Do código ao programa rodando

Quando você executa uma aplicação .NET, acontece um fluxo parecido com este:

1. Você escreve o código em C# (`.cs`).
2. O compilador converte esse código para **IL (Intermediate Language)**.
3. O resultado vira um assembly (`.dll` ou `.exe`).
4. Quando você roda o programa, o **CLR** e o **JIT** convertem o IL em código de máquina.
5. O sistema operacional executa o código nativo.

---

## Comandos básicos

Dentro da pasta do projeto, o fluxo típico é:

```bash
dotnet restore   # baixa dependências (se necessário)
dotnet build     # compila o projeto
dotnet run       # compila (se precisar) e executa
```

Na prática, durante o desenvolvimento, você muitas vezes usa apenas:

```bash
dotnet run
```

---

## Estrutura mínima de um programa C#

Exemplo simples (Console App):

```csharp
using System;

class Program
{
    static void Main(string[] args)
    {
        Console.WriteLine("Olá, .NET!");
    }
}
```

- O método `Main` é o **ponto de entrada** da aplicação.
- A partir dele, o fluxo de execução segue a lógica que você implementar.

---

## Entendendo o ciclo durante o desenvolvimento

- Você altera o código.
- Roda `dotnet run` ou usa a IDE (F5).
- O .NET recompila (se necessário) e executa novamente.

Com o tempo, esse fluxo se torna natural, e você passa a focar apenas na lógica do programa.