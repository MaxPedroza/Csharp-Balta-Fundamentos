# Conversão implícita

---

## O que é?

Conversão **implícita** acontece quando o compilador converte um valor de um tipo para outro **automaticamente**, sem risco de perda de informação.

Exemplo clássico:

```csharp
int x = 10;
double y = x; // conversão implícita de int para double
```

`double` consegue representar todos os valores que um `int` consegue, por isso a conversão é segura.

---

## Exemplos comuns

- `int` → `long`
- `float` → `double`
- Qualquer tipo para `object`

---

## Vantagens

- Código mais limpo, sem necessidade de casts.
- Menos chance de erro quando conversões são realmente seguras.

Sempre que houver risco de perda de informação, a conversão **não será implícita** (ver próxima aula sobre conversão explícita).