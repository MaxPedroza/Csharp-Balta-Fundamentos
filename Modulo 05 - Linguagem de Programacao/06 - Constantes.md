# Constantes

---

## O que é uma constante?

Uma **constante** é um valor que **não muda** durante a execução do programa.

Em C#, usamos a palavra-chave `const`.

---

## Exemplo

```csharp
const double Pi = 3.14159;
const int AnoNascimento = 1990;

Console.WriteLine(Pi);
```

Tentar alterar o valor de `Pi` depois vai gerar erro de compilação.

---

## Quando usar constantes?

- Valores fixos, conhecidos em tempo de compilação.
- Ex.: número de dias da semana, taxa de IOF (se for fixa no contexto do sistema), limites pré-definidos.

---

## Boas práticas

- Use nomes em **PascalCase** para constantes (`TaxaJurosBase`).
- Agrupe constantes relacionadas em uma mesma classe/arquivo quando fizer sentido.