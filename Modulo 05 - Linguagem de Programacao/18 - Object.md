# object

---

## O tipo `object`

`object` é o **tipo base** de todos os tipos em C#.

Qualquer valor pode ser referenciado como `object`:

```csharp
object x = 10;        // int
object y = "texto";  // string
object z = true;      // bool
```

---

## Boxing e unboxing

Quando um tipo de valor (como `int`) é armazenado em um `object`, acontece o **boxing** (empacotamento). Para recuperar, é necessário **unboxing** (conversão de volta):

```csharp
object obj = 10;      // boxing
int numero = (int)obj; // unboxing
```

---

## Quando usar `object`?

- Em APIs muito genéricas, onde o tipo pode variar.
- Em cenários específicos de interoperabilidade.

No dia a dia, prefira sempre tipos **específicos** (como `int`, `string`) para evitar conversões desnecessárias e erros em tempo de execução.