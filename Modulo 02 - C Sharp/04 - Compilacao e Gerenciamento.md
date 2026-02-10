# Compilação e gerenciamento

---

## O que acontece quando você compila um projeto C#?

Fluxo simplificado:

1. Você escreve o código em C# (`.cs`).
2. O compilador C# (csc) converte esse código para **IL (Intermediate Language)**.
3. O resultado é um assembly (`.dll` ou `.exe`) contendo IL e metadados.
4. Em tempo de execução, o **CLR** usa o **JIT (Just-In-Time Compiler)** para converter IL em código de máquina específico da plataforma.

---

## Papel do CLR no gerenciamento

Além de participar da execução (via JIT), o CLR gerencia:

- **Memória**: controla o *heap* gerenciado, onde objetos são alocados.
- **Garbage Collector**: identifica objetos que não são mais utilizados e libera memória automaticamente.
- **Threads**: oferece suporte a multitarefa, *thread pool* etc.
- **Segurança**: garante que o código respeite regras de acesso e tipos.

---

## Vantagens desse modelo

- **Abstração da plataforma**: o mesmo assembly pode rodar em diferentes sistemas onde exista uma implementação do .NET.
- **Otimizações em tempo de execução**: o JIT pode gerar código otimizado para o processador/alvo.
- **Gerenciamento automático de recursos**: reduz erros de memória e recursos não liberados.

---

## Exemplo visual (resumo)

```text
C# (.cs)  --compilador-->  IL (.dll / .exe)  --CLR/JIT-->  Código de máquina
```

Esse fluxo é o coração de como aplicações C#/.NET são executadas.