# Escopo de um programa

---

## O que é escopo?

**Escopo** é a região do código onde uma variável, função ou estrutura é **visível** e pode ser utilizada.

Em C#, o escopo é definido principalmente por **chaves** `{ }`.

---

## Exemplo simples

```csharp
using System;

class Program
{
    static void Main(string[] args)
    {
        int x = 10; // escopo de x começa aqui

        if (x > 5)
        {
            int y = 20; // escopo de y é apenas dentro do if
            Console.WriteLine(x + y);
        }

        // Console.WriteLine(y); // ERRO: y não existe neste escopo
    }
}
```

---

## Tipos de escopo

- **Escopo de bloco**: dentro de `{ }` (if, for, while, métodos, classes).
- **Escopo de método**: variáveis declaradas dentro de um método.
- **Escopo de classe**: campos e propriedades acessíveis pelos métodos da classe.

Entender escopo evita erros como "nome não existe no contexto atual".

---

## Boas práticas

- Declare variáveis **o mais próximo possível** de onde serão usadas.
- Evite variáveis com escopo muito amplo sem necessidade.
- Use nomes claros, pois muitos nomes parecidos em escopos diferentes podem confundir.