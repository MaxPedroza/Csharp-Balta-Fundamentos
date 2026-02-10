# Utilizando if na prática

---

## Combinação com operadores

Você pode combinar `if` com operadores de comparação e lógicos:

```csharp
if (idade >= 18 && possuiCNH)
{
    Console.WriteLine("Pode dirigir");
}
```

---

## Encadeando condições

```csharp
if (!ativo)
{
    Console.WriteLine("Usuário inativo");
}
else if (bloqueado)
{
    Console.WriteLine("Usuário bloqueado");
}
else
{
    Console.WriteLine("Usuário liberado");
}
```

---

## Dicas

- Use chaves `{ }` mesmo para blocos de uma linha, para evitar erros ao adicionar mais código depois.
- Deixe as condições simples e legíveis; se ficar muito complexo, extraia para métodos auxiliares.