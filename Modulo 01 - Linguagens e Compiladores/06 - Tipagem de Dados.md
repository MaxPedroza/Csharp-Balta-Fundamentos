# Tipagem de Dados

---

## O que é tipo de dado?

Todo valor em um programa tem um **tipo**: número inteiro, número decimal, texto, verdadeiro/falso etc.

A **tipagem** define como a linguagem lida com esses tipos:

- Como declarar.
- Como combinar valores.
- Que erros são detectados (ou não).

Exemplo em C#:

```csharp
int idade = 30;        // inteiro
string nome = "Ana";  // texto
bool ativo = true;     // verdadeiro ou falso
```

---

## Tipagem estática x dinâmica

### Tipagem estática

- O tipo é conhecido **em tempo de compilação**.
- Erros de tipo são detectados **antes** de executar o programa.

Exemplo (C#, Java):

```csharp
int numero = 10;
numero = "dez"; // erro de compilação
```

### Tipagem dinâmica

- O tipo é conhecido **em tempo de execução**.
- O mesmo identificador pode receber valores de tipos diferentes.

Exemplo (Python):

```python
x = 10      # inteiro
x = "dez"  # agora é string
```

---

## Tipagem forte x fraca (ideia geral)

- **Forte**: a linguagem não permite misturar tipos "à força" sem conversão explícita.
- **Fraca**: a linguagem faz conversões automáticas mais agressivas.

Essa classificação pode variar de acordo com autores, mas a ideia é:

- Tipagem **forte** tende a evitar erros silenciosos.
- Tipagem **fraca** tende a ser mais permissiva, mas pode gerar comportamentos inesperados.

---

## Por que isso importa para você?

- Ajuda a **prevenir bugs** difíceis de rastrear.
- Influencia a forma como você **modela dados** em suas aplicações.
- Afeta a **clareza** e a **manutenibilidade** do código.

Como desenvolvedor C#, você trabalhará com **tipagem estática e forte**, o que traz bastante segurança em projetos grandes.