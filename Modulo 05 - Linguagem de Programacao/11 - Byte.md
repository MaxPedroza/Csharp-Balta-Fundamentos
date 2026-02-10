# Byte

---

## O tipo `byte`

`byte` é um tipo inteiro **sem sinal** (apenas valores positivos) de **8 bits**.

- Intervalo: `0` a `255`.
- Muito usado para representar **dados binários** (arquivos, imagens, streams) e valores pequenos.

---

## Exemplo

```csharp
byte idade = 30;
byte mascara = 0b_1111_0000; // notação binária
```

---

## Quando usar `byte`?

- Ao trabalhar com **arrays de bytes** (`byte[]`) em operações de rede, criptografia ou arquivos.
- Quando precisa representar números pequenos e quer economizar memória (embora, na prática, `int` seja mais comum no dia a dia).

---

## Observação

- Se você somar dois `byte`, o resultado pode ser promovido para `int`.
- Em operações aritméticas, talvez seja necessário conversão explícita de volta para `byte`.