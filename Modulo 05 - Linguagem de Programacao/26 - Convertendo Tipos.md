# Convertendo tipos

---

## Visão geral

Em C#, você pode converter tipos de várias maneiras:

- **Conversão implícita** (automática, sem perda de informação).
- **Conversão explícita** (cast).
- Métodos de **parse** (`int.Parse`, `double.Parse`).
- Métodos da classe **`Convert`**.

---

## Exemplo completo

```csharp
int inteiro = 10;

// Implícita
double real = inteiro;

// Explícita
int inteiro2 = (int)3.75;

// Parse
int idade = int.Parse("25");

// Convert
double valor = Convert.ToDouble("10,5");
```

---

## Boas práticas

- Prefira **implícita** quando não houver risco de perda de dados.
- Use **parse/Convert** ao lidar com **strings** vindas de entrada do usuário.
- Sempre que puder haver erro de formatação, use `TryParse`.

Entender bem conversões é essencial para evitar bugs sutis em aplicações reais.