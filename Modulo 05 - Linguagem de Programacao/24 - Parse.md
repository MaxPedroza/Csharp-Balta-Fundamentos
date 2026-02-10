# Parse

---

## O que é `Parse`?

Métodos `Parse` convertem **texto (`string`) em tipos de valor**.

Exemplo:

```csharp
string texto = "25";
int idade = int.Parse(texto); // idade = 25
```

Se o texto não estiver em um formato válido, `Parse` lança uma exceção.

---

## Exemplos comuns

```csharp
int numero = int.Parse("10");
double valor = double.Parse("3,14"); // depende da cultura
bool ativo = bool.Parse("true");
DateTime data = DateTime.Parse("2020-10-01");
```

---

## `TryParse`

Versão mais segura, que **não lança exceção** em caso de erro:

```csharp
if (int.TryParse("25", out int resultado))
{
    Console.WriteLine(resultado);
}
else
{
    Console.WriteLine("Valor inválido");
}
```

Use `TryParse` sempre que estiver lidando com entradas externas (usuário, arquivos, etc.).