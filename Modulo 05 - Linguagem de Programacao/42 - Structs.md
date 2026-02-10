# Structs

---

## O que é uma struct?

`struct` é um tipo de valor **definido pelo usuário**, parecido com uma classe simples.

- Usado para representar **estruturas pequenas de dados**.
- Por ser value type, é copiado por valor.

---

## Exemplo

```csharp
public struct Ponto
{
    public int X;
    public int Y;
}

Ponto p1 = new Ponto { X = 10, Y = 20 };
Ponto p2 = p1; // cópia
p2.X = 99;
// p1.X continua 10
```

---

## Quando usar structs?

- Para tipos pequenos, imutáveis e que representam um **valor** (e não uma entidade complexa).
- Ex.: coordenadas, cores, dimensões.

Na dúvida, use **classes**; structs são para cenários específicos.