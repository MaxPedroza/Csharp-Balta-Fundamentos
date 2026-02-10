# Métodos e funções

---

## O que são métodos?

Métodos (ou funções) são **blocos de código reutilizáveis**, que recebem parâmetros, executam uma lógica e (opcionalmente) retornam um valor.

---

## Estrutura básica

```csharp
[modificador] tipoRetorno NomeMetodo(parâmetros)
{
    // corpo do método
}
```

Exemplo:

```csharp
static int Somar(int a, int b)
{
    return a + b;
}
```

---

## Chamando um método

```csharp
int resultado = Somar(2, 3);
Console.WriteLine(resultado); // 5
```

---

## Vantagens

- Reuso de código.
- Organização e clareza.
- Facilidade de teste.

Dividir seu código em métodos bem nomeados é uma das habilidades mais importantes em programação.