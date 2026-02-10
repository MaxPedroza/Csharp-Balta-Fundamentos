# Enums

---

## O que é um enum?

`enum` é um tipo especial que representa um **conjunto de valores nomeados**.

Exemplo:

```csharp
public enum StatusPedido
{
    Pendente,
    Pago,
    Cancelado
}
```

---

## Uso

```csharp
StatusPedido status = StatusPedido.Pago;

if (status == StatusPedido.Pago)
{
    Console.WriteLine("Pedido pago");
}
```

---

## Vantagens

- Evita o uso de "valores mágicos" (como `1`, `2`, `3` para representar estados).
- Torna o código mais legível e seguro.

Por baixo dos panos, um `enum` é armazenado como um tipo inteiro (por padrão, `int`).