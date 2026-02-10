# Operador condicional: if

---

## Estrutura básica

```csharp
if (condicao)
{
    // código executado se a condição for verdadeira
}
```

---

## Exemplo simples

```csharp
int idade = 20;

if (idade >= 18)
{
    Console.WriteLine("Maior de idade");
}
```

---

## if/else

```csharp
if (idade >= 18)
{
    Console.WriteLine("Maior de idade");
}
else
{
    Console.WriteLine("Menor de idade");
}
```

---

## if/else if/else

```csharp
if (nota >= 9)
    Console.WriteLine("Excelente");
else if (nota >= 7)
    Console.WriteLine("Bom");
else
    Console.WriteLine("Precisa melhorar");
```

O `if` é a base de quase toda a lógica condicional em C#.