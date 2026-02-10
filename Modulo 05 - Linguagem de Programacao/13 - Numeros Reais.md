# Números reais

---

## Tipos principais

Em C#, os tipos numéricos com **casas decimais** mais usados são:

| Tipo    | Tamanho | Precisão aproximada        |
|---------|---------|----------------------------|
| `float` | 32 bits | 7 dígitos significativos   |
| `double`| 64 bits | 15-16 dígitos significativos|
| `decimal`| 128 bits| alta precisão (financeiro) |

---

## Exemplo

```csharp
float taxa = 1.5f;      // note o sufixo f
double pi = 3.14159;
decimal preco = 199.99m; // sufixo m para decimal
```

---

## Quando usar cada um?

- **double**: padrão para cálculos gerais com casas decimais.
- **float**: quando precisa economizar memória e um pouco menos de precisão é aceitável (gráficos, jogos).
- **decimal**: para **valores monetários** e situações onde precisão é crítica.

---

## Atenção à precisão

Números de ponto flutuante (`float`, `double`) podem ter **pequenos erros de arredondamento**:

```csharp
Console.WriteLine(0.1 + 0.2); // pode não dar exatamente 0.3
```

Por isso, para dinheiro, prefira `decimal`.