# Comentários

---

## Para que servem comentários?

Comentários são trechos de texto no código **ignorados pelo compilador**, usados para:

- Explicar trechos de lógica mais complexos.
- Deixar anotações para você ou para o time.
- Documentar comportamentos especiais.

---

## Tipos de comentários em C#

### 1. Linha única

```csharp
// Este é um comentário de linha
int idade = 30; // comentário ao lado do código
```

### 2. Múltiplas linhas

```csharp
/*
   Comentário
   em várias linhas
*/
```

### 3. Comentários de documentação

```csharp
/// <summary>
/// Soma dois números inteiros.
/// </summary>
int Somar(int a, int b) => a + b;
```

---

## Boas práticas

- Comente o **porquê** da lógica, não apenas o que o código faz.
- Não exagere: código claro muitas vezes dispensa comentários.
- Atualize comentários quando alterar o código para evitar informações desatualizadas.