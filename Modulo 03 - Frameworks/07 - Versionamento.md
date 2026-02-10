# Versionamento do .NET

---

## Como o .NET é versionado?

As versões do .NET seguem, em geral, um esquema como:

```text
MAIOR.MENOR.PATCH
Ex.: 3.1.201
```

- **MAIOR** (3) → alteraçãos grandes, novas funcionalidades importantes.
- **MENOR** (1) → incrementos menores, ainda dentro da mesma linha principal.
- **PATCH** (201) → correções pequenas, chamadas de *minor changes*.

Essas pequenas correções normalmente **não quebram** o código já existente.

---

## Breaking changes x minor changes

- **Minor changes**: ajustes internos, correções de bugs, melhorias; não exigem mudanças no seu código.
- **Breaking changes**: alterações que podem **quebrar** código que já funcionava (mudança de assinatura de métodos, remoção de APIs, etc.).

Versões com breaking changes costumam estar associadas a saltos de versão **maior**.

---

## Convivência de versões

O .NET (especialmente o .NET Core) permite instalação **lado a lado** de versões diferentes:

- Você pode ter, por exemplo, a 2.0 e a 3.1 instaladas ao mesmo tempo.
- Cada projeto pode apontar para uma versão específica do framework.

Isso facilita:

- Manter projetos antigos em versões estáveis.
- Desenvolver novos projetos em versões mais recentes.

---

## Dica prática

- Sempre consulte a documentação oficial para ver:
  - Qual é a versão atual.
  - Quais são as versões LTS.
  - Até quando cada versão terá suporte.

Assim, você planeja melhor quando **atualizar** seus projetos.