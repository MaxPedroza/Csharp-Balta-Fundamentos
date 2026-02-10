# Variáveis

---

## O que é uma variável?

Uma **variável** é um espaço na memória com:

- Um **nome**.
- Um **tipo**.
- Um **valor** (que pode mudar, exceto em constantes).

---

## Declarando variáveis em C#

```csharp
int idade = 25;
string nome = "Ana";
bool ativo = true;
```

- `int` → número inteiro.
- `string` → texto.
- `bool` → verdadeiro/falso.

---

## Regras básicas de nomes

- Não pode começar com número.
- Não pode conter espaços.
- Evite caracteres especiais.
- Use **camelCase** para variáveis locais: `quantidadeTotal`, `valorProduto`.

---

## Boas práticas

- Use nomes que façam sentido: `idade`, `precoProduto`, `dataCadastro`.
- Comece com tipos simples e claros, não complique cedo demais.
- Inicialize as variáveis sempre que possível para evitar uso sem valor definido.