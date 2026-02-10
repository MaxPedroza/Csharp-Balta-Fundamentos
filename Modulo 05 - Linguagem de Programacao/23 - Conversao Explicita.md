# Conversão explícita

---

## O que é?

Conversão **explícita** é quando você diz ao compilador, de forma clara, que quer converter um tipo para outro, mesmo havendo risco de perda de informação.

Feita com **cast**:

```csharp
double x = 10.75;
int y = (int)x; // y = 10 (parte decimal é perdida)
```

---

## Exemplos

- `double` → `int`
- `long` → `int`
- `int` → `byte`

---

## Riscos

- Perda de parte do valor (casas decimais, estouro de intervalo).
- Exceções em tempo de execução se o valor não couber no tipo de destino (quando usado com `checked`).

---

## Boas práticas

- Faça conversões explícitas apenas quando tiver certeza do que está fazendo.
- Quando possível, valide antes se o valor cabe no novo tipo.