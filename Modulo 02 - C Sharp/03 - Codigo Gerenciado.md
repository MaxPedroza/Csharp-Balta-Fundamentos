# Código gerenciado

---

## O que é código gerenciado?

No contexto do .NET, **código gerenciado** é o código que:

- É compilado para **IL (Intermediate Language)**.
- É executado dentro do **CLR (Common Language Runtime)**.

O CLR é como um ambiente de execução que oferece diversos serviços ao seu programa.

---

## Serviços oferecidos pelo CLR

Quando você escreve código C# e ele é executado como código gerenciado, o CLR cuida de várias coisas para você:

- **Gerenciamento de memória** (alocação e liberação através do *Garbage Collector*).
- **Tratamento de exceções** padronizado.
- **Segurança de tipos** (type safety).
- **Verificações de segurança** (code access security, em contextos específicos).

Isso tudo ajuda a tornar as aplicações mais estáveis e seguras.

---

## Código gerenciado x código não gerenciado

- **Código gerenciado**: roda dentro do CLR.
  - Ex.: C#, VB.NET, F#.

- **Código não gerenciado**: roda diretamente no sistema operacional, sem o CLR.
  - Ex.: Aplicações em C ou C++ nativos, chamadas via ponteiros, etc.

O .NET permite que, quando necessário, você interaja com código não gerenciado (por exemplo, chamando bibliotecas nativas), mas o foco do dia a dia é o código gerenciado.

---

## Vantagens do código gerenciado

- Menos chances de erros graves de memória (como *buffer overflow* ou *memory leak* por esquecimento de liberar memória).
- Modelo de programação mais simples para a maioria dos desenvolvedores.
- Melhor portabilidade entre diferentes sistemas suportados pelo .NET.

Entender o conceito de código gerenciado ajuda a compreender como o C# consegue oferecer **segurança**, **produtividade** e **boa performance** ao mesmo tempo.