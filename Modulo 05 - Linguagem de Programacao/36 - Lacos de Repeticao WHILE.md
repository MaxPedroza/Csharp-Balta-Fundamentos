# Laços de repetição: while

---

## Estrutura básica

```csharp
while (condicao)
{
    // código repetido enquanto a condição for verdadeira
}
```

---

## Exemplo

```csharp
int contador = 0;

while (contador < 5)
{
    Console.WriteLine(contador);
    contador++;
}
```

---

## Quando usar `while`?

- Quando não sabe, de antemão, quantas repetições serão necessárias.
- Quando a repetição depende de uma condição externa (entrada do usuário, leitura de arquivo, etc.).