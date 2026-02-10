# Alto e Baixo Nível

---

## Ideia principal

As linguagens de programação podem ser classificadas de acordo com o **nível de abstração** em relação ao hardware:

- **Alto nível**: mais próximas da forma como humanos pensam.
- **Baixo nível**: mais próximas de como a máquina realmente funciona.

---

## Linguagens de alto nível

Características:

- Sintaxe mais amigável e expressiva.
- Escondem detalhes de hardware (registradores, endereços de memória, etc.).
- Focadas em **produtividade** e **legibilidade**.

Exemplos: C#, Java, Python, JavaScript.

Trecho em C# (alto nível):

```csharp
var numeros = new int[] { 1, 2, 3, 4, 5 };

foreach (var numero in numeros)
{
    Console.WriteLine(numero);
}
```

Você não se preocupa com **endereços de memória**, apenas com a lógica.

---

## Linguagens de baixo nível

Características:

- Mais próximas do **código de máquina**.
- Dão maior controle sobre memória e hardware.
- Geralmente mais difíceis de aprender e ler.

Exemplos: Assembly, C (em muitos contextos é considerado mais baixo nível que C#).

Trecho ilustrativo em Assembly (simplificado):

```asm
MOV AX, 1
ADD AX, 2
```

Aqui, você manipula diretamente **registradores** do processador.

---

## Comparando

| Característica     | Alto nível                         | Baixo nível                         |
|--------------------|------------------------------------|-------------------------------------|
| Legibilidade       | Alta                               | Baixa                               |
| Controle do hardware | Menor                            | Maior                               |
| Produtividade      | Alta                               | Baixa (em geral)                    |
| Uso comum          | Aplicações de negócio, web, apps   | Sistemas operacionais, drivers      |

---

## Quando usar qual?

- No dia a dia, você trabalhará principalmente com **alto nível**.
- Em áreas específicas (sistemas operacionais, embarcados, games muito otimizados), o **baixo nível** ainda é essencial.

Entender a diferença ajuda a valorizar o trabalho que as linguagens de alto nível fazem para simplificar sua vida.