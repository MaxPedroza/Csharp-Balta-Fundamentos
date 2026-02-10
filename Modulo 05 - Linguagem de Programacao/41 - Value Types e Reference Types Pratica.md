# Value types e reference types: prática

---

## Exemplo comparando comportamentos

```csharp
static void Main()
{
    int x = 10;
    AlterarValor(x);
    Console.WriteLine(x); // 10 (não mudou)

    int[] numeros = { 1, 2, 3 };
    AlterarArray(numeros);
    Console.WriteLine(numeros[0]); // 99 (mudou)
}

static void AlterarValor(int valor)
{
    valor = 20;
}

static void AlterarArray(int[] array)
{
    array[0] = 99;
}
```

- `int` é **value type** → cópia.
- `int[]` é **reference type** → altera o mesmo objeto.

---

Brinque com exemplos assim para fixar bem a diferença entre tipos de valor e tipos de referência.