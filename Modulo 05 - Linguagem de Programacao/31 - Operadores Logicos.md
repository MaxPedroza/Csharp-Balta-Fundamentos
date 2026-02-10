# Operadores lógicos

---

## Principais operadores

| Operador | Nome      | Exemplo            |
|----------|-----------|--------------------|
| `&&`     | E lógico  | `cond1 && cond2`   |
| `||`     | OU lógico | `cond1 || cond2`   |
| `!`      | NÃO lógico| `!condicao`        |

Eles trabalham com valores booleanos (`true` ou `false`).

---

## Exemplo

```csharp
bool maiorDeIdade = idade >= 18;
bool temCarteira = possuiCNH;

bool podeDirigir = maiorDeIdade && temCarteira;
```

```csharp
bool fimDeSemana = dia == "Sabado" || dia == "Domingo";

bool naoAtivo = !ativo;
```

---

## Curto-circuito

- Em `cond1 && cond2`, se `cond1` for `false`, `cond2` **não é avaliada**.
- Em `cond1 || cond2`, se `cond1` for `true`, `cond2` **não é avaliada**.

Isso pode evitar chamadas desnecessárias e até erros.