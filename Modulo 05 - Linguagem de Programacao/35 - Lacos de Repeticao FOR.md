# Laços de repetição: for

---

## Estrutura básica

```csharp
for (inicialização; condição; incremento)
{
    // código repetido enquanto a condição for verdadeira
}
```

---

## Exemplo

```csharp
for (int i = 0; i < 5; i++)
{
    Console.WriteLine($"Valor de i: {i}");
}
```

- `int i = 0;` → inicialização.
- `i < 5;` → condição.
- `i++` → incremento a cada iteração.

---

## Uso comum

- Percorrer intervalos numéricos.
- Iterar sobre arrays usando índices.