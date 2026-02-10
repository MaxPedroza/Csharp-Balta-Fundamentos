# Char

---

## O tipo `char`

`char` representa **um único caractere Unicode**.

Exemplos de valores válidos:

```csharp
char letra = 'A';
char digito = '9';
char simbolo = '#';
```

Note o uso de **aspas simples**.

---

## Operações comuns

- Verificar se é letra, número, espaço etc. usando métodos de `char`:

```csharp
char c = 'A';

bool eLetra = char.IsLetter(c);
bool eNumero = char.IsDigit(c);
```

---

## Quando usar `char`?

- Quando trabalha com **análise de texto** caractere a caractere.
- Ao percorrer uma `string` e examinar cada posição individualmente.