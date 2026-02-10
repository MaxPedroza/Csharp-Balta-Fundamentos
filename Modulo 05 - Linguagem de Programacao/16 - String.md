# String

---

## O tipo `string`

`string` representa uma **sequência de caracteres** (texto).

```csharp
string nome = "Ana";
string mensagem = "Bem-vindo ao curso de C#!";
```

---

## Operações básicas

```csharp
string nomeCompleto = "Ana " + "Silva"; // concatenação
int tamanho = nomeCompleto.Length;       // tamanho da string
string maiusculo = nomeCompleto.ToUpper();
string minusculo = nomeCompleto.ToLower();
```

---

## Interpolação de strings

Forma moderna e legível de montar textos:

```csharp
int idade = 25;
string frase = $"Meu nome é {nome} e tenho {idade} anos.";
```

---

## Boas práticas

- Use `string.Empty` em vez de `""` quando fizer muitas inicializações.
- Prefira interpolação (`$"..."`) a muitas concatenações com `+`.
- Atenção a espaços extras ou quebras de linha involuntárias.