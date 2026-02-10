# Boolean

---

## O tipo `bool`

`bool` representa apenas dois valores possíveis:

- `true` (verdadeiro)
- `false` (falso)

É o tipo fundamental para **condições** em estruturas como `if`, `while`, `for`.

---

## Exemplo

```csharp
bool ativo = true;

if (ativo)
{
    Console.WriteLine("Usuário ativo");
}
```

Também é resultado de **operações de comparação**:

```csharp
int idade = 20;
bool maiorDeIdade = idade >= 18; // true
```

---

## Boas práticas

- Use nomes que pareçam perguntas: `estaLogado`, `temPermissao`, `ehValido`.
- Evite comparar com `true`/`false` desnecessariamente:

```csharp
if (maiorDeIdade) { ... } // melhor
if (maiorDeIdade == true) { ... } // desnecessário
```}},{