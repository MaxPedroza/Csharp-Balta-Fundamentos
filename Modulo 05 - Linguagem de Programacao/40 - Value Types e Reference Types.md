# Value types e reference types

---

## Tipos por valor (value types)

- Armazenam **diretamente o valor**.
- Normalmente alocados na **stack**.
- Exemplos: `int`, `double`, `bool`, `char`, `structs`.

Quando você atribui um value type a outra variável, é feita **cópia** do valor.

```csharp
int a = 10;
int b = a; // b recebe uma CÓPIA de a
b = 20;
// a continua 10
```

---

## Tipos por referência (reference types)

- Armazenam uma **referência** a um objeto na memória (heap).
- Exemplos: `string`, classes (`class`), arrays.

```csharp
int[] numeros1 = { 1, 2, 3 };
int[] numeros2 = numeros1; // mesma referência

numeros2[0] = 99;
// numeros1[0] também será 99
```

---

## Por que isso importa?

- Afeta como dados são **copiados** e **compartilhados** entre métodos.
- Ajuda a evitar bugs relacionados a modificações inesperadas em objetos compartilhados.