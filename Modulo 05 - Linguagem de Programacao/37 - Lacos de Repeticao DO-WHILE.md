# Laços de repetição: do/while

---

## Estrutura básica

```csharp
do
{
    // código executado pelo menos uma vez
}
while (condicao);
```

---

## Exemplo

```csharp
string opcao;

do
{
    Console.WriteLine("Digite S para sair");
    opcao = Console.ReadLine();
}
while (opcao != "S");
```

Aqui o bloco será executado **ao menos uma vez**, pois a condição só é verificada ao final.

---

## Quando usar

- Quando é necessário que o bloco execute pelo menos uma vez antes de checar a condição.