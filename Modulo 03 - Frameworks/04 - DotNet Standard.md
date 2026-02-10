# .NET Standard

---

## Problema: dois frameworks, muitas bibliotecas

Durante um período, o ecossistema .NET tinha:

- **.NET Framework** (clássico, focado em Windows).
- **.NET Core** (novo, multiplataforma).

Ambos podiam coexistir e até serem usados no mesmo projeto, o que gerava dúvida:

> "Se eu criar uma biblioteca, ela vai funcionar tanto no .NET Framework quanto no .NET Core?"

---

## O que é o .NET Standard?

O **.NET Standard** surgiu como uma **padronização de APIs**:

- Define um **conjunto mínimo de funcionalidades** que todos os frameworks .NET devem implementar.
- É uma **Surface API**: uma "superfície" de métodos, tipos e namespaces.
- Não é algo que você "instala" ou "roda"; é uma **especificação**.

Você não "programa em .NET Standard"; você cria bibliotecas **que atendem ao .NET Standard**, garantindo compatibilidade.

---

## Benefícios práticos

- Uma biblioteca criada para **.NET Standard** pode ser usada tanto em **.NET Framework** quanto em **.NET Core** (desde que suportem aquela versão do Standard).
- Redução de duplicação de código.
- Facilita compartilhamento de bibliotecas entre diferentes tipos de aplicações.

---

## Resumo

- .NET Standard = **interseção comum** entre diferentes frameworks .NET.
- Garante que código reutilizável funcione em múltiplos ambientes.
- Foi uma peça importante na transição para a plataforma unificada .NET 5+.