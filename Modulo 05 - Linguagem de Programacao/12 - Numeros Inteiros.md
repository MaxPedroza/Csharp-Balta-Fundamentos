# Números inteiros

---

## Tipos inteiros em C#

Os principais tipos inteiros são:

| Tipo  | Tamanho  | Intervalo aproximado            |
|-------|----------|---------------------------------|
| `byte`  | 8 bits  | 0 a 255                         |
| `short` | 16 bits | -32.768 a 32.767                |
| `int`   | 32 bits | -2 bilhões a +2 bilhões         |
| `long`  | 64 bits | valores muito maiores           |

No dia a dia, **`int`** é o tipo inteiro mais utilizado.

---

## Exemplo

```csharp
int quantidade = 10;
short anos = 20;
long populacao = 2000000000L;
```

Note o sufixo `L` para indicar `long` em literais muito grandes.

---

## Operações básicas

```csharp
int a = 10;
int b = 3;

int soma = a + b;
int subtracao = a - b;
int multiplicacao = a * b;
int divisao = a / b; // divisão inteira
```

Dividir inteiros resulta em **inteiro**, descartando casas decimais.

---

## Boas práticas

- Use `int` por padrão, a menos que tenha um motivo claro para outro tipo.
- Tenha cuidado com estouro (`overflow`) ao somar valores muito grandes.