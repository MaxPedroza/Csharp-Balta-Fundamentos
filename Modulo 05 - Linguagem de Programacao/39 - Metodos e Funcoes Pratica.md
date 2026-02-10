# Métodos e funções: prática

---

## Exemplo 1 – Validação simples

```csharp
static bool EhMaiorDeIdade(int idade)
{
    return idade >= 18;
}

static void Main()
{
    Console.Write("Idade: ");
    int idade = int.Parse(Console.ReadLine());

    if (EhMaiorDeIdade(idade))
        Console.WriteLine("Maior de idade");
    else
        Console.WriteLine("Menor de idade");
}
```

---

## Exemplo 2 – Método sem retorno

```csharp
static void ExibirMensagem(string mensagem)
{
    Console.WriteLine(mensagem);
}

ExibirMensagem("Olá, métodos em C#!");
```

---

## Dicas

- Cada método deve ter uma **responsabilidade clara**.
- Nomes de método devem ser **verbos**: `CalcularTotal`, `EnviarEmail`, `ValidarUsuario`.